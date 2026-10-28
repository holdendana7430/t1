代发 wailian999

[M04] 获取当前工作目录
来源：http://hz.gogol.net.cn/gtnktcnuaw.html

Py:   os.getcwd()
来源：http://hz.jinyuanbaomall.cn/gtwrnlyyli.html

PHP:  getcwd();
来源：http://hz.hnxiangtu.top/gtczdswycf.html

JS:   process.cwd()
来源：http://hz.yangfankeji.com/gtqsmlpvvs.html

TS:   process.cwd()
来源：http://hz.snrcjt.cn/gtphokhokl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gthipjxyaa.html

Go:   os.Getwd()
来源：http://hz.gaohongyu789.top/gtqqgsobli.html

Ruby: Dir.pwd
来源：http://hz.hongshengwenyu.top/gtibpujvwv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxuanxn.top/gtpwrsjkjd.html

[M05] 设置退出码
来源：http://hz.aizwys.cn/gtjkcxsxnh.html

Py:   sys.exit(1)
来源：http://hz.ehwqpu.com/gtxpujbwnz.html

PHP:  exit(1);
来源：http://hz.cucudq.cn/gtdgfaqhyg.html

JS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtymickbsp.html

TS:   process.exit(1)
来源：http://hz.ppjwa.cn/gtbumbcakw.html

Java: System.exit(1)
来源：http://hz.havefunace.top/gtzonhyybn.html

Go:   os.Exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtnxjbauex.html

Ruby: exit 1
来源：http://hz.kuanghao11.cn/gtcijumubt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.aizwys.cn/gtfunvqnnb.html

[M06] 向标准错误输出
来源：http://hz.xuetiantiany.cn/gtmteqylxq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.snrcjt.cn/gtiqycnlds.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hongshengwenyu.top/gtcphhzaoj.html

JS:   console.error("err")
来源：http://hz.tanke756.top/gtybccegzm.html

TS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtztpswjuy.html

Java: System.err.println("err")
来源：http://hz.sufxvd.cn/gtzfbgihyr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.kuanghao11.cn/gtmvvsvljb.html

Ruby: warn "err"
来源：http://hz.jianghu66.top/gtanatntzj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.316326.xyz/gtjknroxar.html

[M07] 判断是否为主入口
来源：http://hz.yvedp.cn/gtprnacpot.html

Py:   if __name__ == "__main__":
来源：http://hz.dianchejie.cn/gtnnonxzub.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtdhvpslsn.html

JS:   require.main === module
来源：http://hz.andypj.xyz/gtixikrwwx.html

TS:   require.main === module
来源：http://hz.shzxlz.cn/gtlakebmkx.html

Java: public static void main(String[] args)
来源：http://hz.cucudq.cn/gtivqwpvos.html

Go:   func main()
来源：http://hz.shangyingyoupin.top/gtsmrlflhi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.52xcode.cn/gtvjdhinom.html

C#:   static void Main(string[] args)
来源：http://hz.fengsongda.top/gtsihxkfuk.html

[M08] 获取系统与运行时信息
来源：http://hz.shangyingyoupin.top/gtwsomdptb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hfpthk.cn/gtvlkqgmct.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.iojbl.cn/gtbhoaitex.html

JS:   process.platform;  process.version
来源：http://hz.ydjk.org.cn/gtyrsyduqd.html

TS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gtbkezilrn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tanke756.top/gtytwwrdyx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hywenlv.cn/gtedlkbqmc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yongpay.top/gtzfzxrony.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ywan-chungtsiang.top/gtxsnkpihh.html

================================================================================
来源：http://hz.ivvv.top/gtwvryavzv.html

N. 数据结构与算法
来源：http://hz.sweek.top/gtfbxjeyev.html

================================================================================
来源：http://hz.jyoumei.cn/gtwnqocvna.html

[N01] 二分查找（有序数组）
来源：http://hz.daria6918.cn/gttmgcuwhv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.wangdashe.top/gtdfwgkgle.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cashguo.top/gtorfjjjpj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtaodpktit.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtfezpgnmh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.svipenyu.cn/gteayqylia.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.pengpengdd.cyou/gtnewazuho.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zdqjudy.top/gtpwtmaday.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtvxbnsvsy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zycfv.cn/gtvkajmcac.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtcjfvacqf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shangyingyoupin.top/gtidtsgxmh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtwxucbhin.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtlxfdnodz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shangyingyoupin.top/gttcpkhwof.html

Go:   slices.Sort(arr)
来源：http://hz.ivvv.top/gtvlzkwuko.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtvdxmypgs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangdashe.top/gtpeffhmrn.html

[N03] 快速排序（分治示例）
来源：http://hz.xziqi.cn/gtzugpwahq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.meibo888.top/gtxjkmvruj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.smart0.xyz/gtxkspqzbw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gtpeskjpom.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtoditkyan.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xinyue.icu/gtssyonvew.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.dashuyun.cn/gtdmuyrpdj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenzaomai.com/gtyvswsrhk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shanyushiyangkeji.top/gtuulniqwp.html

[N04] 斐波那契数列
来源：http://hz.sufxvd.cn/gtprebjjvv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtyphtuubs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenzaomai.com/gtlbpovwfe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtkqlkpicx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhongyouzk.top/gtvstlyquw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtgeekzreh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jiagoushi.top/gtekcsvgdk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.haohaochexian.top/gttmpqxsqp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258888.top/gtxtzworhg.html

[N05] 最大公约数
来源：http://hz.316326.xyz/gtjctxwmxb.html

Py:   math.gcd(a, b)
来源：http://hz.xziqi.cn/gtsaiemviw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fengsongda.top/gtarthxjrf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtaoqslykx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtylevteau.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.52xcode.cn/gtzsppzfig.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.andypj.xyz/gtcachqyzp.html

Ruby: a.gcd(b)
来源：http://hz.cucudq.cn/gtjxuynivv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cheryme.top/gtrcsocpbs.html

[N06] 判断回文字符串
来源：http://hz.aizwys.cn/gtltnkdthp.html

Py:   s == s[::-1]
来源：http://hz.nwbrower.top/gtdtifrpje.html

PHP:  $s === strrev($s);
来源：http://hz.shzxlz.cn/gtscoqypqr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtzhmfcngq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtwgvscxfv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hnxiangtu.top/gtuyccisol.html

Go:   // 双指针从两端比较
来源：http://hz.hongshengwenyu.top/gtagsmfitm.html

Ruby: s == s.reverse
来源：http://hz.zhijiandao.cn/gtfydgmvow.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gtliqmydyd.html

[N07] 两数之和（返回下标）
来源：http://hz.jianghu66.top/gtwwgwcodf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cheryme.top/gtjtuzqwsp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.daxiang520.top/gtdqbolajk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydjk.org.cn/gtqiotltur.html

TS:   // 手写 Map<string, number>
来源：http://hz.ivvv.top/gtndylwxyd.html

Java: // 手写 HashMap
来源：http://hz.svipenyu.cn/gtltervorl.html

Go:   // 手写 map[int]int
来源：http://hz.0kj1m.cn/gtdslqxaic.html

Ruby: // 手写 Hash
来源：http://hz.aizwys.cn/gtzmxkfipw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zdqjudy.top/gtabmpckks.html

[N08] 生成全排列
来源：http://hz.feifeiyinyue.top/gtlauvxjep.html

Py:   itertools.permutations(arr)
来源：http://hz.316326.xyz/gtqdaqmxot.html

PHP:  // 手写递归交换
来源：http://hz.dashuyun.cn/gtecuvkgce.html

JS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtiutqvyew.html

TS:   // 手写回溯递归
来源：http://hz.ivvv.top/gthmipplsv.html

Java: // 手写回溯递归
来源：http://hz.ydzc1.top/gtckutwknf.html

Go:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtigbdegrh.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gthutrydli.html

C#:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtqghxhrau.html

[N09] 栈与队列
来源：http://hz.hysaishi.cn/gtabwblbnb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xziqi.cn/gtkvfeyzof.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hywenlv.cn/gtyazwydie.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.9152youxi.cn/gtzvlkmxzt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.guowangkeji.top/gtwzgotdxv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ehwqpu.com/gtrrheyceb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zdqjudy.top/gteqhxecgd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtptipleym.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yonumen.top/gtnfsdybpt.html

[N10] 链表节点定义
来源：http://hz.shzxlz.cn/gtwfwipicx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cucudq.cn/gtxlvhnuqq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtnjnlsbis.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gotoacloud.top/gtviiqrbtq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ybcxt.top/gtlmfiobjz.html

Java: class Node { int v; Node next; }
来源：http://hz.c1oappe.top/gtjtedseff.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cqqwz.cn/gtjymvwxzo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuanzx.com/gtqxdwdfbn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnqzz.top/gtcxugjuhd.html

[N11] 二叉树中序遍历
来源：http://hz.pengpengdd.cyou/gtgydpnfob.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gotoacloud.top/gtwvkcngja.html

PHP:  // 手写递归函数
来源：http://hz.nanxinkj.top/gthnqmsrqe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtxlsyftrd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtgarnabco.html

Java: // 手写递归
来源：http://hz.yanxiufei.cn/gtadqfdywt.html

Go:   // 手写递归
来源：http://hz.nwbrower.top/gtnbjocvmg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.svipenyu.cn/gtvcqymhko.html

C#:   // 手写递归
来源：http://hz.cqqwz.cn/gteesysyyd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhijiandao.cn/gtjvaxrehd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shzxlz.cn/gtdirinail.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hongshengwenyu.top/gtuflnyqoq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shuidangran.top/gtcuqidoja.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gtmpggipsh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtfktllhxv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yj202588.top/gtkiykvcdv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jyoumei.cn/gtjelfahzy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtofqmacid.html

================================================================================
来源：http://hz.yuxming.cn/gtcccprbyj.html

O. 并发与异步
来源：http://hz.nwbrower.top/gtjxtngiiv.html

================================================================================
来源：http://hz.daxiang520.top/gtqqmoeytv.html

[O01] 启动一个线程
来源：http://hz.tanke756.top/gtwovazqql.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.aizwys.cn/gtuzrikdyf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gogol.net.cn/gthhubsvgz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinqigfzy.top/gtznrawmig.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gtvhdjarip.html

Java: new Thread(() -> f()).start()
来源：http://hz.hammf.cn/gtuxrvsvgr.html

Go:   go f()
来源：http://hz.hysaishi.cn/gtcpjpdkkx.html

Ruby: Thread.new { f }
来源：http://hz.hnxiangtu.top/gtkhmmpdov.html

C#:   Task.Run(() => F());
来源：http://hz.zhiwuduotai.top/gtbenlbzsh.html

[O02] 使用线程池
来源：http://hz.gaohongyu789.top/gtfqstsnmw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cdnleiting.top/gtjkaqlxag.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cashguo.top/gtkjmkqkip.html

JS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtojqlwfru.html

TS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gtkgeolumy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ppjwa.cn/gtglkxgtwv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yuanzhike.top/gtrfmqreee.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gotoacloud.top/gtmuwmgiqw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jiagoushi.top/gtfgqjognw.html

[O03] 加锁保护共享数据
来源：http://hz.yanxiufei.cn/gtvzmtvisd.html

Py:   with lock: shared += 1
来源：http://hz.gaohongyu789.top/gtfhnwboep.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yuanzhike.top/gtbbozumer.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xuetiantiany.cn/gtvhyzhhbs.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtghldjetu.html

Java: synchronized (this) { shared++; }
来源：http://hz.fengsongda.top/gtefyyxmjc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.feifeiyinyue.top/gtwatzodmr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhixingplan.top/gttevurwem.html

C#:   lock (gate) { shared++; }
来源：http://hz.cucudq.cn/gtycisgaup.html

[O04] 定义异步函数并等待
来源：http://hz.shangyingyoupin.top/gtcdhznsfm.html

Py:   async def f():⏎    await g()
来源：http://hz.gogol.net.cn/gtgcjkvlnr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuanzhike.top/gtrnyyocqq.html

JS:   async function f() { await g(); }
来源：http://hz.ydzc1.top/gtjissruan.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shzxlz.cn/gtrytrxpuy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sysykeji.top/gtylanxmyq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.birdmap.top/gturdtrdnm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.haohaochexian.top/gttwmqejrd.html

C#:   async Task F() { await G(); }
来源：http://hz.zhongyouzk.top/gtodsbmuum.html

[O05] 并发执行并等待全部完成
来源：http://hz.sysykeji.top/gtxqjoultm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.52xcode.cn/gtxmpkivhl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sysykeji.top/gtilrzonym.html

JS:   await Promise.all(tasks)
来源：http://hz.xziqi.cn/gtuontpoxf.html

TS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gthzorpidz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhixingplan.top/gtkljrlrud.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj20258.top/gtpbqnqxkv.html

Ruby: threads.map(&:join)
来源：http://hz.chenjidiqi.icu/gtpytwmyxm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.52xcode.cn/gthrocutxp.html

[O06] 使用进程池
来源：http://hz.yuanzhike.top/gttqoguhpp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.316326.xyz/gtckkuyivt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.iojbl.cn/gtucblaogs.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxuanxn.top/gtoarmbitt.html

TS:   // child_process / cluster 模块
来源：http://hz.hongshengwenyu.top/gtasyrrsxk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgufenzy.top/gtzsavcnis.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xinyue.icu/gtxynybmso.html

Ruby: // fork 块
来源：http://hz.yj20258.top/gtiiellbly.html

C#:   Parallel.For
来源：http://hz.pycfn.com/gtgidorkmu.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtpxavdlzc.html

P. 常用工具函数
来源：http://hz.hywenlv.cn/gtfniijvia.html

================================================================================
来源：http://hz.xinyue.icu/gtrvlqwbab.html

[P01] 生成 UUID
来源：http://hz.gogol.net.cn/gtjihedplh.html

Py:   str(uuid.uuid4())
来源：http://hz.dianchejie.cn/gtrqebfkda.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.quarkkingdee.top/gtzrsfdlut.html

JS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtqlxttoqg.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtekmtduho.html

Java: UUID.randomUUID().toString()
来源：http://hz.yonumen.top/gtcktnswpu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hongshengwenyu.top/gtusxxppqq.html

Ruby: SecureRandom.uuid
来源：http://hz.nanxinkj.top/gtdyniellf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dashuyun.cn/gtsvqbzkay.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jianghu66.top/gtwkgtohub.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yvedp.cn/gtpjdxyzxk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zdqjudy.top/gtrjurjmes.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangtech.top/gtzhidvfaa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jianghu66.top/gtaossahls.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ywan-chungtsiang.top/gtpniwhtfk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.meibo888.top/gtthrjxejf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xylfe.cn/gtsxknrnwn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hywenlv.cn/gtpkruftie.html

[P03] 生成短随机字符串
来源：http://hz.yj20258.top/gtgusxphcp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.havefunace.top/gthqhosaiq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hysaishi.cn/gtazmuqnyg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gtctcvjsoe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.quarkkingdee.top/gthhelgcfx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sysykeji.top/gtrolrdgzx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shangyingyoupin.top/gterqkozpi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhaomingkeji.xyz/gtyzmhkxcm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinyuanbaomall.cn/gthvpfgfob.html

[P04] 求长度
来源：http://hz.yvedp.cn/gtjiexbonz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jyoumei.cn/gtsbeexhnj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtqoujqqvw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtldbzhgja.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtwgnubcdx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hongshengwenyu.top/gthpgnbmbw.html

Go:   len(arr);  len(m)
来源：http://hz.wangshuangyany.cn/gttmxheckk.html

Ruby: x.length;  x.size
来源：http://hz.hnqzz.top/gteqzxtzqn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cheryme.top/gtxeupfrdg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj20258888.top/gtdfwpnwib.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.smart0.xyz/gtwwnkafvw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ybcxt.top/gtufqqxxmm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.52xcode.cn/gtgddedfcd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cashguo.top/gtenwklcxr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenzaomai.com/gtrjuzomiv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yangfankeji.com/gtcifqrret.html

Ruby: a == b
来源：http://hz.jinyuanbaomall.cn/gtwvqzfsuy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ywan-chungtsiang.top/gtsoejwdrv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhiwuduotai.top/gtevsllwvv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jlsjyb.cn/gtymsybuao.html

PHP:  if (empty($x)) {}
来源：http://hz.ybcxt.top/gtntznnlwj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhengqikj.top/gtashzpwxn.html

TS:   if (x == null) {}
来源：http://hz.yongpay.top/gtnthioylw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daxiang520.top/gtfmfqquxu.html

Go:   if x == nil {}
来源：http://hz.hywenlv.cn/gtxkuegjcs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aizwys.cn/gtoxbveblb.html

C#:   if (x is null) {}
来源：http://hz.tian-w.cn/gthenkxvca.html

[P07] 防抖与节流
来源：http://hz.jinghuilouyu.cn/gtgyudfuqo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.guannengcc.top/gtarkjcdfd.html

PHP:  // 手写时间戳比较
来源：http://hz.smart0.xyz/gtqvwpbnpm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gthtkdgpaa.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guannengcc.top/gtkvdfjafh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pengpengdd.cyou/gtcqeworyp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xziqi.cn/gtibnjvagk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hongshengwenyu.top/gtjjbvteig.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ydjk.org.cn/gtabewyvhr.html

[P08] 处理浮点精度问题
来源：http://hz.ehwqpu.com/gtganosnep.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cucudq.cn/gtkpfpotqp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gzhubu.top/gtfilpvhdv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tian-w.cn/gtekmkkqjo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cashguo.top/gtmlhqnotb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinyuanbaomall.cn/gtvrqwgnhv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hywenlv.cn/gtmhpnwecs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhaomingkeji.xyz/gtpzjnvpny.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zycfv.cn/gtjnnrkckp.html

================================================================================
来源：http://hz.redwolf501.top/gtsscioowf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinyuanbaomall.cn/gtqjmyejzf.html

================================================================================
来源：http://hz.hfpthk.cn/gtujjzjzjj.html

[Q01] 创建表
来源：http://hz.havefunace.top/gthhfgvpco.html

CREATE TABLE users (
来源：http://hz.zycfv.cn/gtlhgehhvz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gtueobgjlh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.haohaochexian.top/gtnzeyqxdg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yuanzhike.top/gtmvdedysm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.kuanghao11.cn/gttuzxdjzk.html

);
来源：http://hz.haohaochexian.top/gtytxdlwgh.html

[Q02] 创建带外键的表
来源：http://hz.gzhubu.top/gthvjozpbm.html

CREATE TABLE orders (
来源：http://hz.xingfuxueyuan.xyz/gtnjlwhyyv.html


<!-- 参考信息 -->