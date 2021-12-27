输入输出文件格式见样例：train.txt 和 test.txt

命令说明：
	训练：
		MonParser.exe -train -trainFile train.txt -modelFile model.mod
		-train：说明本次任务包括训练
		-trainFile：其后的参数(train.txt)为训练文件名
		-modelFile：其后的参数(model.mod)为模型文件名
	测试：
		1. 用树库文件进行测试
		MonParser.exe -test -testFile test.txt -modelFile model.mod -outFile out.txt
		-test：说明本次任务包括用树库文件进行测试
		-testFile：其后的参数(test.txt)为测试文件名
		-modelFile：其后的参数(model.mod)为模型文件名	
		-outFile：其后的参数(out.txt)为输出文件名	

		2. 用词和词性标注序列的文件进行测试
		MonParser.exe -parse -parseFile parse.txt -modelFile model.mod -outFile out.txt
		-parse：说明本次任务包括用词和词性标注序列的文件进行测试
		-parseFile：其后的参数(parse.txt)为测试文件名
		-modelFile：其后的参数(model.mod)为模型文件名	
		-outFile：其后的参数(out.txt)为输出文件名	

注：训练和测试可以在同一次任务执行，例如：
>MonParser.exe -train -trainFile train.txt -modelFile model.mod -test -testFile test.txt -outFile out.txt
但-test和-parse两种模式不能在同一次任务中执行