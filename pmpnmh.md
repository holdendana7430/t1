代发 wailian999

TS:   process.cwd()
来源：http://hz.ybcxt.top/gtkujxxojl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gzhubu.top/gtnmwzdham.html

Go:   os.Getwd()
来源：http://hz.shuidangran.top/gtrrdhjdmo.html

Ruby: Dir.pwd
来源：http://hz.yj202588.top/gtpxjnwahu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.daxiang520.top/gtzpjgxhcq.html

[M05] 设置退出码
来源：http://hz.guowangkeji.top/gthibvtavg.html

Py:   sys.exit(1)
来源：http://hz.hfpthk.cn/gtzjuwuxle.html

PHP:  exit(1);
来源：http://hz.cqqwz.cn/gtgsasdxra.html

JS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtfnmjjpoa.html

TS:   process.exit(1)
来源：http://hz.redwolf501.top/gtvqottdgc.html

Java: System.exit(1)
来源：http://hz.zhoulong.xyz/gtdungeeid.html

Go:   os.Exit(1)
来源：http://hz.birdmap.top/gtpdltwevm.html

Ruby: exit 1
来源：http://hz.cashguo.top/gtobuynpfg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.52xcode.cn/gtjvnfgcsb.html

[M06] 向标准错误输出
来源：http://hz.xinyue.icu/gtojvtdjxt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gthhfiyfyk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yanxiufei.cn/gtojovtyid.html

JS:   console.error("err")
来源：http://hz.guowangkeji.top/gtiyctueyd.html

TS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gttvacsghd.html

Java: System.err.println("err")
来源：http://hz.yongpay.top/gtpabafhcx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigfzy.top/gttigmoeti.html

Ruby: warn "err"
来源：http://hz.chenzaomai.com/gtacowsioa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhixingplan.top/gtghhvqnly.html

[M07] 判断是否为主入口
来源：http://hz.ppjwa.cn/gtfuzypiuo.html

Py:   if __name__ == "__main__":
来源：http://hz.hongshengwenyu.top/gteboffbzq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.316326.xyz/gtqdxkmzcd.html

JS:   require.main === module
来源：http://hz.wangdashe.top/gtrcxlrcgu.html

TS:   require.main === module
来源：http://hz.gotoacloud.top/gtqnpiprup.html

Java: public static void main(String[] args)
来源：http://hz.cashguo.top/gtysmbrmdd.html

Go:   func main()
来源：http://hz.9152youxi.cn/gtryonndfi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yonumen.top/gtwicprxwm.html

C#:   static void Main(string[] args)
来源：http://hz.sysykeji.top/gtnvbevkxb.html

[M08] 获取系统与运行时信息
来源：http://hz.shzxlz.cn/gtjuezdugf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xuanzx.com/gtijyoiitx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daxiang520.top/gtzipxpqei.html

JS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtqtrpfsjq.html

TS:   process.platform;  process.version
来源：http://hz.c1oappe.top/gteldkpcci.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.birdmap.top/gtknwbtwdh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.smart0.xyz/gtmponheid.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xingfuxueyuan.xyz/gttlxsoaqe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sufxvd.cn/gttntjipzk.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtididvmhb.html

N. 数据结构与算法
来源：http://hz.hywenlv.cn/gtvayisoao.html

================================================================================
来源：http://hz.nanxinkj.top/gtxxzmglnd.html

[N01] 二分查找（有序数组）
来源：http://hz.pycfn.com/gtmrfgjmso.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgfzy.top/gtwqivsspd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hfpthk.cn/gtagwnvwxi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtwjudoucf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtaszflkeu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtetoiqyec.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gogol.net.cn/gthmkpxvyx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hywenlv.cn/gtazxzciif.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pycfn.com/gtzbpawtjv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhoulong.xyz/gtlakeqskv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtpinfkqbd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yonumen.top/gtlwrqgnzr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnqzz.top/gtyhrkwkkb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtzlvadpuz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.kuanghao11.cn/gthuozexkm.html

Go:   slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gteczwmoem.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtogmyjeca.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenzaomai.com/gtuqxvdiyr.html

[N03] 快速排序（分治示例）
来源：http://hz.nanxuanxn.top/gtnujoyfcn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258.top/gtiyrpmgbi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guannengcc.top/gtaqkuzsga.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtlxctrerv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtisggoofz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhaomingkeji.xyz/gtuqbuyuik.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.snrcjt.cn/gtzxzagddy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dashuyun.cn/gtxwszzgwg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgfzy.top/gtuqnluqjp.html

[N04] 斐波那契数列
来源：http://hz.ppjwa.cn/gtncohrsfw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gthpqetofs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zdqjudy.top/gticaxqiqz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shzxlz.cn/gtluvnbsal.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daria6918.cn/gtfkzuiekz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dianchejie.cn/gtwfqdghxm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tian-w.cn/gtnclqfzyc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtopwbbapo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hywenlv.cn/gterkcedpm.html

[N05] 最大公约数
来源：http://hz.dianchejie.cn/gtjjmwwtmt.html

Py:   math.gcd(a, b)
来源：http://hz.9152youxi.cn/gtzgermkbs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cheryme.top/gtaevokpoi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtafmggyfj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jiagoushi.top/gtkbvifsxa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gotoacloud.top/gtjqmyqjzu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhiwuduotai.top/gtqjjkisny.html

Ruby: a.gcd(b)
来源：http://hz.yuanzhike.top/gtemwwluic.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jyoumei.cn/gtqvxmvcjk.html

[N06] 判断回文字符串
来源：http://hz.yuxming.cn/gtnkpajcxa.html

Py:   s == s[::-1]
来源：http://hz.ydzc1.top/gtcokgxoim.html

PHP:  $s === strrev($s);
来源：http://hz.nwbrower.top/gtdcczcxlb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtplqwnplt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtdhelwcvv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tian-w.cn/gtxzkdasam.html

Go:   // 双指针从两端比较
来源：http://hz.hnqzz.top/gtytvateph.html

Ruby: s == s.reverse
来源：http://hz.ivvv.top/gtwxbaovzg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenlongwang.top/gtlsxliwen.html

[N07] 两数之和（返回下标）
来源：http://hz.jqgufenzy.top/gtxbbkqnyy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgufenzy.top/gtpxxnjalh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gtwnndcmer.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hammf.cn/gteqpmqnpy.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gthbrurjex.html

Java: // 手写 HashMap
来源：http://hz.vqdsnc.cn/gtcdidrqur.html

Go:   // 手写 map[int]int
来源：http://hz.zhixingplan.top/gtthlukeqn.html

Ruby: // 手写 Hash
来源：http://hz.chenzaomai.com/gtiikxommf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dashuyun.cn/gtkwqomodz.html

[N08] 生成全排列
来源：http://hz.zhixingplan.top/gtwkjwlnru.html

Py:   itertools.permutations(arr)
来源：http://hz.yj202588.top/gtpbtzeqhf.html

PHP:  // 手写递归交换
来源：http://hz.jqgufenzy.top/gtznuemequ.html

JS:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtrihnvxpx.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtjyfgmugf.html

Java: // 手写回溯递归
来源：http://hz.xziqi.cn/gtfecuawsi.html

Go:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtnzpvpnik.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigfzy.top/gtyfjfguyp.html

C#:   // 手写回溯递归
来源：http://hz.316326.xyz/gtdfkeepfw.html

[N09] 栈与队列
来源：http://hz.xinyue.icu/gtktxdikgf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinqigufen.top/gtxlokwcfs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.daxiang520.top/gtczstjukv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhijiandao.cn/gtvnbrjxdm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhaomingkeji.xyz/gtujgdxfek.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shuidangran.top/gtwhrbiwbr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nwbrower.top/gtwpxgcyfh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.redwolf501.top/gtdjfbbwbe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.smart0.xyz/gtzrxjcqcd.html

[N10] 链表节点定义
来源：http://hz.tian-w.cn/gtajeieuay.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.meibo888.top/gtbwpkazbc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nanxuanxn.top/gtreteswvv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sufxvd.cn/gtvfkjvnwy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dianchejie.cn/gtirtvwety.html

Java: class Node { int v; Node next; }
来源：http://hz.redwolf501.top/gtfvlrrhee.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shangyingyoupin.top/gtinrogiqu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.andypj.xyz/gtdxlhjkjm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.andypj.xyz/gtyjbophqv.html

[N11] 二叉树中序遍历
来源：http://hz.gogol.net.cn/gtbzhukxib.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yanxiufei.cn/gtnyqsjxxg.html

PHP:  // 手写递归函数
来源：http://hz.hammf.cn/gtsvatjtww.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.9152youxi.cn/gtgwnkvspk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gtorwhawfa.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gtrkwwuxwf.html

Go:   // 手写递归
来源：http://hz.chenlongwang.top/gtzknsdcup.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gotoacloud.top/gtxsypyesw.html

C#:   // 手写递归
来源：http://hz.pengpengdd.cyou/gtxvhlkmlm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zdqjudy.top/gtmnabwdiu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.havefunace.top/gtnprsqukw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangshuangyany.cn/gtmbuaxegd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtwdrvaxih.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gttdcpmguc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangdashe.top/gtjhwtcewt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgufenzy.top/gtbgfajfew.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daxiang520.top/gtdbspbhjo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gttfcltblh.html

================================================================================
来源：http://hz.ydjk.org.cn/gtlduwrjkv.html

O. 并发与异步
来源：http://hz.fengsongda.top/gtznifxudg.html

================================================================================
来源：http://hz.zhengqikj.top/gtgvqkzgko.html

[O01] 启动一个线程
来源：http://hz.gzhubu.top/gttpwduafy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.pycfn.com/gtyrcstfpf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tian-w.cn/gtofxfxdzr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinqigufen.top/gtdkigubti.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtqvodkpur.html

Java: new Thread(() -> f()).start()
来源：http://hz.yongpay.top/gtyrkkpqrc.html

Go:   go f()
来源：http://hz.yuanzhike.top/gtyzbnlkfg.html

Ruby: Thread.new { f }
来源：http://hz.yongpay.top/gtkdmaxjwp.html

C#:   Task.Run(() => F());
来源：http://hz.wangdashe.top/gtrrilucna.html

[O02] 使用线程池
来源：http://hz.hongshengwenyu.top/gtaneywptg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yueranfly.top/gtjadjbgxp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zycfv.cn/gtfaizurpg.html

JS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gtjslzlzye.html

TS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtsfqgiphp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.meibo888.top/gtannehczz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shuidangran.top/gtqwxhfrxf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gogol.net.cn/gtyhjbcelr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hnqzz.top/gtgnzwqdpn.html

[O03] 加锁保护共享数据
来源：http://hz.ehwqpu.com/gtntfzdshg.html

Py:   with lock: shared += 1
来源：http://hz.cqqwz.cn/gtyhqgilib.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cdnleiting.top/gtxzkjlnvr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shzxlz.cn/gtgixhvkuq.html

TS:   // 同 JS
来源：http://hz.316326.xyz/gtnywcnvjo.html

Java: synchronized (this) { shared++; }
来源：http://hz.gotoacloud.top/gtoeskofbp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yanxiufei.cn/gtvdlugjbp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cheryme.top/gtsvoepwrh.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhoulong.xyz/gtqlbufpmj.html

[O04] 定义异步函数并等待
来源：http://hz.hammf.cn/gtjljrfslg.html

Py:   async def f():⏎    await g()
来源：http://hz.xuetiantiany.cn/gtkcrsvspa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gaohongyu789.top/gtodeeemah.html

JS:   async function f() { await g(); }
来源：http://hz.gogol.net.cn/gtuncwlfif.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhoulong.xyz/gtifnzbazn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhixingplan.top/gthquscwnw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuanzhike.top/gtuidnphfc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dashuyun.cn/gtpnikfnrx.html

C#:   async Task F() { await G(); }
来源：http://hz.yongpay.top/gttjfpzxna.html

[O05] 并发执行并等待全部完成
来源：http://hz.jlsjyb.cn/gtjdzfisyb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhaomingkeji.xyz/gtigjrpgru.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.meibo888.top/gtvmkbeoro.html

JS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtisswognt.html

TS:   await Promise.all(tasks)
来源：http://hz.haohaochexian.top/gtqfzfdgym.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhongyouzk.top/gtafmsspay.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhiwuduotai.top/gtschglxvq.html

Ruby: threads.map(&:join)
来源：http://hz.yanxiufei.cn/gtposmjcqj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhixingplan.top/gtcthyrquc.html

[O06] 使用进程池
来源：http://hz.shuidangran.top/gtteijfnza.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jlsjyb.cn/gtjxfilans.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.quarkkingdee.top/gtallxizgx.html

JS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gthzwqbqhh.html

TS:   // child_process / cluster 模块
来源：http://hz.xingfuxueyuan.xyz/gttvcjnlol.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xuetiantiany.cn/gtsjozzfva.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258.top/gtpslqwkmn.html

Ruby: // fork 块
来源：http://hz.jiagoushi.top/gtnyfaqeci.html

C#:   Parallel.For
来源：http://hz.gotoacloud.top/gtfdnydpgg.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtvsrkqrvl.html

P. 常用工具函数
来源：http://hz.aibaodan.cn/gtvsvbqiih.html

================================================================================
来源：http://hz.pycfn.com/gtmfmbpjac.html

[P01] 生成 UUID
来源：http://hz.yanxiufei.cn/gtiiiopikx.html

Py:   str(uuid.uuid4())
来源：http://hz.hfpthk.cn/gtsveekyxe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.redwolf501.top/gtaoolzred.html

JS:   crypto.randomUUID()
来源：http://hz.52xcode.cn/gtayoozslo.html

TS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gthnzceidf.html

Java: UUID.randomUUID().toString()
来源：http://hz.gogol.net.cn/gtfcooneqr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.wangdashe.top/gtalbfomuj.html

Ruby: SecureRandom.uuid
来源：http://hz.jinyuanbaomall.cn/gtvazarhpo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yanxiufei.cn/gtvqesuajj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gtjbauzkdo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.fengsongda.top/gtqfxekyjc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.guowangkeji.top/gtbgieohvj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yonumen.top/gtpblvtcwb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yanxiufei.cn/gtdwdvuykr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yvedp.cn/gtmwncahbz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydzc1.top/gtacatqbre.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hongshengwenyu.top/gtvaznltxi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.meibo888.top/gtquulddjn.html

[P03] 生成短随机字符串
来源：http://hz.gotoacloud.top/gtetibxasd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xziqi.cn/gtrjzmszhs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yongpay.top/gtjimthlve.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.snrcjt.cn/gtjfuuyfcf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.mhx1999.top/gtrygmrkrt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gotoacloud.top/gtmljeahtd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nwbrower.top/gtbkqqtftr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yangfankeji.com/gtehrppkqm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ivvv.top/gtpppcmgyr.html

[P04] 求长度
来源：http://hz.nanxuanxn.top/gtrwshtcop.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zdqjudy.top/gtougywnbv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtxdlfnajn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gtestnoudy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gogol.net.cn/gtsgdhwwhq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sweek.top/gtalnzpkgi.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258888.top/gtlajxzdru.html

Ruby: x.length;  x.size
来源：http://hz.ehwqpu.com/gtwhgoxtax.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hammf.cn/gtopdeuats.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gzhubu.top/gtcsccgjky.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydzc1.top/gtxhrxvwvf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yueranfly.top/gtqercwnjm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shanyushiyangtech.top/gtfseeozfb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zycfv.cn/gtqkgnthcp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yanxiufei.cn/gtdtvidina.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.feifeiyinyue.top/gtmvabfqzy.html

Ruby: a == b
来源：http://hz.yueranfly.top/gtjwhhbkmh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nanxuanxn.top/gtzzmujfpx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xingfuxueyuan.xyz/gtobcifkqd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.smart0.xyz/gttmpedkep.html

PHP:  if (empty($x)) {}
来源：http://hz.tianlin.xyz/gtvecbenng.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.snrcjt.cn/gttidkckpy.html

TS:   if (x == null) {}
来源：http://hz.pycfn.com/gtlbdjywvy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cdnleiting.top/gtpiwtfpyp.html

Go:   if x == nil {}
来源：http://hz.feifeiyinyue.top/gtvnbtxzwc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ybcxt.top/gtoprokzco.html

C#:   if (x is null) {}
来源：http://hz.feifeiyinyue.top/gtptkccfnf.html

[P07] 防抖与节流
来源：http://hz.jianghu66.top/gtitrhtnnn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.smart0.xyz/gtfbbkrson.html

PHP:  // 手写时间戳比较
来源：http://hz.9152youxi.cn/gtmjshgsea.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtgmrtekya.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gteyttjczt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yongpay.top/gtcmdubbus.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.haohaochexian.top/gtvabjjrcm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xylfe.cn/gtkehanzqx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.aibaodan.cn/gtigfiejvy.html

[P08] 处理浮点精度问题
来源：http://hz.svipenyu.cn/gtgnvmopex.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.meibo888.top/gtmfqxiglg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.316326.xyz/gtbfovbbsb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.meibo888.top/gthidbcedt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinqigufen.top/gtuhdztzga.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenzaomai.com/gtyydzpfde.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xinyue.icu/gtseilmrey.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinqigfzy.top/gtydxnqytk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.meibo888.top/gtdnyzqcsq.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtxhgcjktw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jyoumei.cn/gtsfvzqxoe.html

================================================================================
来源：http://hz.zhijiandao.cn/gtjlozdsjs.html

[Q01] 创建表
来源：http://hz.zhongyouzk.top/gtdarnokes.html

CREATE TABLE users (
来源：http://hz.hammf.cn/gtaxlfvunf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.meibo888.top/gtoluwnlhe.html

name VARCHAR(50) NOT NULL,
来源：http://hz.havefunace.top/gtdqefmmny.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ybcxt.top/gtaxxuifns.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigufen.top/gthvxhmapd.html

);
来源：http://hz.cucudq.cn/gtvowtuopf.html

[Q02] 创建带外键的表
来源：http://hz.redwolf501.top/gtvyvsscik.html

CREATE TABLE orders (
来源：http://hz.jinghuilouyu.cn/gtldgxdrzn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtwcxfsdbg.html

user_id INT NOT NULL,
来源：http://hz.pycfn.com/gtputdgesv.html

amount DECIMAL(10, 2),
来源：http://hz.ppjwa.cn/gtwizdbnbl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuanzhike.top/gttwyonmgp.html


<!-- 参考信息 -->