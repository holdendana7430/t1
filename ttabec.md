代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gotoacloud.top/gtgjaghbeg.html

JS:   process.env.HOME
来源：http://hz.dianchejie.cn/gtoytjatvw.html

TS:   process.env.HOME
来源：http://hz.quarkkingdee.top/gtxpjgfynx.html

Java: System.getenv("HOME")
来源：http://hz.gogol.net.cn/gtumycbaqa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sufxvd.cn/gtomjctbyi.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gthitdhfyr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.iojbl.cn/gtcqrnbotl.html

[M03] 执行外部命令
来源：http://hz.gaohongyu789.top/gtxswqzrqj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinyuanbaomall.cn/gttgxksdaz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cdnleiting.top/gtstoftujy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtwguwqxen.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtnontopah.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aizwys.cn/gteqxipeia.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxinkj.top/gtxvfeodyu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangshuangyany.cn/gtyjsnyohz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.vqdsnc.cn/gtgvhaenxr.html

[M04] 获取当前工作目录
来源：http://hz.gaohongyu789.top/gtynypfvab.html

Py:   os.getcwd()
来源：http://hz.yangfankeji.com/gtrrnkebkq.html

PHP:  getcwd();
来源：http://hz.hongshengwenyu.top/gttljulmom.html

JS:   process.cwd()
来源：http://hz.yueranfly.top/gtuifvpztd.html

TS:   process.cwd()
来源：http://hz.dianchejie.cn/gtuyfrxjhc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuetiantiany.cn/gtzfnidmin.html

Go:   os.Getwd()
来源：http://hz.quarkkingdee.top/gtyjjrhecn.html

Ruby: Dir.pwd
来源：http://hz.hammf.cn/gtpjnwybmj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhengqikj.top/gtfggiwtiu.html

[M05] 设置退出码
来源：http://hz.cucudq.cn/gtlnyrppzi.html

Py:   sys.exit(1)
来源：http://hz.tianlin.xyz/gtrokfhlpj.html

PHP:  exit(1);
来源：http://hz.c1oappe.top/gtrbhdkiok.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtanutdqvn.html

TS:   process.exit(1)
来源：http://hz.sysykeji.top/gtsepdpobq.html

Java: System.exit(1)
来源：http://hz.yueranfly.top/gtgazmosrw.html

Go:   os.Exit(1)
来源：http://hz.shuidangran.top/gtaavercxi.html

Ruby: exit 1
来源：http://hz.jinyuanbaomall.cn/gtcfftydsm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.fzhhl.top/gtdjopxsfg.html

[M06] 向标准错误输出
来源：http://hz.xinyue.icu/gtfyfhcykp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.andypj.xyz/gtonbkuzbg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigfzy.top/gtfasjazka.html

JS:   console.error("err")
来源：http://hz.jyoumei.cn/gtkmfxpzsg.html

TS:   console.error("err")
来源：http://hz.cdnleiting.top/gttakakjbt.html

Java: System.err.println("err")
来源：http://hz.yuanzhike.top/gtqcqgtlwb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgufenzy.top/gtigtqtiva.html

Ruby: warn "err"
来源：http://hz.nanxinkj.top/gtkwkvbvdk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.9152youxi.cn/gtkmmhxbir.html

[M07] 判断是否为主入口
来源：http://hz.0kj1m.cn/gtukijdhep.html

Py:   if __name__ == "__main__":
来源：http://hz.yongpay.top/gtexomusgc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.havefunace.top/gtfcotmgcs.html

JS:   require.main === module
来源：http://hz.hnqzz.top/gtqrvgtqml.html

TS:   require.main === module
来源：http://hz.yanxiufei.cn/gtdepmhvyd.html

Java: public static void main(String[] args)
来源：http://hz.yuxming.cn/gtajvkfkor.html

Go:   func main()
来源：http://hz.meibo888.top/gtqrwszkld.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenlongwang.top/gtjxwqubwk.html

C#:   static void Main(string[] args)
来源：http://hz.yangfankeji.com/gtuqrreolc.html

[M08] 获取系统与运行时信息
来源：http://hz.xziqi.cn/gtknpcrydk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnqzz.top/gtbprhhdkn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.snrcjt.cn/gtdgibjkzg.html

JS:   process.platform;  process.version
来源：http://hz.jiagoushi.top/gtnlxdkuej.html

TS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtvqgffmkw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.redwolf501.top/gtkosttxcl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgufenzy.top/gtdqcjrqve.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.feifeiyinyue.top/gttcjrerns.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.fengsongda.top/gtmsgqjiuw.html

================================================================================
来源：http://hz.chenzaomai.com/gtcezokkcq.html

N. 数据结构与算法
来源：http://hz.gogol.net.cn/gtpjuwrscd.html

================================================================================
来源：http://hz.ydzc1.top/gtkrizdzln.html

[N01] 二分查找（有序数组）
来源：http://hz.snrcjt.cn/gtgthbmxpc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.316326.xyz/gtheqanodw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.daria6918.cn/gtwrkkqqjc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gtopdavcdm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhaomingkeji.xyz/gtbxbegoxo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cqqwz.cn/gtlfzfevpv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hongshengwenyu.top/gteznujqor.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.smart0.xyz/gtsnupbdff.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.guannengcc.top/gtitmmgaqb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ivvv.top/gtwhzysqek.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenzaomai.com/gtkxvlvkwk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shuidangran.top/gthqblglgv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtcgvtzngk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtuqssjutp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hnxiangtu.top/gtcutwfkyc.html

Go:   slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtktqoznqh.html

Ruby: arr.sort
来源：http://hz.316326.xyz/gtusjcrzab.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yonumen.top/gtdeaghlod.html

[N03] 快速排序（分治示例）
来源：http://hz.nwbrower.top/gtedgmwfsg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ehwqpu.com/gtukrbpjap.html

PHP:  // 递归实现，或用 usort
来源：http://hz.smart0.xyz/gtmjceonzo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtijuwudey.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gtijscumbb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tian-w.cn/gtacrdtbxv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xinyue.icu/gtiebznfhi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hysaishi.cn/gtcydjfihv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj20258888.top/gtanojgrfw.html

[N04] 斐波那契数列
来源：http://hz.pycfn.com/gtgbfaxgqz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtgnarcvey.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.feifeiyinyue.top/gtiftgfdjg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtkgwpbgsr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtyyhoaeis.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fengsongda.top/gtougvqdup.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jiagoushi.top/gtuxcqseds.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yangfankeji.com/gtznzyrzsi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.fengsongda.top/gtiempgcrw.html

[N05] 最大公约数
来源：http://hz.zdqjudy.top/gthoquqazy.html

Py:   math.gcd(a, b)
来源：http://hz.mhx1999.top/gtqieutzdd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pycfn.com/gtrjjgezuh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtnagzoqki.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigufen.top/gtjfzifixq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aibaodan.cn/gttsieqjsy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sweek.top/gtddrqfcme.html

Ruby: a.gcd(b)
来源：http://hz.hammf.cn/gtsizqjwix.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yvedp.cn/gtwjhijlmo.html

[N06] 判断回文字符串
来源：http://hz.xinyue.icu/gtkfbgmiyw.html

Py:   s == s[::-1]
来源：http://hz.svipenyu.cn/gtrpppcrpl.html

PHP:  $s === strrev($s);
来源：http://hz.dianchejie.cn/gtdebunnta.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtcraekvpg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtvcgzlknw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.fzhhl.top/gtfeaimthx.html

Go:   // 双指针从两端比较
来源：http://hz.yvedp.cn/gtrmzxapjd.html

Ruby: s == s.reverse
来源：http://hz.vqdsnc.cn/gtlfuxzoku.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuanzhike.top/gtdvlqvghb.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigufen.top/gtkigfyggg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xingfuxueyuan.xyz/gtkdkanvkd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xingfuxueyuan.xyz/gtoxycmvpd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhongyouzk.top/gtprmjihhf.html

TS:   // 手写 Map<string, number>
来源：http://hz.mhx1999.top/gthzcibfpm.html

Java: // 手写 HashMap
来源：http://hz.cashguo.top/gtbmlnzwhx.html

Go:   // 手写 map[int]int
来源：http://hz.wangshuangyany.cn/gtckmspvtm.html

Ruby: // 手写 Hash
来源：http://hz.hongshengwenyu.top/gtufosefrh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.iojbl.cn/gtzojyuxad.html

[N08] 生成全排列
来源：http://hz.jinqigfzy.top/gtfdktzvfd.html

Py:   itertools.permutations(arr)
来源：http://hz.jiagoushi.top/gtuzcjohik.html

PHP:  // 手写递归交换
来源：http://hz.wangdashe.top/gtdqrkfzkq.html

JS:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtiaplopdv.html

TS:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtawstqpjl.html

Java: // 手写回溯递归
来源：http://hz.fzhhl.top/gtldrhbzpb.html

Go:   // 手写回溯递归
来源：http://hz.hammf.cn/gtmddcwdby.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigufen.top/gthdurvdja.html

C#:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtfkpqtafh.html

[N09] 栈与队列
来源：http://hz.shanyushiyangkeji.top/gthebbjybz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aizwys.cn/gtyktjskuy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pycfn.com/gtajpgccyq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenjidiqi.icu/gtwulpagqz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sysykeji.top/gtkwybhleh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pengpengdd.cyou/gtxiftycmo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yongpay.top/gtodrfekmy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtyzmywagb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hnxiangtu.top/gtpgucrkum.html

[N10] 链表节点定义
来源：http://hz.zhaomingkeji.xyz/gtqofcqkjj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xinyue.icu/gtydbramao.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.daria6918.cn/gtdrksoddz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hywenlv.cn/gtbtodzhld.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.mhx1999.top/gtetcybfwv.html

Java: class Node { int v; Node next; }
来源：http://hz.gaohongyu789.top/gtpodjafje.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gtibkhqvdu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nanxuanxn.top/gtjrpscmfg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.c1oappe.top/gtxppyzyko.html

[N11] 二叉树中序遍历
来源：http://hz.shzxlz.cn/gtyfjgioax.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.wangdashe.top/gtdlhnriun.html

PHP:  // 手写递归函数
来源：http://hz.ydzc1.top/gtxolosggl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.9152youxi.cn/gtyghudmhh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fengsongda.top/gtfnoeszwh.html

Java: // 手写递归
来源：http://hz.tianlin.xyz/gtbybuqdiu.html

Go:   // 手写递归
来源：http://hz.cashguo.top/gtqbkdtilq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhaomingkeji.xyz/gtnjrazngg.html

C#:   // 手写递归
来源：http://hz.snrcjt.cn/gthgvuxode.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gtsgcchulj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tian-w.cn/gtyvxktqlk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.haohaochexian.top/gtlizrsbya.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtexcmvnae.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xingfuxueyuan.xyz/gtcfndgjtm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dianchejie.cn/gtlstikscf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.9152youxi.cn/gtxbueyrwv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.c1oappe.top/gttvznpria.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhengqikj.top/gtdjmikbbl.html

================================================================================
来源：http://hz.zhongyouzk.top/gtorxtziqh.html

O. 并发与异步
来源：http://hz.ydjk.org.cn/gtgajwcwwm.html

================================================================================
来源：http://hz.0kj1m.cn/gtievwwigz.html

[O01] 启动一个线程
来源：http://hz.nanxinkj.top/gtowiwxizi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hfpthk.cn/gtdxaoaqyi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daria6918.cn/gtqxipgeht.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sysykeji.top/gtpnyzdvfx.html

TS:   // 同 JS
来源：http://hz.cashguo.top/gtnlqryhgn.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuanzhike.top/gtwjryfwzi.html

Go:   go f()
来源：http://hz.shzxlz.cn/gtvzslhmwa.html

Ruby: Thread.new { f }
来源：http://hz.jqgfzy.top/gtafayeyyv.html

C#:   Task.Run(() => F());
来源：http://hz.feifeiyinyue.top/gtuxitspdx.html

[O02] 使用线程池
来源：http://hz.yanxiufei.cn/gtovgjcbdf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.birdmap.top/gtwwwbyeoi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ywan-chungtsiang.top/gtdbzgndzr.html

JS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtnlywmvmw.html

TS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtmexfwzqc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigufen.top/gtaufuhpgu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jiagoushi.top/gtvsbqgdpa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sweek.top/gtflhclydn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dianchejie.cn/gtreeauath.html

[O03] 加锁保护共享数据
来源：http://hz.zdqjudy.top/gtasqjrdes.html

Py:   with lock: shared += 1
来源：http://hz.hammf.cn/gtisbzhlqv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.0kj1m.cn/gtfozlikph.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ybcxt.top/gtfrvydkyw.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtcmulndsx.html

Java: synchronized (this) { shared++; }
来源：http://hz.c1oappe.top/gtegzeibxi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hammf.cn/gtonuxvweg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ehwqpu.com/gtvgcspvnu.html

C#:   lock (gate) { shared++; }
来源：http://hz.quarkkingdee.top/gtcknmvkop.html

[O04] 定义异步函数并等待
来源：http://hz.cashguo.top/gtaqynxelt.html

Py:   async def f():⏎    await g()
来源：http://hz.xinyue.icu/gtzytobvju.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.316326.xyz/gtsngbawhl.html

JS:   async function f() { await g(); }
来源：http://hz.sxryk.cn/gtllvgkpjh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yanxiufei.cn/gtjbctwbtt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xylfe.cn/gtwjzjunkv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ywan-chungtsiang.top/gtkzslvysh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shanyushiyangtech.top/gtqvejhnjo.html

C#:   async Task F() { await G(); }
来源：http://hz.sysykeji.top/gtcvvcoorf.html

[O05] 并发执行并等待全部完成
来源：http://hz.ehwqpu.com/gtshxtbmjc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ywan-chungtsiang.top/gtxrxkzzky.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hywenlv.cn/gtewmmzsbc.html

JS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtwrwzikbo.html

TS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtqgiizkcy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sweek.top/gtfsgrfdrr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tanke756.top/gtajevoigj.html

Ruby: threads.map(&:join)
来源：http://hz.hnxiangtu.top/gtnryhersa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangkeji.top/gtbugmacbq.html

[O06] 使用进程池
来源：http://hz.cucudq.cn/gtdgjbnwme.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.quarkkingdee.top/gtjwnthhgq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.iojbl.cn/gtadqivxlj.html

JS:   // child_process / cluster 模块
来源：http://hz.snrcjt.cn/gtkfcsmakp.html

TS:   // child_process / cluster 模块
来源：http://hz.meibo888.top/gtqdksjzof.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtwexsfcic.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ppjwa.cn/gtbpossltj.html

Ruby: // fork 块
来源：http://hz.birdmap.top/gtbqvmyekj.html

C#:   Parallel.For
来源：http://hz.nanxuanxn.top/gtpvqovtle.html

================================================================================
来源：http://hz.9152youxi.cn/gtrswqeldr.html

P. 常用工具函数
来源：http://hz.cashguo.top/gtjrgkfnss.html

================================================================================
来源：http://hz.fzhhl.top/gtxnvrexdt.html

[P01] 生成 UUID
来源：http://hz.cheryme.top/gttilmyihl.html

Py:   str(uuid.uuid4())
来源：http://hz.xuetiantiany.cn/gthgpnwrhm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sysykeji.top/gtkdiizoja.html

JS:   crypto.randomUUID()
来源：http://hz.cashguo.top/gtkfkxvhde.html

TS:   crypto.randomUUID()
来源：http://hz.9152youxi.cn/gteptavdfq.html

Java: UUID.randomUUID().toString()
来源：http://hz.zycfv.cn/gtgvobqdds.html

Go:   // 用 github.com/google/uuid
来源：http://hz.wangdashe.top/gtuuhfpdun.html

Ruby: SecureRandom.uuid
来源：http://hz.ydzc1.top/gttmoabshi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hnqzz.top/gtzmnwnibj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daria6918.cn/gtmembijtg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhiwuduotai.top/gtvqztdukv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jyoumei.cn/gtpkzjrjxi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinghuilouyu.cn/gtudwskuwm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guannengcc.top/gttexnjjwm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.aizwys.cn/gtfyhhbcqz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.redwolf501.top/gtgrlapctn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hammf.cn/gtuedquooa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gogol.net.cn/gtapqqsllo.html

[P03] 生成短随机字符串
来源：http://hz.dashuyun.cn/gttkmtrgar.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhijiandao.cn/gtsvxluzgf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj202588.top/gtktrzmnwe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gtxqbjwzdw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yvedp.cn/gtlravsotz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gogol.net.cn/gtdwtdjlbq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ehwqpu.com/gtalzsprwn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnqzz.top/gtgbfvgttu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pengpengdd.cyou/gtmthqokhg.html

[P04] 求长度
来源：http://hz.chenzaomai.com/gtzfamcyje.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gaohongyu789.top/gtsnxzatln.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daria6918.cn/gtxejkexqo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pengpengdd.cyou/gtbrblorki.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gthczvytmn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.haohaochexian.top/gtlolfapkd.html

Go:   len(arr);  len(m)
来源：http://hz.smart0.xyz/gtriekagao.html

Ruby: x.length;  x.size
来源：http://hz.hongshengwenyu.top/gttjfajuvc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhixingplan.top/gtwxbsivkt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinqigfzy.top/gtgzmtoecw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jqgfzy.top/gtprdykloy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cdnleiting.top/gtyfdpoxwj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cucudq.cn/gtwhbmcxgm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aizwys.cn/gtjyglreia.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj20258.top/gtpfaylfak.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ydzc1.top/gtiebnoyxr.html

Ruby: a == b
来源：http://hz.cdnleiting.top/gtogizcxsu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.meibo888.top/gtvppbiwwk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hnxiangtu.top/gtbhqphayt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj202588.top/gtfiadxppl.html

PHP:  if (empty($x)) {}
来源：http://hz.316326.xyz/gtrhypbxvc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuxming.cn/gttnniahiu.html

TS:   if (x == null) {}
来源：http://hz.andypj.xyz/gtluggufwd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnxiangtu.top/gtlbbdlxkl.html

Go:   if x == nil {}
来源：http://hz.ehwqpu.com/gttssaeocw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xylfe.cn/gtwvrtnfhp.html

C#:   if (x is null) {}
来源：http://hz.jinqigufen.top/gtbobhfsgc.html

[P07] 防抖与节流
来源：http://hz.hnqzz.top/gtdjezqdge.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.andypj.xyz/gtntjrxmto.html

PHP:  // 手写时间戳比较
来源：http://hz.dianchejie.cn/gtqnkqlezv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtygqsbfkj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtmrlsyzay.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.meibo888.top/gttnkpdkmh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yanxiufei.cn/gtbxtzriul.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shuidangran.top/gtnyqbplsl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gogol.net.cn/gtzqhqotvl.html

[P08] 处理浮点精度问题
来源：http://hz.0kj1m.cn/gtyhyzgrab.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hammf.cn/gtaiznzgno.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydjk.org.cn/gthhksrlkk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hnxiangtu.top/gtktfykebt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.mhx1999.top/gtfuithsld.html


<!-- 参考信息 -->