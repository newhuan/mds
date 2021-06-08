1. 获取pid
    ps -ef | grep java => pid
   或
    top | grep java => pid

2. 获取线程id

   top -Hp $pid => PID => threadId

 3. 计算线程id的16进制：

    printf "%x\n" $threadId => 得到16进制数 => $ex

4. jstack获取线程堆栈信息：

   jstack $pid | grep -20 $ex

