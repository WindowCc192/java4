# java4
实验四
## 实验目的
1.掌握Java中抽象类和抽象方法的定义；
2.掌握Java中接口的定义，熟练掌握接口的定义形式以及接口的实现方法
3.了解异常的使用方法，并在程序中根据输入情况做异常处理
## 实验要求
1.在博士研究生类中实现各个接口定义的抽象方法;
2.对年学费和年收入进行统计，用收入减去学费，求得纳税额；
3.国家最新纳税标准（系数），属于某一时期的特定固定值，与实例化对象没有关系，考虑如何用static final修饰定义。
4.实例化研究生类时，可采用运行时通过main方法的参数args一次性赋值，或者交互性赋值
## 核心代码
DoctoralCandidate doc1 = new DoctoralCandidate("赵五", "男", 25, 4500, 8000);
		//DoctoralCandidate doc2 = new DoctoralCandidate("刘一", "女", 22, 5200, 7250);
		StudentManagement stu1 = doc1;
		//StudentManagement stu2 = doc2;
		TeacherManagement tea1 = doc1;
		//TeacherManagement tea2 = doc2;
		System.out.println("第二个");
		try {
			giveSalary(doc1.getSalary(),doc1.getTuition());
			doc1.giveSalary(doc1.getSalary(),giveRevenue(doc1.getSalary(),doc1.getTuition()));
			stu1.searchTuition();
			tea1.searchSalary();	
		}
		catch(MoneyException e) {
			System.out.println("请输入正确学费！");
			System.out.println(e.warnMess());
	    }
//		System.out.println("第二个");
//		try {
//			giveSalary(doc2.getSalary(),doc2.getTuition());
//			doc2.giveSalary(doc2.getSalary(),giveRevenue(doc2.getSalary(),doc2.getTuition()));
//			stu2.searchTuition();
//			tea2.searchSalary();	
//		}
//		catch(MoneyException e) {
//			System.out.println("请输入正确学费！");
//			System.out.println(e.warnMess());
//	  
## 实验结果
 如文件中所示
## 实验感想
实验本身对我个人来说具有一定难度，所涉及的Java知识掌握不够。对于逻辑方面的理解不够到位。应该在完成实验之后，去尝试熟练掌握知识，以补充实验和课堂的不足。
