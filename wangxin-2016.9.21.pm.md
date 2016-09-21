2016.9.21.pm.工作日志
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
3. 未完成工作
4. 未完成原因
5. 工作成功
6. 遇到的问题及解决方法
