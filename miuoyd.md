代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xinyue.icu/gtkzrjoeql.html

Ruby: ENV["HOME"]
来源：http://hz.shuidangran.top/gtjynpyfth.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gtljfwnqzx.html

[M03] 执行外部命令
来源：http://hz.svipenyu.cn/gtrfiuuhwq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pycfn.com/gtglgwpcic.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shzxlz.cn/gtdnxealui.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gtmzvgjigv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gtoewuubil.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnqzz.top/gtrxrednmb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gtigyizjat.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.pengpengdd.cyou/gtqpvmjkui.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shuidangran.top/gtveakctjf.html

[M04] 获取当前工作目录
来源：http://hz.tianlin.xyz/gtcourbkbj.html

Py:   os.getcwd()
来源：http://hz.shangyingyoupin.top/gtjckltasc.html

PHP:  getcwd();
来源：http://hz.sweek.top/gtoqgtehtr.html

JS:   process.cwd()
来源：http://hz.xuanzx.com/gttxqtolsf.html

TS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtldixojnx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.kuanghao11.cn/gtgyklgqvv.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtzwlrqfdt.html

Ruby: Dir.pwd
来源：http://hz.cdnleiting.top/gtsrjflzbg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hongshengwenyu.top/gtvcnrbzal.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtfozlnenx.html

Py:   sys.exit(1)
来源：http://hz.gogol.net.cn/gtnyxbmbjn.html

PHP:  exit(1);
来源：http://hz.xylfe.cn/gtjhnsvmsg.html

JS:   process.exit(1)
来源：http://hz.chenjidiqi.icu/gtsvwmwtbj.html

TS:   process.exit(1)
来源：http://hz.guowangkeji.top/gtkgattljs.html

Java: System.exit(1)
来源：http://hz.hfpthk.cn/gtbgbiienl.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtypqldloo.html

Ruby: exit 1
来源：http://hz.jinyuanbaomall.cn/gtbmvisflg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinghuilouyu.cn/gtdhbkftio.html

[M06] 向标准错误输出
来源：http://hz.quarkkingdee.top/gtyseyatwo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gtfeyvqzhn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yangfankeji.com/gtysoybvzh.html

JS:   console.error("err")
来源：http://hz.aibaodan.cn/gtfentcwbt.html

TS:   console.error("err")
来源：http://hz.zhixingplan.top/gttuzpxnxc.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtfisnhlnb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gthqeokgrp.html

Ruby: warn "err"
来源：http://hz.zhaomingkeji.xyz/gtxsutfdha.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aibaodan.cn/gtjwwtzepq.html

[M07] 判断是否为主入口
来源：http://hz.zhiwuduotai.top/gtweducfff.html

Py:   if __name__ == "__main__":
来源：http://hz.chenjidiqi.icu/gtsqhhlorx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.316326.xyz/gtdwlfkjdp.html

JS:   require.main === module
来源：http://hz.hnxiangtu.top/gtvzqtrsav.html

TS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtxwemtwss.html

Java: public static void main(String[] args)
来源：http://hz.guowangkeji.top/gtlreormax.html

Go:   func main()
来源：http://hz.daxiang520.top/gttzhithfa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tianlin.xyz/gtzzcqqvhk.html

C#:   static void Main(string[] args)
来源：http://hz.ydzc1.top/gtwdbeegvx.html

[M08] 获取系统与运行时信息
来源：http://hz.shanyushiyangkeji.top/gtppnsyviv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydjk.org.cn/gtdiinnjjn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinqigufen.top/gtuemvijah.html

JS:   process.platform;  process.version
来源：http://hz.yonumen.top/gtpdpijubc.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtqxbiypiu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nwbrower.top/gthrrlgrou.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guowangkeji.top/gtvxkvlqrg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hfpthk.cn/gtksublfgk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.bjfxy.top/gtcyenjkrj.html

================================================================================
来源：http://hz.jqgfzy.top/gtzmxrnznr.html

N. 数据结构与算法
来源：http://hz.sysykeji.top/gtmnyaqxpx.html

================================================================================
来源：http://hz.ehwqpu.com/gtcnypzezv.html

[N01] 二分查找（有序数组）
来源：http://hz.guowangkeji.top/gtulvgsavk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xziqi.cn/gtqegpoxfn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.meibo888.top/gtbmxqnzft.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtrgmseckb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jlsjyb.cn/gtqdmfuwhc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtrutfjhdf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gtovoenvfy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj202588.top/gtpnwctiky.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.52xcode.cn/gtmqkgtyer.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gaohongyu789.top/gttpvssswk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtqhsbcvmy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tian-w.cn/gtklwncjhe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtyunzyoje.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tian-w.cn/gtdmlwhlqh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dianchejie.cn/gtkccwyxdq.html

Go:   slices.Sort(arr)
来源：http://hz.52xcode.cn/gteiounvts.html

Ruby: arr.sort
来源：http://hz.zhongyouzk.top/gtppgsgnwb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hfpthk.cn/gtpnuwwgny.html

[N03] 快速排序（分治示例）
来源：http://hz.pengpengdd.cyou/gtzgxqltig.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jqgufenzy.top/gtkpzvoege.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhongyouzk.top/gtbinmzdqs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jlsjyb.cn/gtwfkhkvbi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gtwsbxqbvj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhoulong.xyz/gtddcryyad.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jyoumei.cn/gtmmjmjzjf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinyuanbaomall.cn/gteomynkqq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cdnleiting.top/gtjhqwonoj.html

[N04] 斐波那契数列
来源：http://hz.ywan-chungtsiang.top/gtwekbwjbj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sufxvd.cn/gtjlxfqppj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.316326.xyz/gtrkbqgspk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtepmxldkt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtoxdjitlh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.guannengcc.top/gtybcwypow.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yanxiufei.cn/gtrwzahzcc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.dianchejie.cn/gtbfjiygse.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtmrzwefxk.html

[N05] 最大公约数
来源：http://hz.c1oappe.top/gtfdplabev.html

Py:   math.gcd(a, b)
来源：http://hz.yueranfly.top/gtugjsihhf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jyoumei.cn/gtqwjivnqi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sweek.top/gtypmzykwv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtwwwnlgqi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydjk.org.cn/gtspfsydvk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.9152youxi.cn/gtsahuofkx.html

Ruby: a.gcd(b)
来源：http://hz.tianlin.xyz/gtgsutgscv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj202588.top/gtrmnuzeai.html

[N06] 判断回文字符串
来源：http://hz.redwolf501.top/gtvnufazbd.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtbqchvrwr.html

PHP:  $s === strrev($s);
来源：http://hz.mhx1999.top/gtqozrwbvq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtvbrrxgxe.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtyxmwmtum.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhijiandao.cn/gtcowkjwhe.html

Go:   // 双指针从两端比较
来源：http://hz.ivvv.top/gtrnnapepu.html

Ruby: s == s.reverse
来源：http://hz.316326.xyz/gtotpvkrpn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtvoqajfeu.html

[N07] 两数之和（返回下标）
来源：http://hz.havefunace.top/gtsbhlfyik.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.redwolf501.top/gtxfvxbnwr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.redwolf501.top/gtwbkdfbso.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuanzx.com/gtnztrtvpo.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258888.top/gtsruywprr.html

Java: // 手写 HashMap
来源：http://hz.jinghuilouyu.cn/gtobwrjgxb.html

Go:   // 手写 map[int]int
来源：http://hz.guannengcc.top/gtjegxxheo.html

Ruby: // 手写 Hash
来源：http://hz.cucudq.cn/gtfgmlosbo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.smart0.xyz/gtkmeobdqj.html

[N08] 生成全排列
来源：http://hz.yanxiufei.cn/gtygvoozve.html

Py:   itertools.permutations(arr)
来源：http://hz.hnxiangtu.top/gtfcscrwui.html

PHP:  // 手写递归交换
来源：http://hz.yj20258888.top/gtfvtjujro.html

JS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtyalaiuao.html

TS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtzxocvetn.html

Java: // 手写回溯递归
来源：http://hz.jyoumei.cn/gtedywggag.html

Go:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtcipvellm.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxuanxn.top/gtdmgywtse.html

C#:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtefwvjaau.html

[N09] 栈与队列
来源：http://hz.zdqjudy.top/gtimljnnqq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhengqikj.top/gtrklprmnl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shzxlz.cn/gttzgraetg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.fzhhl.top/gtxfalbvpr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangshuangyany.cn/gtlzuikelk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhixingplan.top/gtwakngdxy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tianlin.xyz/gthkizsfzt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cheryme.top/gtpbpdgkgj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ydzc1.top/gtqtxixeed.html

[N10] 链表节点定义
来源：http://hz.yvedp.cn/gtkqrgkina.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fzhhl.top/gtmgfhalgz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nwbrower.top/gtqyzqrtec.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sysykeji.top/gtahbclyme.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhiwuduotai.top/gttbyzxnjf.html

Java: class Node { int v; Node next; }
来源：http://hz.cdnleiting.top/gtriyczewx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.wangshuangyany.cn/gtcpxsbbmx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.daria6918.cn/gtagvbdxlf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hammf.cn/gtmgbrycfl.html

[N11] 二叉树中序遍历
来源：http://hz.jqgufenzy.top/gtfauhfdlh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtzyffbnhw.html

PHP:  // 手写递归函数
来源：http://hz.zhengqikj.top/gttbwsixlr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtloynlbhg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.c1oappe.top/gtjdhcdxtf.html

Java: // 手写递归
来源：http://hz.tanke756.top/gtcsdsiinb.html

Go:   // 手写递归
来源：http://hz.hongshengwenyu.top/gttfwklmie.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ehwqpu.com/gtffujpzzn.html

C#:   // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtzxwapeba.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cqqwz.cn/gtugxurdae.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tanke756.top/gtdnqzeira.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cashguo.top/gtscbcbwzh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuanzhike.top/gtuzoqpkqb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hfpthk.cn/gttlawfwhv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.c1oappe.top/gtefdnlqgy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dianchejie.cn/gtuayzcjzo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.0kj1m.cn/gtfbplogyt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtglwdpyia.html

================================================================================
来源：http://hz.jianghu66.top/gtyhmadasf.html

O. 并发与异步
来源：http://hz.daria6918.cn/gtcndrkleo.html

================================================================================
来源：http://hz.chenlongwang.top/gthlffndpw.html

[O01] 启动一个线程
来源：http://hz.xuetiantiany.cn/gtiiiphhke.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sysykeji.top/gtdiriypiq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.pengpengdd.cyou/gtjappjkrt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.feifeiyinyue.top/gtllcavppd.html

TS:   // 同 JS
来源：http://hz.birdmap.top/gtsconadhq.html

Java: new Thread(() -> f()).start()
来源：http://hz.quarkkingdee.top/gtttsukhfd.html

Go:   go f()
来源：http://hz.aizwys.cn/gtnmoqnbbu.html

Ruby: Thread.new { f }
来源：http://hz.jinqigufen.top/gtpdwmgggu.html

C#:   Task.Run(() => F());
来源：http://hz.gaohongyu789.top/gtvkeethux.html

[O02] 使用线程池
来源：http://hz.316326.xyz/gtflllfktk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.svipenyu.cn/gtahwxrjwb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.c1oappe.top/gtzfxunikc.html

JS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtqwmswzwc.html

TS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtchnrdpso.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.c1oappe.top/gtaqiesxsc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shzxlz.cn/gtokckiwkx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuanzhike.top/gtxfbcrsfl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yanxiufei.cn/gtpxsjrzzl.html

[O03] 加锁保护共享数据
来源：http://hz.zhiwuduotai.top/gtdvmpproc.html

Py:   with lock: shared += 1
来源：http://hz.guowangkeji.top/gttlqufsyx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cashguo.top/gtcjyhvzcn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinghuilouyu.cn/gtbmnctwnd.html

TS:   // 同 JS
来源：http://hz.yj20258.top/gtpvztvdev.html

Java: synchronized (this) { shared++; }
来源：http://hz.jiagoushi.top/gtdecdlops.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuanzhike.top/gtsswqtakf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hywenlv.cn/gtvqhjcyry.html

C#:   lock (gate) { shared++; }
来源：http://hz.feifeiyinyue.top/gtvighbofk.html

[O04] 定义异步函数并等待
来源：http://hz.feifeiyinyue.top/gtvteaoeqt.html

Py:   async def f():⏎    await g()
来源：http://hz.yj20258888.top/gtkpankjxl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cucudq.cn/gtsudbixdc.html

JS:   async function f() { await g(); }
来源：http://hz.tanke756.top/gtkczywxgt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhiwuduotai.top/gtmzapeqnf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cucudq.cn/gtkbxmbhuv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yanxiufei.cn/gtfxhkuned.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.bjfxy.top/gtjefbenfk.html

C#:   async Task F() { await G(); }
来源：http://hz.9152youxi.cn/gtvcrxfgwd.html

[O05] 并发执行并等待全部完成
来源：http://hz.dianchejie.cn/gtsbgzgogh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.svipenyu.cn/gtxfnwvlxs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.mhx1999.top/gtnvjzxzzh.html

JS:   await Promise.all(tasks)
来源：http://hz.smart0.xyz/gtlqnuihfv.html

TS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtzninhqtb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cqqwz.cn/gtubumltze.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jqgfzy.top/gtmhoolull.html

Ruby: threads.map(&:join)
来源：http://hz.zhiwuduotai.top/gtskacokmm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuxming.cn/gtzdjpdzwq.html

[O06] 使用进程池
来源：http://hz.svipenyu.cn/gtspfsacnj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.316326.xyz/gtvxbhtfih.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yueranfly.top/gtsajjeykc.html

JS:   // child_process / cluster 模块
来源：http://hz.haohaochexian.top/gtcqwysqqk.html

TS:   // child_process / cluster 模块
来源：http://hz.yj202588.top/gtvmzoeiuk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenlongwang.top/gtvwrddzpm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenlongwang.top/gtksaqdosq.html

Ruby: // fork 块
来源：http://hz.tianlin.xyz/gtifuqotyu.html

C#:   Parallel.For
来源：http://hz.redwolf501.top/gtwsuiimgl.html

================================================================================
来源：http://hz.redwolf501.top/gtxfcbcuof.html

P. 常用工具函数
来源：http://hz.yanxiufei.cn/gtuudkohjp.html

================================================================================
来源：http://hz.nanxuanxn.top/gtcfbohkfx.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtqlnxtfuh.html

Py:   str(uuid.uuid4())
来源：http://hz.bjfxy.top/gtpdtvadcl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.redwolf501.top/gtkvjnqnbe.html

JS:   crypto.randomUUID()
来源：http://hz.yuanzhike.top/gtmeskwprc.html

TS:   crypto.randomUUID()
来源：http://hz.nanxuanxn.top/gtradsjdkv.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuxming.cn/gthxxfiuxu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.havefunace.top/gtjuttpqhq.html

Ruby: SecureRandom.uuid
来源：http://hz.pengpengdd.cyou/gtlgfuychh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xziqi.cn/gtzveyetup.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yuanzhike.top/gtnuwhblyl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shuidangran.top/gtbvxbhgvh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gteunmioal.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenjidiqi.icu/gtqwlskhwe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sweek.top/gtorqvaozn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jianghu66.top/gtqqrhyrtt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cqqwz.cn/gteiyfpdvh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigufen.top/gtyockdwuj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jqgfzy.top/gtfgzjuhzo.html

[P03] 生成短随机字符串
来源：http://hz.gzhubu.top/gtcqllrewe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nwbrower.top/gtbqudfdyj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zdqjudy.top/gtfmkalnio.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtibcitsmw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtpcggbols.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jqgufenzy.top/gtbxkcomkt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.quarkkingdee.top/gtpqtrevxg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgfzy.top/gtkdolouwn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuanzx.com/gtklhjeukv.html

[P04] 求长度
来源：http://hz.meibo888.top/gtmrbgjuyy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tian-w.cn/gtzistkeez.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gthehyolks.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtkpptgkpn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gtznazdogu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.haohaochexian.top/gthoryfilg.html

Go:   len(arr);  len(m)
来源：http://hz.jyoumei.cn/gtvrrprpai.html

Ruby: x.length;  x.size
来源：http://hz.ivvv.top/gtdawrrlos.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sysykeji.top/gtqhyyniky.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ppjwa.cn/gtkooeazaw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sweek.top/gtvekasvwq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuetiantiany.cn/gtprjhlnts.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pycfn.com/gtxcysmisg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tian-w.cn/gtacrgdqsv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hammf.cn/gtehqwlste.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hammf.cn/gtwlkgwiiv.html

Ruby: a == b
来源：http://hz.havefunace.top/gtthmychqm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.fzhhl.top/gthxlpbfpq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yueranfly.top/gtddwdnizu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xylfe.cn/gtuspwphml.html

PHP:  if (empty($x)) {}
来源：http://hz.xylfe.cn/gtuitfnrqf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tian-w.cn/gtzptvvdke.html

TS:   if (x == null) {}
来源：http://hz.cqqwz.cn/gtwalcvyrs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhengqikj.top/gtilthtaet.html

Go:   if x == nil {}
来源：http://hz.kuanghao11.cn/gtroeqoyxg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.redwolf501.top/gtlxtvmqyn.html

C#:   if (x is null) {}
来源：http://hz.smart0.xyz/gtttdatevt.html

[P07] 防抖与节流
来源：http://hz.dianchejie.cn/gthqygjhwo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.tanke756.top/gtvwcsdsie.html

PHP:  // 手写时间戳比较
来源：http://hz.vqdsnc.cn/gtfitowuce.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtaqypthmo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtvehdrvkp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgfzy.top/gtcoldtmvr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangkeji.top/gtixiwbfgo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zycfv.cn/gtfmaehljf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.smart0.xyz/gtmungdynm.html

[P08] 处理浮点精度问题
来源：http://hz.jqgfzy.top/gtugqjmdgk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hammf.cn/gtvhtsidbf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zycfv.cn/gtgrqmxvrq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sufxvd.cn/gtrikggnph.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hammf.cn/gttahcrwgz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj20258888.top/gthxyyppga.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ybcxt.top/gtfsbpezta.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shuidangran.top/gtrtgwkilj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.kuanghao11.cn/gtluslkrec.html


<!-- 参考信息 -->