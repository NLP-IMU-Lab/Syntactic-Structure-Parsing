��������ļ���ʽ��������train.txt �� test.txt

����˵����
	ѵ����
		MonParser.exe -train -trainFile train.txt -modelFile model.mod
		-train��˵�������������ѵ��
		-trainFile�����Ĳ���(train.txt)Ϊѵ���ļ���
		-modelFile�����Ĳ���(model.mod)Ϊģ���ļ���
	���ԣ�
		1. �������ļ����в���
		MonParser.exe -test -testFile test.txt -modelFile model.mod -outFile out.txt
		-test��˵��������������������ļ����в���
		-testFile�����Ĳ���(test.txt)Ϊ�����ļ���
		-modelFile�����Ĳ���(model.mod)Ϊģ���ļ���	
		-outFile�����Ĳ���(out.txt)Ϊ����ļ���	

		2. �ôʺʹ��Ա�ע���е��ļ����в���
		MonParser.exe -parse -parseFile parse.txt -modelFile model.mod -outFile out.txt
		-parse��˵��������������ôʺʹ��Ա�ע���е��ļ����в���
		-parseFile�����Ĳ���(parse.txt)Ϊ�����ļ���
		-modelFile�����Ĳ���(model.mod)Ϊģ���ļ���	
		-outFile�����Ĳ���(out.txt)Ϊ����ļ���	

ע��ѵ���Ͳ��Կ�����ͬһ������ִ�У����磺
>MonParser.exe -train -trainFile train.txt -modelFile model.mod -test -testFile test.txt -outFile out.txt
��-test��-parse����ģʽ������ͬһ��������ִ��