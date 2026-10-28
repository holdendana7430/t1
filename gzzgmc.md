代发 wailian999

================================================================================
来源：http://hz.cheryme.top/gtcqtgxeqa.html

[M01] 读取命令行参数
来源：http://hz.yanxiufei.cn/gthpwrfwpa.html

Py:   sys.argv[1:]
来源：http://hz.nwbrower.top/gtfgrhvuxg.html

PHP:  $argv;  $argc;
来源：http://hz.xylfe.cn/gtqkcmdwac.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtymyncwmg.html

TS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtnjzrykhc.html

Java: args 数组（main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gtjlqfymuc.html

Go:   os.Args[1:]
来源：http://hz.aizwys.cn/gtjknxwtkk.html

Ruby: ARGV
来源：http://hz.xylfe.cn/gtnodptxpx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtvntmalhf.html

[M02] 读取环境变量
来源：http://hz.pengpengdd.cyou/gtphouzpcy.html

Py:   os.environ.get("HOME")
来源：http://hz.hammf.cn/gtylvwqtqe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daxiang520.top/gtcwsiplcs.html

JS:   process.env.HOME
来源：http://hz.daria6918.cn/gtzwbcysgq.html

TS:   process.env.HOME
来源：http://hz.yuanzhike.top/gtyhhphiqn.html

Java: System.getenv("HOME")
来源：http://hz.cucudq.cn/gtjjbjxckv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtufukaqef.html

Ruby: ENV["HOME"]
来源：http://hz.smart0.xyz/gtoazycpqj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guannengcc.top/gtvhjidfcz.html

[M03] 执行外部命令
来源：http://hz.zhongyouzk.top/gtpkrnqpdv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhongyouzk.top/gtwgpqrpif.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhiwuduotai.top/gtwfrrdpfe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.fengsongda.top/gtfueipqqx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtwjumkleo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cheryme.top/gtgvwgtgyt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aibaodan.cn/gtrnfbxzkp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.mhx1999.top/gtsysnjstk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtwojirwsb.html

[M04] 获取当前工作目录
来源：http://hz.0kj1m.cn/gturvsslel.html

Py:   os.getcwd()
来源：http://hz.yonumen.top/gttdpqrkbm.html

PHP:  getcwd();
来源：http://hz.xziqi.cn/gtwqqyjnuc.html

JS:   process.cwd()
来源：http://hz.xingfuxueyuan.xyz/gtcqyyghhi.html

TS:   process.cwd()
来源：http://hz.jyoumei.cn/gtihlsccjv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgfzy.top/gtbiifcfbe.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtbxjcfxfk.html

Ruby: Dir.pwd
来源：http://hz.dashuyun.cn/gtbpladeoi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.dashuyun.cn/gtdgcwrvnc.html

[M05] 设置退出码
来源：http://hz.jinqigfzy.top/gtsycqtnjt.html

Py:   sys.exit(1)
来源：http://hz.yj202588.top/gtunuzhwld.html

PHP:  exit(1);
来源：http://hz.gaohongyu789.top/gtwjslxtkz.html

JS:   process.exit(1)
来源：http://hz.aizwys.cn/gtkuxlmopm.html

TS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtkkewbase.html

Java: System.exit(1)
来源：http://hz.tianlin.xyz/gtpixqbfco.html

Go:   os.Exit(1)
来源：http://hz.zhongyouzk.top/gtmlwznpcu.html

Ruby: exit 1
来源：http://hz.gzhubu.top/gtmhdpjdib.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shzxlz.cn/gtmotytktx.html

[M06] 向标准错误输出
来源：http://hz.ivvv.top/gtfjdurnpc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhiwuduotai.top/gtrxnabfso.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinghuilouyu.cn/gtvitlszgj.html

JS:   console.error("err")
来源：http://hz.redwolf501.top/gtxfrcvrcd.html

TS:   console.error("err")
来源：http://hz.hywenlv.cn/gtwqjwdtoh.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtkbjliswj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xylfe.cn/gtzuixkobi.html

Ruby: warn "err"
来源：http://hz.yuxming.cn/gtwndfviah.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ivvv.top/gtfrhdrbqt.html

[M07] 判断是否为主入口
来源：http://hz.zhixingplan.top/gtjsmqabqo.html

Py:   if __name__ == "__main__":
来源：http://hz.aizwys.cn/gtfbeyqyaw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xuetiantiany.cn/gtodkxbysp.html

JS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gttqkknbch.html

TS:   require.main === module
来源：http://hz.gotoacloud.top/gtipplnyxf.html

Java: public static void main(String[] args)
来源：http://hz.redwolf501.top/gtizxseeta.html

Go:   func main()
来源：http://hz.tian-w.cn/gtmfgiqvaa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.0kj1m.cn/gtsgqzmatl.html

C#:   static void Main(string[] args)
来源：http://hz.zhixingplan.top/gtbzckhuly.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gtxvmjwmvl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnqzz.top/gtqkcguigc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ehwqpu.com/gtzxbnfspl.html

JS:   process.platform;  process.version
来源：http://hz.ywan-chungtsiang.top/gtwicrfjnn.html

TS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtsrfhjkbt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ydzc1.top/gtozwysoer.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuanzx.com/gtkhsssbkw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuanzx.com/gtbijnaxue.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tanke756.top/gtsolhygik.html

================================================================================
来源：http://hz.cashguo.top/gtarsfqsxl.html

N. 数据结构与算法
来源：http://hz.feifeiyinyue.top/gthvqwhmdt.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtxxhawhaf.html

[N01] 二分查找（有序数组）
来源：http://hz.ywan-chungtsiang.top/gtignedlfj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.c1oappe.top/gtaahkfpju.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hammf.cn/gtistzpzuq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtmixcxvfy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangkeji.top/gtjsxkzfex.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtdufktuhz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.fengsongda.top/gtlqjorpyr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangdashe.top/gtgoyeukls.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sweek.top/gtqtddkivq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.haohaochexian.top/gtuowifrpz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ivvv.top/gtcoqlbyyr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ydjk.org.cn/gtweneuccj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtryejiwks.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gaohongyu789.top/gtywobnxrf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.kuanghao11.cn/gturezgmdn.html

Go:   slices.Sort(arr)
来源：http://hz.bjfxy.top/gtcobevghu.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtcawqcoop.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydjk.org.cn/gtcpbfwzac.html

[N03] 快速排序（分治示例）
来源：http://hz.xziqi.cn/gtnnpygxwq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinghuilouyu.cn/gtvkcvvzkf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinyuanbaomall.cn/gtxinwjvve.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhiwuduotai.top/gtbsifawir.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtorcoxire.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenzaomai.com/gtuajfbsua.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zycfv.cn/gtkyqrxdxs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangkeji.top/gtseecrqzj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ehwqpu.com/gtksjoycjw.html

[N04] 斐波那契数列
来源：http://hz.ehwqpu.com/gttenyfgnx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtislzflqf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.havefunace.top/gtyxwwgnit.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtbqbbfrbi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtucadrwqo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ywan-chungtsiang.top/gtkphwfumm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hongshengwenyu.top/gtojthnezq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangtech.top/gtynulfbhd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.snrcjt.cn/gtdbcdynmx.html

[N05] 最大公约数
来源：http://hz.shangyingyoupin.top/gtvqzyphfh.html

Py:   math.gcd(a, b)
来源：http://hz.9152youxi.cn/gtncnkiptm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zdqjudy.top/gtcvhhjrxb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gtepuoqvrw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yangfankeji.com/gtrzeolygh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pengpengdd.cyou/gtkdkdrdul.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.mhx1999.top/gtojnqdpnb.html

Ruby: a.gcd(b)
来源：http://hz.dashuyun.cn/gtqezwhrjq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xziqi.cn/gtewpefnme.html

[N06] 判断回文字符串
来源：http://hz.xylfe.cn/gtmdznsqtr.html

Py:   s == s[::-1]
来源：http://hz.shanyushiyangkeji.top/gtenvpgfdm.html

PHP:  $s === strrev($s);
来源：http://hz.52xcode.cn/gttpxoomvt.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtbknwmvkj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtcifwkyqx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zycfv.cn/gthokiuqgj.html

Go:   // 双指针从两端比较
来源：http://hz.gotoacloud.top/gtsaliiewk.html

Ruby: s == s.reverse
来源：http://hz.cashguo.top/gtxljmwnhd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jiagoushi.top/gtcwtqbcke.html

[N07] 两数之和（返回下标）
来源：http://hz.yvedp.cn/gtkrdxnqen.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gotoacloud.top/gtplrmruwu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sxryk.cn/gtbxixqqhm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tianlin.xyz/gtgnvhsisd.html

TS:   // 手写 Map<string, number>
来源：http://hz.cucudq.cn/gtnupkodxq.html

Java: // 手写 HashMap
来源：http://hz.tianlin.xyz/gtxdnycapk.html

Go:   // 手写 map[int]int
来源：http://hz.yuxming.cn/gtbtcaeyxv.html

Ruby: // 手写 Hash
来源：http://hz.cdnleiting.top/gtqqsmftfq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xuanzx.com/gtyeskmyol.html

[N08] 生成全排列
来源：http://hz.wangshuangyany.cn/gtmgkdtixw.html

Py:   itertools.permutations(arr)
来源：http://hz.feifeiyinyue.top/gtxaertxnb.html

PHP:  // 手写递归交换
来源：http://hz.daxiang520.top/gtvtnfkdsd.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtrnvmkhss.html

TS:   // 手写回溯递归
来源：http://hz.birdmap.top/gtbdpzyrrl.html

Java: // 手写回溯递归
来源：http://hz.sysykeji.top/gtmhbcuiev.html

Go:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtqyvpkoiz.html

Ruby: arr.permutation.to_a
来源：http://hz.chenjidiqi.icu/gthihlpdiz.html

C#:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtyxydoaar.html

[N09] 栈与队列
来源：http://hz.aibaodan.cn/gtyatnmrzs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gotoacloud.top/gtlhzaaooj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.meibo888.top/gtmhoesdlf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ivvv.top/gtwygnfltg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258888.top/gtslaasfss.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhijiandao.cn/gtlquabtxn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yuanzhike.top/gtnuwdeaus.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ybcxt.top/gtgexxfuph.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jiagoushi.top/gtaweboesn.html

[N10] 链表节点定义
来源：http://hz.hnxiangtu.top/gtskoralpg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhoulong.xyz/gtpxbnypfd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jqgufenzy.top/gtajwmktke.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gtftzxbung.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hongshengwenyu.top/gthdmuojmx.html

Java: class Node { int v; Node next; }
来源：http://hz.316326.xyz/gtblhmmavf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gzhubu.top/gtptznfrva.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yangfankeji.com/gtmhtipmih.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ydzc1.top/gtyrocksqz.html

[N11] 二叉树中序遍历
来源：http://hz.zhijiandao.cn/gtjunengpz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.52xcode.cn/gtpokgrrcw.html

PHP:  // 手写递归函数
来源：http://hz.tian-w.cn/gtajxjjowg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtlmrxemzm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtjmsozuye.html

Java: // 手写递归
来源：http://hz.xylfe.cn/gtoxjlkkpk.html

Go:   // 手写递归
来源：http://hz.xinyue.icu/gtvdhdnnkx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hnxiangtu.top/gteuhsqxll.html

C#:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtfwiwpakx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.kuanghao11.cn/gtgvvbmqow.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenlongwang.top/gtdzcshtif.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj20258888.top/gtixlkwyxq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ivvv.top/gtrvxijttw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gttpwgxtcm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtaqcutrcl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.quarkkingdee.top/gtcgtegwwy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.andypj.xyz/gtwqtjlswn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gtdpsesynt.html

================================================================================
来源：http://hz.tian-w.cn/gtmuqjpbhr.html

O. 并发与异步
来源：http://hz.hfpthk.cn/gtvcognedc.html

================================================================================
来源：http://hz.snrcjt.cn/gturgdvlto.html

[O01] 启动一个线程
来源：http://hz.yj20258888.top/gthfpwwjki.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sweek.top/gtsvargjej.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuetiantiany.cn/gthdsgojhn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtagimxwzm.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtfzxqpwto.html

Java: new Thread(() -> f()).start()
来源：http://hz.redwolf501.top/gtdmhikmiq.html

Go:   go f()
来源：http://hz.jiagoushi.top/gtkhxdimar.html

Ruby: Thread.new { f }
来源：http://hz.daria6918.cn/gtxfyrrwtu.html

C#:   Task.Run(() => F());
来源：http://hz.cucudq.cn/gtrppkemvi.html

[O02] 使用线程池
来源：http://hz.ppjwa.cn/gtppmjefgf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ivvv.top/gtioiwxkiv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hammf.cn/gtvnfpybbj.html

JS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtmnaybaoc.html

TS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtmvhsylxw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yueranfly.top/gtbjusmtha.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cdnleiting.top/gtnikkbmid.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuanzhike.top/gtojeljwrg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tian-w.cn/gtvfvytbur.html

[O03] 加锁保护共享数据
来源：http://hz.jinyuanbaomall.cn/gtugawtcpv.html

Py:   with lock: shared += 1
来源：http://hz.xingfuxueyuan.xyz/gtmsncseof.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shuidangran.top/gtucvryeuj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhoulong.xyz/gtkchwqmqy.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtrjuaggrj.html

Java: synchronized (this) { shared++; }
来源：http://hz.yonumen.top/gttgjmvjpu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhiwuduotai.top/gthymmoqgc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shuidangran.top/gtubukxyku.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuetiantiany.cn/gtmhfuzoqc.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangtech.top/gtzajlgqax.html

Py:   async def f():⏎    await g()
来源：http://hz.fzhhl.top/gtyqqijvlf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xylfe.cn/gtzltdglhp.html

JS:   async function f() { await g(); }
来源：http://hz.yanxiufei.cn/gtcoiarssm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.fengsongda.top/gtabpvynnv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinqigufen.top/gtqwxssjqm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jqgufenzy.top/gtdcstkylj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhongyouzk.top/gtqqwscdtb.html

C#:   async Task F() { await G(); }
来源：http://hz.ppjwa.cn/gtvqrrqxyn.html

[O05] 并发执行并等待全部完成
来源：http://hz.hysaishi.cn/gtjflhhljf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuanzhike.top/gtdutsyrhb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.andypj.xyz/gtvdssgjgx.html

JS:   await Promise.all(tasks)
来源：http://hz.hnqzz.top/gtcyrswxkp.html

TS:   await Promise.all(tasks)
来源：http://hz.jinqigufen.top/gthtoazqid.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gaohongyu789.top/gtzpzgfytr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.bjfxy.top/gtistcjrdk.html

Ruby: threads.map(&:join)
来源：http://hz.chenlongwang.top/gtrtektelu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jqgfzy.top/gtxnvykatp.html

[O06] 使用进程池
来源：http://hz.chenlongwang.top/gtwnckvahu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.svipenyu.cn/gtnzokszty.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jqgfzy.top/gtjjabhrcf.html

JS:   // child_process / cluster 模块
来源：http://hz.xziqi.cn/gtrdvllwqv.html

TS:   // child_process / cluster 模块
来源：http://hz.sweek.top/gtixhxfsjm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ivvv.top/gtqlkwfbeh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zdqjudy.top/gtqusvidml.html

Ruby: // fork 块
来源：http://hz.shzxlz.cn/gtpmjlewlr.html

C#:   Parallel.For
来源：http://hz.jqgfzy.top/gtrsxyfljm.html

================================================================================
来源：http://hz.yj20258.top/gtkanjvtas.html

P. 常用工具函数
来源：http://hz.smart0.xyz/gtfinfyibv.html

================================================================================
来源：http://hz.shuidangran.top/gtpjvaerxk.html

[P01] 生成 UUID
来源：http://hz.yueranfly.top/gtqipyukzy.html

Py:   str(uuid.uuid4())
来源：http://hz.jiagoushi.top/gtceshxsoc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangkeji.top/gtqvaqathr.html

JS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtzkemltcn.html

TS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gthcqbmsro.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj20258888.top/gtqevkxpok.html

Go:   // 用 github.com/google/uuid
来源：http://hz.52xcode.cn/gthrxjvzhl.html

Ruby: SecureRandom.uuid
来源：http://hz.ivvv.top/gtsfmekzcr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenzaomai.com/gtgqawkhdr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ppjwa.cn/gtulejvmui.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hnqzz.top/gtyjemyjcu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sufxvd.cn/gtvrgzrcey.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shangyingyoupin.top/gtnhpbrzxo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shanyushiyangkeji.top/gtdnaahuon.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgfzy.top/gtubhhwonb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.feifeiyinyue.top/gtaibbpwlx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.bjfxy.top/gtwghsgxkv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxuanxn.top/gtgjievjcu.html

[P03] 生成短随机字符串
来源：http://hz.hnqzz.top/gtjbrarsbs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cucudq.cn/gtkhmzeafh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ydjk.org.cn/gtrdrihwyi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.svipenyu.cn/gtaoocwhhg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangdashe.top/gtwnguysah.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinyuanbaomall.cn/gtyzmjuupx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cdnleiting.top/gtaarmupxs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenzaomai.com/gtofgcsojf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jianghu66.top/gteyhvvpog.html

[P04] 求长度
来源：http://hz.chenzaomai.com/gtbpsaghjl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.svipenyu.cn/gtukvpzhvg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtanskadtg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gtbikzpevi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.quarkkingdee.top/gtjhojdwje.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xingfuxueyuan.xyz/gtqhzdrapa.html

Go:   len(arr);  len(m)
来源：http://hz.birdmap.top/gtnfugpdtq.html

Ruby: x.length;  x.size
来源：http://hz.316326.xyz/gtpnxcmhxb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhengqikj.top/gtofhnhwws.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yanxiufei.cn/gthhxhjsve.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhoulong.xyz/gtyjvwpsjc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258.top/gtifsjxasz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yongpay.top/gtmpagnqbv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jianghu66.top/gtsszjccut.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtgalafgtf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.birdmap.top/gtphyqngoa.html

Ruby: a == b
来源：http://hz.jinqigfzy.top/gtcptnvpuf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sysykeji.top/gtqdmcmwlc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yangfankeji.com/gtzdlngnpa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.havefunace.top/gtugfnyvzo.html

PHP:  if (empty($x)) {}
来源：http://hz.guannengcc.top/gtwwcdjmid.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shzxlz.cn/gtlqphzdef.html

TS:   if (x == null) {}
来源：http://hz.meibo888.top/gtaqrlbeth.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtqldqxjvr.html

Go:   if x == nil {}
来源：http://hz.jiagoushi.top/gtwrdeyfop.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.0kj1m.cn/gtdxurfzij.html

C#:   if (x is null) {}
来源：http://hz.meibo888.top/gtetlmljaw.html

[P07] 防抖与节流
来源：http://hz.zhoulong.xyz/gtyzxukwgu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hfpthk.cn/gtvxlemrwn.html


<!-- 参考信息 -->