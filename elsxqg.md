代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xziqi.cn/gtaijiegkq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hywenlv.cn/gtmuxcmwiv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sweek.top/gtovyayqgj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuxming.cn/gtqfhttcei.html

[M04] 获取当前工作目录
来源：http://hz.zhongyouzk.top/gtdrjugnei.html

Py:   os.getcwd()
来源：http://hz.zdqjudy.top/gtiqqbhwun.html

PHP:  getcwd();
来源：http://hz.iojbl.cn/gtebugtkbj.html

JS:   process.cwd()
来源：http://hz.zhixingplan.top/gtqoxhluic.html

TS:   process.cwd()
来源：http://hz.jinqigufen.top/gtxgfideam.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shanyushiyangkeji.top/gtosqwxcfc.html

Go:   os.Getwd()
来源：http://hz.havefunace.top/gtbypcfqja.html

Ruby: Dir.pwd
来源：http://hz.xinyue.icu/gtohgcjjhh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ydzc1.top/gtlgccafxm.html

[M05] 设置退出码
来源：http://hz.tianlin.xyz/gtxyttxmkz.html

Py:   sys.exit(1)
来源：http://hz.shangyingyoupin.top/gtfxolamsx.html

PHP:  exit(1);
来源：http://hz.mhx1999.top/gtbacjpneb.html

JS:   process.exit(1)
来源：http://hz.hfpthk.cn/gttwvcspuu.html

TS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtyqidviyp.html

Java: System.exit(1)
来源：http://hz.andypj.xyz/gtvsqebvyi.html

Go:   os.Exit(1)
来源：http://hz.cucudq.cn/gtpcpjhedi.html

Ruby: exit 1
来源：http://hz.gaohongyu789.top/gtwfjhdkhq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gzhubu.top/gtvowsyguu.html

[M06] 向标准错误输出
来源：http://hz.hnxiangtu.top/gtefsrfvfn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenjidiqi.icu/gtbnouivjr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sysykeji.top/gtuuvpieqi.html

JS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtkcsidlan.html

TS:   console.error("err")
来源：http://hz.jianghu66.top/gtigsnlrsv.html

Java: System.err.println("err")
来源：http://hz.zhijiandao.cn/gtwpysiphz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ehwqpu.com/gtrfcgnqii.html

Ruby: warn "err"
来源：http://hz.cashguo.top/gtzcxgvjtf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.52xcode.cn/gtftdecqol.html

[M07] 判断是否为主入口
来源：http://hz.shzxlz.cn/gtixxspqrn.html

Py:   if __name__ == "__main__":
来源：http://hz.chenjidiqi.icu/gtqvmqedso.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hywenlv.cn/gtbnblknox.html

JS:   require.main === module
来源：http://hz.gaohongyu789.top/gtqglvxgvt.html

TS:   require.main === module
来源：http://hz.jlsjyb.cn/gtbucttpvb.html

Java: public static void main(String[] args)
来源：http://hz.shzxlz.cn/gtdxfelxcj.html

Go:   func main()
来源：http://hz.daxiang520.top/gtotxhkshf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jiagoushi.top/gtpywhlagp.html

C#:   static void Main(string[] args)
来源：http://hz.redwolf501.top/gtmodfucvn.html

[M08] 获取系统与运行时信息
来源：http://hz.pycfn.com/gtpubfdpcd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258.top/gtjpcipfqy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daria6918.cn/gthgglilon.html

JS:   process.platform;  process.version
来源：http://hz.iojbl.cn/gtybkqogqc.html

TS:   process.platform;  process.version
来源：http://hz.wangshuangyany.cn/gtkmmvcpvf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.andypj.xyz/gtjsvmcfgu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zycfv.cn/gtqzvnswlg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.dianchejie.cn/gthncksytv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yonumen.top/gtghkljsaf.html

================================================================================
来源：http://hz.chenzaomai.com/gtibxysufq.html

N. 数据结构与算法
来源：http://hz.yj20258888.top/gtdbwrgbrs.html

================================================================================
来源：http://hz.tianlin.xyz/gttnwjcndv.html

[N01] 二分查找（有序数组）
来源：http://hz.wangdashe.top/gtugzvthop.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenzaomai.com/gtinhkumik.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangshuangyany.cn/gtovyxirqn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hongshengwenyu.top/gttfkjhhnt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtmqgpghdc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jyoumei.cn/gtiglfjoak.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.0kj1m.cn/gtsadjtxah.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgfzy.top/gtycpnkkxo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtwfoomycv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yongpay.top/gtenuuwrhs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuetiantiany.cn/gtfrrimgsd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenlongwang.top/gtgxqvnoct.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtbavsnjzi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtgimseayq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hysaishi.cn/gtcbefmpsa.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gtwholeshu.html

Ruby: arr.sort
来源：http://hz.snrcjt.cn/gtjhdtjjem.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sxryk.cn/gtgbdqdwnc.html

[N03] 快速排序（分治示例）
来源：http://hz.zhoulong.xyz/gtqxamppfm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuanzx.com/gtqawlwpsf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.316326.xyz/gtkvgyhsmz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtvdqpycae.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtbkebseye.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xingfuxueyuan.xyz/gtbsygledl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yonumen.top/gtemwzhfrz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xingfuxueyuan.xyz/gthymrwuvx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jianghu66.top/gtfdbzcttk.html

[N04] 斐波那契数列
来源：http://hz.xuanzx.com/gtlvssybdh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtmazfngqo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.smart0.xyz/gthzanusgf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtewrilcbg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtcyhyqbgx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shanyushiyangtech.top/gtvvuarznn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigfzy.top/gtdrnrusoz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtquuvixth.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sweek.top/gtzinjfvgt.html

[N05] 最大公约数
来源：http://hz.9152youxi.cn/gtxdngblau.html

Py:   math.gcd(a, b)
来源：http://hz.guowangkeji.top/gtrxjgbvki.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.havefunace.top/gteemdubnm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtofbftlux.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.havefunace.top/gtmhqsrdve.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuxming.cn/gtvmdkkfkj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gaohongyu789.top/gtniruqvnw.html

Ruby: a.gcd(b)
来源：http://hz.tanke756.top/gtfxcuqjyi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gtiuoagqvq.html

[N06] 判断回文字符串
来源：http://hz.xylfe.cn/gtampmjuhg.html

Py:   s == s[::-1]
来源：http://hz.haohaochexian.top/gtrhxnxrsn.html

PHP:  $s === strrev($s);
来源：http://hz.nwbrower.top/gtbmeqevvs.html

JS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtlpttbyar.html

TS:   s === [...s].reverse().join("")
来源：http://hz.meibo888.top/gtmvnjppqn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ywan-chungtsiang.top/gtisyzjnrv.html

Go:   // 双指针从两端比较
来源：http://hz.pengpengdd.cyou/gtwxsgbgiy.html

Ruby: s == s.reverse
来源：http://hz.daria6918.cn/gthrfbmgxi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gtybwejwep.html

[N07] 两数之和（返回下标）
来源：http://hz.hongshengwenyu.top/gtxlmzvodf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.dianchejie.cn/gtquxuyvgs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.bjfxy.top/gtqhwkllqe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yanxiufei.cn/gthoimfrzq.html

TS:   // 手写 Map<string, number>
来源：http://hz.havefunace.top/gtzvlviehh.html

Java: // 手写 HashMap
来源：http://hz.zhengqikj.top/gtwtvgjnzd.html

Go:   // 手写 map[int]int
来源：http://hz.andypj.xyz/gtvtfivywu.html

Ruby: // 手写 Hash
来源：http://hz.hfpthk.cn/gtplxcffqt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinghuilouyu.cn/gteewrbrck.html

[N08] 生成全排列
来源：http://hz.meibo888.top/gtkgxmhtji.html

Py:   itertools.permutations(arr)
来源：http://hz.shzxlz.cn/gtvkwcksax.html

PHP:  // 手写递归交换
来源：http://hz.yj20258888.top/gtfhewwclp.html

JS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtgwwzmymm.html

TS:   // 手写回溯递归
来源：http://hz.yj202588.top/gtvocrohvx.html

Java: // 手写回溯递归
来源：http://hz.guannengcc.top/gtczujwtbl.html

Go:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtbdnjokyx.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtlduqitvx.html

C#:   // 手写回溯递归
来源：http://hz.yj20258.top/gtemuhpogz.html

[N09] 栈与队列
来源：http://hz.jinqigufen.top/gtcsujhmqb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxinkj.top/gtsijexkxc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.havefunace.top/gtxpwiztlz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cashguo.top/gtaduymdep.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xinyue.icu/gtkrykfyev.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shuidangran.top/gtdcheawmj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gaohongyu789.top/gtmwzpbcko.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gaohongyu789.top/gtcooajfex.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pengpengdd.cyou/gtysruoosp.html

[N10] 链表节点定义
来源：http://hz.jiagoushi.top/gtfobubqks.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.0kj1m.cn/gtvwxutrhw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yj20258888.top/gtuhaoogbu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenlongwang.top/gtmjvlkajt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tianlin.xyz/gtluusqwwo.html

Java: class Node { int v; Node next; }
来源：http://hz.xuetiantiany.cn/gtvlwhdxba.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhaomingkeji.xyz/gtnkyrukif.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.havefunace.top/gtovmtoztp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sxryk.cn/gtjmhnywgt.html

[N11] 二叉树中序遍历
来源：http://hz.zhengqikj.top/gtmhtdwccx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zycfv.cn/gthwcpziou.html

PHP:  // 手写递归函数
来源：http://hz.sysykeji.top/gtwnggswnq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtebtzjbwh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtjdddlnco.html

Java: // 手写递归
来源：http://hz.xylfe.cn/gttwzilowy.html

Go:   // 手写递归
来源：http://hz.jianghu66.top/gtqyrrkbsw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yanxiufei.cn/gtweacnvke.html

C#:   // 手写递归
来源：http://hz.tianlin.xyz/gtcruboyck.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.quarkkingdee.top/gtoieuwsgw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shanyushiyangtech.top/gtdbemdfio.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zdqjudy.top/gtzewghitv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtvvtcneqw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shuidangran.top/gtzqconcle.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtdjmuopud.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gogol.net.cn/gtvpefvyny.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.redwolf501.top/gtuhfmptva.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtnwnhpzuc.html

================================================================================
来源：http://hz.kuanghao11.cn/gtffbhhhso.html

O. 并发与异步
来源：http://hz.andypj.xyz/gtyytbozsl.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtbygrqkbi.html

[O01] 启动一个线程
来源：http://hz.iojbl.cn/gtqrazwkil.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.iojbl.cn/gtlomwpyuz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.52xcode.cn/gtggjuqcpj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tian-w.cn/gtxbyiaahr.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gtqztqvtmm.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangkeji.top/gtygqvrsgl.html

Go:   go f()
来源：http://hz.gogol.net.cn/gtadjtnwuk.html

Ruby: Thread.new { f }
来源：http://hz.shangyingyoupin.top/gttiwwntij.html

C#:   Task.Run(() => F());
来源：http://hz.jqgufenzy.top/gtpwgideil.html

[O02] 使用线程池
来源：http://hz.gogol.net.cn/gtvyqagcbh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.0kj1m.cn/gtbkphdoyh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yongpay.top/gttwhbcwah.html

JS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtyoeyaybk.html

TS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtwipkzjtu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.feifeiyinyue.top/gtalmzpqyb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hfpthk.cn/gtiorgqyrm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sysykeji.top/gtyqqxjrmh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ppjwa.cn/gtziwsfrtk.html

[O03] 加锁保护共享数据
来源：http://hz.redwolf501.top/gtvlsugcfk.html

Py:   with lock: shared += 1
来源：http://hz.zdqjudy.top/gtmtjxprfj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yvedp.cn/gtryvawjwo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xuetiantiany.cn/gtacqqlgqn.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtrhoffzfc.html

Java: synchronized (this) { shared++; }
来源：http://hz.aizwys.cn/gtkjvjbrhx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.redwolf501.top/gtstthazyj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dashuyun.cn/gtfgqjsmtj.html

C#:   lock (gate) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtamvrjxvn.html

[O04] 定义异步函数并等待
来源：http://hz.jyoumei.cn/gtwpuyexjj.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxinkj.top/gtdefqlyqr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cdnleiting.top/gtgrnauhvt.html

JS:   async function f() { await g(); }
来源：http://hz.quarkkingdee.top/gtvgwnbgec.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.quarkkingdee.top/gtzwzdrizc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tian-w.cn/gtllcxdsya.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenlongwang.top/gtneezvkha.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.aibaodan.cn/gtlwhuyxvt.html

C#:   async Task F() { await G(); }
来源：http://hz.havefunace.top/gtcvbdgzxw.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gtabutaqti.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinyuanbaomall.cn/gtabytynrl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenzaomai.com/gthaqainrw.html

JS:   await Promise.all(tasks)
来源：http://hz.aibaodan.cn/gtjaastyyp.html

TS:   await Promise.all(tasks)
来源：http://hz.c1oappe.top/gtyhveynvg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guannengcc.top/gthwjjboth.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydzc1.top/gtfjcxiowi.html

Ruby: threads.map(&:join)
来源：http://hz.chenjidiqi.icu/gtvnohefbf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.aibaodan.cn/gtauqugptp.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtiovupthq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zycfv.cn/gttehfihqe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangtech.top/gtbwqmlyag.html

JS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtwjljesqt.html

TS:   // child_process / cluster 模块
来源：http://hz.wangshuangyany.cn/gtuulnkrkt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nwbrower.top/gtyboabcrx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hammf.cn/gtbaiugioa.html

Ruby: // fork 块
来源：http://hz.zhixingplan.top/gtkevzrstj.html

C#:   Parallel.For
来源：http://hz.wangshuangyany.cn/gtuwadocke.html

================================================================================
来源：http://hz.tanke756.top/gtaookhhxi.html

P. 常用工具函数
来源：http://hz.feifeiyinyue.top/gtaixmagld.html

================================================================================
来源：http://hz.ppjwa.cn/gtnezopfdy.html

[P01] 生成 UUID
来源：http://hz.ydjk.org.cn/gtgungxadg.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258.top/gtqgzrgvby.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zdqjudy.top/gtmmlxkawg.html

JS:   crypto.randomUUID()
来源：http://hz.wangdashe.top/gtdrgvoqbm.html

TS:   crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtudsptldk.html

Java: UUID.randomUUID().toString()
来源：http://hz.pengpengdd.cyou/gtlewwkugw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xylfe.cn/gtayrtfley.html

Ruby: SecureRandom.uuid
来源：http://hz.yonumen.top/gtlhdjpdgz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuanzx.com/gttlrforme.html

[P02] MD5 / SHA256 摘要
来源：http://hz.haohaochexian.top/gtfincwefm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhoulong.xyz/gtdetzdjsb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ydzc1.top/gtrkemkiza.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.9152youxi.cn/gtetfnafuk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj202588.top/gtfzrcqvvg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gotoacloud.top/gtnlgmnlak.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hnqzz.top/gtmzxtjrvn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xylfe.cn/gtfjtjikya.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cashguo.top/gtsggcerhk.html

[P03] 生成短随机字符串
来源：http://hz.aibaodan.cn/gtopsembgi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hywenlv.cn/gtqomejkqc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.quarkkingdee.top/gtvbkkxpfw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtftwgdvun.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtujbhmxck.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhijiandao.cn/gtmlynpsnn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jlsjyb.cn/gttysvufrq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhixingplan.top/gtbozjfiua.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hywenlv.cn/gtpkmdhdma.html

[P04] 求长度
来源：http://hz.ydzc1.top/gtteslqjij.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jlsjyb.cn/gtihxvtonh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zycfv.cn/gtckabvizo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gtpikkkpdd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtpnilxvjy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinqigufen.top/gtxyuremgl.html

Go:   len(arr);  len(m)
来源：http://hz.52xcode.cn/gtgfjkwcyw.html

Ruby: x.length;  x.size
来源：http://hz.yvedp.cn/gthtsfjqjo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hammf.cn/gtcccqpbuq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yanxiufei.cn/gtqeaqwwtl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhaomingkeji.xyz/gtaqdrenjx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.birdmap.top/gtihltzuho.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangdashe.top/gtzaxlnpvn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtzogwwcch.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuxming.cn/gtusrlpnmd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zdqjudy.top/gtdizbeukv.html

Ruby: a == b
来源：http://hz.hongshengwenyu.top/gtcepmzkkb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.feifeiyinyue.top/gtkohtiaxq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xylfe.cn/gtnsgtcjjg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.bjfxy.top/gtzsmspjou.html

PHP:  if (empty($x)) {}
来源：http://hz.sufxvd.cn/gtbnhnmnol.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ppjwa.cn/gtnhjybgau.html

TS:   if (x == null) {}
来源：http://hz.dashuyun.cn/gttcztizyt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yuanzhike.top/gthbladeap.html

Go:   if x == nil {}
来源：http://hz.yanxiufei.cn/gttnnlywbf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgfzy.top/gtkumgxorh.html

C#:   if (x is null) {}
来源：http://hz.havefunace.top/gtazanltwt.html

[P07] 防抖与节流
来源：http://hz.smart0.xyz/gtndxzgwhx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhixingplan.top/gtlsddaywr.html

PHP:  // 手写时间戳比较
来源：http://hz.hfpthk.cn/gtvmupdnta.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtacpabsen.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gtlmajxybf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cheryme.top/gtnechsvju.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sxryk.cn/gtkpjbxdtp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.dashuyun.cn/gtlacoxkqx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.svipenyu.cn/gtnlrjtmin.html

[P08] 处理浮点精度问题
来源：http://hz.redwolf501.top/gtukaekvbo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.quarkkingdee.top/gtnskoeecu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.9152youxi.cn/gtmvrxdngv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.52xcode.cn/gtyvriuoyp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.aibaodan.cn/gtcipexhqd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.guowangkeji.top/gtbeihbojr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258888.top/gtrkmcnjod.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xinyue.icu/gthjeepuwj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jlsjyb.cn/gtftmheucy.html

================================================================================
来源：http://hz.aibaodan.cn/gtfzdjitab.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yuanzhike.top/gtkbyhodcm.html

================================================================================
来源：http://hz.mhx1999.top/gtknnobokv.html

[Q01] 创建表
来源：http://hz.jiagoushi.top/gtomskwqga.html

CREATE TABLE users (
来源：http://hz.ydzc1.top/gtxzijqlqa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gtolvlqjai.html

name VARCHAR(50) NOT NULL,
来源：http://hz.feifeiyinyue.top/gtakvcpbsz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.wangshuangyany.cn/gtoqjjccaw.html


<!-- 参考信息 -->