# 一、实验内容
##### 某学校为了给学生提供勤工俭学机会，也减轻授课教师的部分压力，准许博士研究生参与课程的助教工作。此时，该博士研究生有双重身份：学生和助教教师。
##### (1)设计两个管理接口：学生管理接口和教师管理接口。学生接口必须包括缴纳学费、查学费的方法；教师接口包括发放薪水和查询薪水的方法。
##### (2)设计博士研究生类，实现上述的两个接口，该博士研究生应具有姓名、性别、年龄、每学期学费、每月薪水等属性。（其他属性及方法，可自行发挥）
##### (3)编写测试类，并实例化至少两名博士研究生，统计他们的年收入和学费。根据两者之差，算出每名博士研究生的年应纳税金额（国家最新工资纳税标准，请自行检索）。

# 二、实验要求
##### (1)在博士研究生类中实现各个接口定义的抽象方法;
##### (2)对年学费和年收入进行统计，用收入减去学费，求得纳税额；
##### (3)国家最新纳税标准（系数），属于某一时期的特定固定值，与实例化对象没有关系，考虑如何用static  final修饰定义。
##### (4)实例化研究生类时，可采用运行时通过main方法的参数args一次性赋值，也可采用Scanner类实现运行时交互式输入。
##### (5)根据输入情况，要在程序中做异常处理。

# 三、实验方法
##### 1、用interface方法连接定义student和teacher两个类。
##### 2、定义Graduate类，编写其年收入，学费等方法。
##### 3、编写setRate类，并继承Graduate，在setRate类中编写税率的计算方法。
##### 4、编写Test测试类，其中接受用户输入的信息并用try方法处理异常。

# 五、核心代码
``` 

public interface teacher {
    public abstract void setPay(double pay);
    public abstract void getPay(double pay);
}

public interface student {
    public abstract void setFee(double fee);
    public abstract void getFee(double fee);

}

```

# 六、结果截图
![实验4](https://github.com/wangruifengwrf/Javashiyan4/blob/main/%E5%AE%9E%E9%AA%8C4.png)

# 七、感想
