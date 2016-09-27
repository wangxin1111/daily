2016.9.22.pm.工作日志
====================
*1. 今日所学
 public interface UsbInterface {

/**

USB接口提供服务。 */

void service();

}

public class UDisk implements UsbInterface { public void service() { System.out.println("连接USB口，开始传输数据。"); }

} UsbInterface uDisk = new UDisk(); uDisk.service();
 2. 已完成工作
 *1.构造函数**
 String(byte[ ] bytes)：通过byte数组构造字符串对象。
 String(char[ ] value)：通过char数组构造字符串对象。
 String(Sting original)：构造一个original的副本。即：拷贝一个original。
 String(StringBuffer buffer)：通过StringBuffer数组构造字符串对象。  
例如：
  byte[] b = {'a','b','c','d','e','f','g','h','i','j'};
  char[] c = {'0','1','2','3','4','5','6','7','8','9'};
  String sb = new String(b);                 
  String sb_sub = new String(b,3,2);    
  String sc = new String(c);                  
  String sc_sub = new String(c,3,2);    
  String sb_copy = new String(sb);        
  System.out.println("sb:"+sb);
  System.out.println("sb_sub:"+sb_sub);
  System.out.println("sc:"+sc);
  System.out.println("sc_sub:"+sc_sub);
  System.out.println("sb_copy:"+sb_copy);

输出结果：sb:abcdefghij
         sb_sub:de
         sc:0123456789
         sc_sub:34
         sb_copy:abcdefghij
 2.构造方法
说明: 1、所有方法均为public。
      2、书写格式： [修饰符] <返回类型><方法名([参数列表])>
例如：static int parseInt(String s)
表示此方法(parseInt)为类方法(static),返回类型为(int),方法所需要为String类型。
1. char charAt(int index) ：取字符串中的某一个字符，其中的参数index指的是字符串中序数。字符串的序数从0开始到length()-1 。
    例如：String s = new String("abcdefghijklmnopqrstuvwxyz");
          System.out.println("s.charAt(5): " + s.charAt(5) );
          结果为： s.charAt(5): f
2. int compareTo(String anotherString) ：当前String对象与anotherString比较。相等关系返回0；不相等时，从两个字符串第0个字符开始比较，返回第一个不相等的字符差，另一种情况，较长字符串的前面部分恰巧是较短的字符串，返回它们的长度差。
3. int compareTo(Object o) ：如果o是String对象，和2的功能一样；否则抛出ClassCastException异常。
    例如:String s1 = new String("abcdefghijklmn");
            String s2 = new String("abcdefghij");
           String s3 = new String("abcdefghijalmn");
           System.out.println("s1.compareTo(s2): " + s1.compareTo(s2) ); //返回长度差
           System.out.println("s1.compareTo(s3): " + s1.compareTo(s3) ); //返回'k'-'a'的差
           结果为：s1.compareTo(s2): 4
                       s1.compareTo(s3): 10
4. String concat(String str) ：将该String对象与str连接在一起。
5. boolean contentEquals(StringBuffer sb) ：将该String对象与StringBuffer对象sb进行比较。
6. static String copyValueOf(char[] data) ：
7. static String copyValueOf(char[] data, int offset, int count) ：这两个方法将char数组转换成String，与其中一个构造函数类似。
8. boolean endsWith(String suffix) ：该String对象是否以suffix结尾。
    例如：String s1 = new String("abcdefghij");
           String s2 = new String("ghij");
           System.out.println("s1.endsWith(s2): " + s1.endsWith(s2) );
           结果为：s1.endsWith(s2): true
9. boolean equals(Object anObject) ：当anObject不为空并且与当前String对象一样，返回true；否则，返回false。

 3. 未完成工作
 4. 未完成原因
 5. 工作成功
 6. 遇到的问题及解决方法
