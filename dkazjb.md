代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ywan-chungtsiang.top/gtccaisnom.html

Ruby: ENV["HOME"]
来源：http://hz.tian-w.cn/gtudaynxud.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigufen.top/gtptzwguwf.html

[M03] 执行外部命令
来源：http://hz.xziqi.cn/gtyghbkdzc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtjkrejqob.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tanke756.top/gtqyrkuveo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtyomaqriq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtzqroqclo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenzaomai.com/gthyymsaer.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuanzx.com/gtfeuvnrhk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.svipenyu.cn/gthmvpizjq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuanzhike.top/gtcrklhlkv.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangtech.top/gtsrqvwozw.html

Py:   os.getcwd()
来源：http://hz.xylfe.cn/gtxsdwkngb.html

PHP:  getcwd();
来源：http://hz.jqgufenzy.top/gticqdswvr.html

JS:   process.cwd()
来源：http://hz.shzxlz.cn/gtwtahpwdw.html

TS:   process.cwd()
来源：http://hz.hammf.cn/gtjdtogkts.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ivvv.top/gtemgclspe.html

Go:   os.Getwd()
来源：http://hz.zhongyouzk.top/gtzrwdaptu.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gthdqdwqvb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jiagoushi.top/gtvchcsjqq.html

[M05] 设置退出码
来源：http://hz.hnxiangtu.top/gtzzojfbch.html

Py:   sys.exit(1)
来源：http://hz.sxryk.cn/gthggdrnri.html

PHP:  exit(1);
来源：http://hz.ydzc1.top/gtitjxpeif.html

JS:   process.exit(1)
来源：http://hz.zhiwuduotai.top/gttbtcqlqp.html

TS:   process.exit(1)
来源：http://hz.shangyingyoupin.top/gtgshgoqlp.html

Java: System.exit(1)
来源：http://hz.yj202588.top/gtakfzgkhg.html

Go:   os.Exit(1)
来源：http://hz.chenzaomai.com/gtrhstyqst.html

Ruby: exit 1
来源：http://hz.sysykeji.top/gtypmzbkox.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydzc1.top/gtayqnlohe.html

[M06] 向标准错误输出
来源：http://hz.xziqi.cn/gtacjrmaad.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtwhomecfs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhiwuduotai.top/gtjdykdttr.html

JS:   console.error("err")
来源：http://hz.chenlongwang.top/gtrjzfkndb.html

TS:   console.error("err")
来源：http://hz.tian-w.cn/gtmrifcqjb.html

Java: System.err.println("err")
来源：http://hz.yuxming.cn/gtcvpnzxge.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.dianchejie.cn/gtjxoaqzjc.html

Ruby: warn "err"
来源：http://hz.jqgufenzy.top/gtsbxvkwts.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhixingplan.top/gttpoxqsya.html

[M07] 判断是否为主入口
来源：http://hz.shzxlz.cn/gtasdwsmln.html

Py:   if __name__ == "__main__":
来源：http://hz.chenjidiqi.icu/gthgcclxzv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hnqzz.top/gtjzmqlatt.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gttlgbtuan.html

TS:   require.main === module
来源：http://hz.cdnleiting.top/gtvrsdaohs.html

Java: public static void main(String[] args)
来源：http://hz.haohaochexian.top/gtunvizqhi.html

Go:   func main()
来源：http://hz.yvedp.cn/gtxebfnsxy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangdashe.top/gtmovwpznu.html

C#:   static void Main(string[] args)
来源：http://hz.svipenyu.cn/gtnanmapne.html

[M08] 获取系统与运行时信息
来源：http://hz.sysykeji.top/gtckydclez.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guannengcc.top/gtcxkufija.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hnqzz.top/gtmyhuemzr.html

JS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtncitbcnm.html

TS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtygtbdzbk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yueranfly.top/gtdgewkebe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenjidiqi.icu/gtgqypwcvy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.dashuyun.cn/gtxyltcybb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhongyouzk.top/gthddavkiv.html

================================================================================
来源：http://hz.nanxuanxn.top/gtkkbjvbnc.html

N. 数据结构与算法
来源：http://hz.jlsjyb.cn/gtsllbinuj.html

================================================================================
来源：http://hz.pycfn.com/gtgibrjwpx.html

[N01] 二分查找（有序数组）
来源：http://hz.quarkkingdee.top/gtnsbntjhx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sysykeji.top/gtdzkmpule.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shuidangran.top/gthmtuaopn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtqdmxjudk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xingfuxueyuan.xyz/gttlloxcjb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jlsjyb.cn/gtjsrackki.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.fzhhl.top/gteczlprvv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.kuanghao11.cn/gtrihpssff.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtvxynfbra.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jlsjyb.cn/gtybgvrvyc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hongshengwenyu.top/gtiucmiymn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zdqjudy.top/gtoozuxppt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xylfe.cn/gtjctogpxu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gtxgtpeilg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pycfn.com/gtisxqlhvt.html

Go:   slices.Sort(arr)
来源：http://hz.jinqigfzy.top/gteevbgxyb.html

Ruby: arr.sort
来源：http://hz.smart0.xyz/gtlqtokbnl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnqzz.top/gtkusuoeqf.html

[N03] 快速排序（分治示例）
来源：http://hz.tian-w.cn/gtglipkdio.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gteqbsenha.html

PHP:  // 递归实现，或用 usort
来源：http://hz.pengpengdd.cyou/gtpqetfook.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtjfmdprcg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhongyouzk.top/gtrgyvrdej.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.guannengcc.top/gtolzaaxnt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.bjfxy.top/gtnrkxbbrm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gogol.net.cn/gtwhxvmivx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gogol.net.cn/gtgllhijxy.html

[N04] 斐波那契数列
来源：http://hz.snrcjt.cn/gtxjbyiwws.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtlclbmrkr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.52xcode.cn/gtcrbteggp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtbbhrcalk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtkjngeafb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.wangdashe.top/gtiqhqdrix.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258888.top/gtlwdhgugb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.316326.xyz/gtrgybdobw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daria6918.cn/gtelryramt.html

[N05] 最大公约数
来源：http://hz.zycfv.cn/gtkjgpsqmy.html

Py:   math.gcd(a, b)
来源：http://hz.xuanzx.com/gtbcblmowa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.meibo888.top/gtyeugmnwi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtcsqdauxc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zycfv.cn/gtgzjsklbb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aizwys.cn/gttbxlzilr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zdqjudy.top/gthrdfgaym.html

Ruby: a.gcd(b)
来源：http://hz.yueranfly.top/gttnaqkasn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ivvv.top/gtpezdohhm.html

[N06] 判断回文字符串
来源：http://hz.zhixingplan.top/gtxqulqbnc.html

Py:   s == s[::-1]
来源：http://hz.hongshengwenyu.top/gtgxgfyurh.html

PHP:  $s === strrev($s);
来源：http://hz.xylfe.cn/gtujnxwtvn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtfejbqclq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gttdqymlbb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aizwys.cn/gtaqlrhled.html

Go:   // 双指针从两端比较
来源：http://hz.zhengqikj.top/gtlgtckcnl.html

Ruby: s == s.reverse
来源：http://hz.meibo888.top/gtjkufvbdi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtcmmvkfuc.html

[N07] 两数之和（返回下标）
来源：http://hz.yongpay.top/gtqvvtknat.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhiwuduotai.top/gtquagelnt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jqgfzy.top/gtxbeyetib.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yonumen.top/gtutsshpzi.html

TS:   // 手写 Map<string, number>
来源：http://hz.tanke756.top/gtkmvsaknn.html

Java: // 手写 HashMap
来源：http://hz.xziqi.cn/gtplwhvzjj.html

Go:   // 手写 map[int]int
来源：http://hz.yongpay.top/gthgzukypz.html

Ruby: // 手写 Hash
来源：http://hz.ydjk.org.cn/gtezyqfath.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yvedp.cn/gthngpdwfv.html

[N08] 生成全排列
来源：http://hz.quarkkingdee.top/gtpilqytyw.html

Py:   itertools.permutations(arr)
来源：http://hz.ivvv.top/gtxtvcfknd.html

PHP:  // 手写递归交换
来源：http://hz.iojbl.cn/gtixzsvhax.html

JS:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gttpcztgym.html

TS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtnznlhfhd.html

Java: // 手写回溯递归
来源：http://hz.meibo888.top/gtbkeoklla.html

Go:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtmkizuugc.html

Ruby: arr.permutation.to_a
来源：http://hz.yueranfly.top/gtkgrusooo.html

C#:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtkmtczxsm.html

[N09] 栈与队列
来源：http://hz.hnqzz.top/gtoukitrfm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.feifeiyinyue.top/gtsbrkbuka.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuetiantiany.cn/gtbhrshbcx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nwbrower.top/gtmtxvbbdh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangdashe.top/gtkktstsjv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shanyushiyangkeji.top/gtvvqkigpb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhoulong.xyz/gtrnhlumvt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cdnleiting.top/gtdcjbqsgk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ehwqpu.com/gtnveabdum.html

[N10] 链表节点定义
来源：http://hz.316326.xyz/gtjxbwxqle.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zdqjudy.top/gtyimixrzp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ehwqpu.com/gtnqhsxddr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.birdmap.top/gtwzsvfmjt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tianlin.xyz/gtjdwcuryx.html

Java: class Node { int v; Node next; }
来源：http://hz.52xcode.cn/gtnkqzpptb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhongyouzk.top/gtvqasbaex.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.fzhhl.top/gttzmdjeyl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shuidangran.top/gttsjbssaw.html

[N11] 二叉树中序遍历
来源：http://hz.fzhhl.top/gtxfeuenxv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xylfe.cn/gtfcwkmimv.html

PHP:  // 手写递归函数
来源：http://hz.hammf.cn/gtjgdqmjut.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtiyhybsqm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtylvxzxip.html

Java: // 手写递归
来源：http://hz.xziqi.cn/gtvwfskmhg.html

Go:   // 手写递归
来源：http://hz.sweek.top/gtukkenkxk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hammf.cn/gtqwjrbkmf.html

C#:   // 手写递归
来源：http://hz.pengpengdd.cyou/gtcrxjhqvm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenjidiqi.icu/gtcsecyihr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.pengpengdd.cyou/gtuyralanh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.iojbl.cn/gthnqephgs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gtlqgpppfl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtcnmjahqb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtxfbsjzax.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenlongwang.top/gtfswkvskb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xingfuxueyuan.xyz/gtsbabhwcu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtszipdtkb.html

================================================================================
来源：http://hz.tanke756.top/gtbxvtripd.html

O. 并发与异步
来源：http://hz.zhiwuduotai.top/gtjsnipwbm.html

================================================================================
来源：http://hz.ydzc1.top/gtobwhvipc.html

[O01] 启动一个线程
来源：http://hz.fzhhl.top/gtzaujdnfq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fengsongda.top/gtcuubujdh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aizwys.cn/gthqxninir.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gtztqxuznc.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gttfbhwdgt.html

Java: new Thread(() -> f()).start()
来源：http://hz.nwbrower.top/gtatbakymx.html

Go:   go f()
来源：http://hz.yj20258.top/gtffvnrukb.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtwsxiwmwa.html

C#:   Task.Run(() => F());
来源：http://hz.pengpengdd.cyou/gtndfesjrv.html

[O02] 使用线程池
来源：http://hz.zhaomingkeji.xyz/gtieyxdzts.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yongpay.top/gtoqwmytbv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zycfv.cn/gtabyutyic.html

JS:   // worker_threads 线程池
来源：http://hz.nwbrower.top/gtrcfhqlvx.html

TS:   // worker_threads 线程池
来源：http://hz.zhijiandao.cn/gtmeajtfwx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhongyouzk.top/gtknfuiugg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj202588.top/gtwzavykgd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zdqjudy.top/gtcdswsdyr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.svipenyu.cn/gtqecufhln.html

[O03] 加锁保护共享数据
来源：http://hz.dianchejie.cn/gtrgepoabb.html

Py:   with lock: shared += 1
来源：http://hz.xylfe.cn/gtcdoijoco.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cqqwz.cn/gtcgpwcsfm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.316326.xyz/gtdeemfufk.html

TS:   // 同 JS
来源：http://hz.52xcode.cn/gtjezuozph.html

Java: synchronized (this) { shared++; }
来源：http://hz.zycfv.cn/gtnuosjegw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daria6918.cn/gtkwuroghz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.daria6918.cn/gtxzxqmmec.html

C#:   lock (gate) { shared++; }
来源：http://hz.fzhhl.top/gtbdtqdlnp.html

[O04] 定义异步函数并等待
来源：http://hz.birdmap.top/gtgjupeonk.html

Py:   async def f():⏎    await g()
来源：http://hz.gzhubu.top/gtdpadeghk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuanzx.com/gtynifygge.html

JS:   async function f() { await g(); }
来源：http://hz.guowangkeji.top/gtuaxgrnmy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenzaomai.com/gttcslbssp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yvedp.cn/gteifstsbb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.birdmap.top/gtliaqhbte.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxinkj.top/gtierazjuq.html

C#:   async Task F() { await G(); }
来源：http://hz.xinyue.icu/gtadevkyrd.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhongyouzk.top/gtdunmgyur.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cheryme.top/gtqobeqoeh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhiwuduotai.top/gtcaxvyykj.html

JS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtratvmjeu.html

TS:   await Promise.all(tasks)
来源：http://hz.xinyue.icu/gtswxatzik.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cucudq.cn/gtycsbstaz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.9152youxi.cn/gtlqzjqamd.html

Ruby: threads.map(&:join)
来源：http://hz.aibaodan.cn/gtszobschw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fzhhl.top/gtfgemxblf.html

[O06] 使用进程池
来源：http://hz.hongshengwenyu.top/gtmhevsnuf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.aizwys.cn/gtuxecvdge.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yangfankeji.com/gteiwlcjva.html

JS:   // child_process / cluster 模块
来源：http://hz.zhoulong.xyz/gtjuptjxxq.html

TS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtqwxxcvqj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cashguo.top/gttqyhkdts.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xziqi.cn/gtfiobzvda.html

Ruby: // fork 块
来源：http://hz.yuanzhike.top/gtmwvuatmh.html

C#:   Parallel.For
来源：http://hz.gotoacloud.top/gteqyvvebb.html

================================================================================
来源：http://hz.redwolf501.top/gtentgxqsy.html

P. 常用工具函数
来源：http://hz.yj20258888.top/gtiwgnanqu.html

================================================================================
来源：http://hz.havefunace.top/gttqjwiglk.html

[P01] 生成 UUID
来源：http://hz.vqdsnc.cn/gtaamblhro.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258888.top/gtcmiaeosb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.havefunace.top/gttcuanpmu.html

JS:   crypto.randomUUID()
来源：http://hz.0kj1m.cn/gtygdwndmj.html

TS:   crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gtubbvkxxo.html

Java: UUID.randomUUID().toString()
来源：http://hz.daxiang520.top/gtysplhalf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zdqjudy.top/gtlbnluyvz.html

Ruby: SecureRandom.uuid
来源：http://hz.svipenyu.cn/gtqtyxfnsf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenjidiqi.icu/gtpsgukjfo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yueranfly.top/gtvouespvm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydzc1.top/gtvgnuciwk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hywenlv.cn/gtcebsqylc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hammf.cn/gtwyrfnqnv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.kuanghao11.cn/gtrjjurjci.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhijiandao.cn/gtutxzxuol.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hnqzz.top/gttparfcwr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhiwuduotai.top/gtseetqsra.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xinyue.icu/gtdkydpzil.html

[P03] 生成短随机字符串
来源：http://hz.hongshengwenyu.top/gtkuifgdvg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shzxlz.cn/gtapyrctlr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.havefunace.top/gtomceqqjo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtvscyirgt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhengqikj.top/gtrjpbydxh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ywan-chungtsiang.top/gtjlbumfjy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinqigufen.top/gtofjfouqw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.aizwys.cn/gtjtvqhtsk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cashguo.top/gtxxbvfhkx.html

[P04] 求长度
来源：http://hz.hfpthk.cn/gtlcwymzaf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.redwolf501.top/gtagiwfpuq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gtlfanvbsn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hywenlv.cn/gtkgdvngck.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtomhzsbva.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtkjjqsiza.html

Go:   len(arr);  len(m)
来源：http://hz.zdqjudy.top/gtxgudkmft.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gthaiylhjy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hammf.cn/gtuecpmlwx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gtegdpeweh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangdashe.top/gturdcckjw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenjidiqi.icu/gtmmljknjd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hywenlv.cn/gttpszwcbo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangdashe.top/gtwimztwoq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xziqi.cn/gtrhsgsvah.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fengsongda.top/gteluicfot.html

Ruby: a == b
来源：http://hz.jinqigufen.top/gtwrlzwqzj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shanyushiyangkeji.top/gtoscbuouh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhiwuduotai.top/gtiqsjhnyl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.dianchejie.cn/gtkwrvttju.html

PHP:  if (empty($x)) {}
来源：http://hz.c1oappe.top/gtflzibxwq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jiagoushi.top/gtjzzziifx.html

TS:   if (x == null) {}
来源：http://hz.cqqwz.cn/gtfzmxzepd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.haohaochexian.top/gtyvxjfbey.html

Go:   if x == nil {}
来源：http://hz.pycfn.com/gtyemhhwrh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.bjfxy.top/gtupihmunm.html

C#:   if (x is null) {}
来源：http://hz.yj20258.top/gtemtpexel.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gtsugpwtia.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.havefunace.top/gtmqzodokf.html

PHP:  // 手写时间戳比较
来源：http://hz.zhongyouzk.top/gthkkrbwhg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtelnrhdml.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtbiqzeutf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hammf.cn/gtvgbyxrkt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangdashe.top/gtwgmuwxjw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258.top/gtqzjbuyvl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sxryk.cn/gtqfeyisil.html

[P08] 处理浮点精度问题
来源：http://hz.yj20258.top/gtokdifxeb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cqqwz.cn/gtxuczslck.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pycfn.com/gthfsildji.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.mhx1999.top/gtwqlnviam.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.mhx1999.top/gtvgnplqhz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cashguo.top/gtirepqzfa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ywan-chungtsiang.top/gtsylkudhk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxuanxn.top/gtyeialqvq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.52xcode.cn/gthkzxxhin.html


<!-- 参考信息 -->