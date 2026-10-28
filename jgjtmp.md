代发 wailian999

TS:   process.cwd()
来源：http://hz.zycfv.cn/gtcppxvdek.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yangfankeji.com/gtnafxvybd.html

Go:   os.Getwd()
来源：http://hz.nanxuanxn.top/gtrgebxmme.html

Ruby: Dir.pwd
来源：http://hz.zhongyouzk.top/gtjecoxuda.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.aibaodan.cn/gtbfypxeqb.html

[M05] 设置退出码
来源：http://hz.sxryk.cn/gtpsvscluj.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangtech.top/gtsuzzfzal.html

PHP:  exit(1);
来源：http://hz.yvedp.cn/gteeusuwiq.html

JS:   process.exit(1)
来源：http://hz.daxiang520.top/gtaitnrkad.html

TS:   process.exit(1)
来源：http://hz.52xcode.cn/gtsctzksap.html

Java: System.exit(1)
来源：http://hz.gotoacloud.top/gtoxtdyhxj.html

Go:   os.Exit(1)
来源：http://hz.aizwys.cn/gtkgytfhcc.html

Ruby: exit 1
来源：http://hz.hywenlv.cn/gtecazbtjn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xuanzx.com/gtytijokow.html

[M06] 向标准错误输出
来源：http://hz.316326.xyz/gttuoyrqzd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinghuilouyu.cn/gtyutvsczw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sufxvd.cn/gtrbsbrims.html

JS:   console.error("err")
来源：http://hz.daria6918.cn/gtrmjcjxeb.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gtxrriglle.html

Java: System.err.println("err")
来源：http://hz.hnxiangtu.top/gtohauxxyx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yangfankeji.com/gtkrzlkvbz.html

Ruby: warn "err"
来源：http://hz.nanxuanxn.top/gtaqunmflp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cdnleiting.top/gtvkvtkgpd.html

[M07] 判断是否为主入口
来源：http://hz.pengpengdd.cyou/gtrtfpavfz.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258888.top/gtbmvqucqy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shangyingyoupin.top/gtocosnbfk.html

JS:   require.main === module
来源：http://hz.zhixingplan.top/gtxjbnvvny.html

TS:   require.main === module
来源：http://hz.cheryme.top/gtiatenpkb.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtxiszoolv.html

Go:   func main()
来源：http://hz.hfpthk.cn/gtlhqsjlwd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zycfv.cn/gtpbfwleal.html

C#:   static void Main(string[] args)
来源：http://hz.shuidangran.top/gtuguosfvd.html

[M08] 获取系统与运行时信息
来源：http://hz.xuetiantiany.cn/gtftghssor.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sysykeji.top/gtgykozhtg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.wangshuangyany.cn/gtvaluikcv.html

JS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtaujfbykw.html

TS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtwrbibupb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xylfe.cn/gtvtusncap.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.birdmap.top/gtyxppppmu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinyuanbaomall.cn/gtczgxjzta.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dashuyun.cn/gtvkljqhes.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtspigqgxq.html

N. 数据结构与算法
来源：http://hz.xylfe.cn/gtjrukjked.html

================================================================================
来源：http://hz.yj202588.top/gtbrvtokqe.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxinkj.top/gttisthidm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gzhubu.top/gteaxgqgfd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.quarkkingdee.top/gtniggvbvb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtiobrbear.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuetiantiany.cn/gtxdrzcqwe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.havefunace.top/gttmrirjwi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.redwolf501.top/gthkerpsvd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tian-w.cn/gtvnbvdmdo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yangfankeji.com/gtdovpngff.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gzhubu.top/gtwiixzlnp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtftlbtfeq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.iojbl.cn/gtbjfdfawz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtgzlmlamp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pengpengdd.cyou/gteertmocr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cheryme.top/gtwvryjhfn.html

Go:   slices.Sort(arr)
来源：http://hz.pengpengdd.cyou/gtfcejlrne.html

Ruby: arr.sort
来源：http://hz.bjfxy.top/gtotfitpgl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jyoumei.cn/gtivtzfyvp.html

[N03] 快速排序（分治示例）
来源：http://hz.tianlin.xyz/gtvclhnesd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jiagoushi.top/gtdnplexdc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuanzx.com/gtvfxuwzxi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtndupbway.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aibaodan.cn/gtvnnnghmu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fzhhl.top/gtfgrtsylg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pycfn.com/gtjbxrdrmm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.fzhhl.top/gtbtmjjqts.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgfzy.top/gthuspxuie.html

[N04] 斐波那契数列
来源：http://hz.fzhhl.top/gtapelwzlz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yanxiufei.cn/gtbhluypsr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cashguo.top/gtkxjyqhsn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gtfblhfmjg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhixingplan.top/gtqxgdskrk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gtxewgfclc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zdqjudy.top/gtznrugyga.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.daxiang520.top/gtqqvjgptq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nanxinkj.top/gtmirpthnl.html

[N05] 最大公约数
来源：http://hz.xingfuxueyuan.xyz/gtbybkiqmm.html

Py:   math.gcd(a, b)
来源：http://hz.pengpengdd.cyou/gtfczriudz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.kuanghao11.cn/gtuzsbmpyr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtgzrkmvzz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gteblynafo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xuanzx.com/gtftddtzzw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yueranfly.top/gtvlnuidyv.html

Ruby: a.gcd(b)
来源：http://hz.kuanghao11.cn/gtyoualapa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sysykeji.top/gtqjgduslm.html

[N06] 判断回文字符串
来源：http://hz.jqgufenzy.top/gtkofnqgbz.html

Py:   s == s[::-1]
来源：http://hz.cucudq.cn/gtppyskacd.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258.top/gtgkavxwqq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtueuwyvjm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtgfbxzode.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.haohaochexian.top/gtmdyfqybe.html

Go:   // 双指针从两端比较
来源：http://hz.tian-w.cn/gtfgznlxtv.html

Ruby: s == s.reverse
来源：http://hz.gogol.net.cn/gtttxsgeek.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.guannengcc.top/gtajyslvqy.html

[N07] 两数之和（返回下标）
来源：http://hz.shanyushiyangtech.top/gtbtpcxstt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhaomingkeji.xyz/gtmzrzqdxa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tianlin.xyz/gtjupaffgw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.meibo888.top/gtktpnupvh.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgfzy.top/gtclmijxif.html

Java: // 手写 HashMap
来源：http://hz.redwolf501.top/gtnioccmin.html

Go:   // 手写 map[int]int
来源：http://hz.yongpay.top/gtutsuyybc.html

Ruby: // 手写 Hash
来源：http://hz.daxiang520.top/gtyidmrzxw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtkybritef.html

[N08] 生成全排列
来源：http://hz.sweek.top/gtcgsgjicm.html

Py:   itertools.permutations(arr)
来源：http://hz.ivvv.top/gtclpsjpuv.html

PHP:  // 手写递归交换
来源：http://hz.xinyue.icu/gtvwpvkkox.html

JS:   // 手写回溯递归
来源：http://hz.hammf.cn/gtaagpzkww.html

TS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gthjtlmtey.html

Java: // 手写回溯递归
来源：http://hz.chenlongwang.top/gtmgsdofep.html

Go:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtorpeipfz.html

Ruby: arr.permutation.to_a
来源：http://hz.dashuyun.cn/gtdjfgqikm.html

C#:   // 手写回溯递归
来源：http://hz.sweek.top/gtkiozqccf.html

[N09] 栈与队列
来源：http://hz.ivvv.top/gtccdefkpy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ywan-chungtsiang.top/gtmiwkbxxx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tian-w.cn/gtnjhtmyqh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.0kj1m.cn/gteugxcblt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gtqejwlmlg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.feifeiyinyue.top/gtujfjidzw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tian-w.cn/gtgdqoxdag.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yueranfly.top/gtreuiuoez.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenjidiqi.icu/gtiebnvkur.html

[N10] 链表节点定义
来源：http://hz.yueranfly.top/gtvjiseseb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangkeji.top/gtugvapamw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jqgfzy.top/gtqllyvpqs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gaohongyu789.top/gtjoeqkucv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ywan-chungtsiang.top/gtdvfmnbjp.html

Java: class Node { int v; Node next; }
来源：http://hz.guowangkeji.top/gttheudryg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cqqwz.cn/gtutiewkve.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xziqi.cn/gtwxhlvudr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.9152youxi.cn/gtissqdxmb.html

[N11] 二叉树中序遍历
来源：http://hz.zhaomingkeji.xyz/gtwgibowyu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yj20258888.top/gtnptdbhht.html

PHP:  // 手写递归函数
来源：http://hz.fzhhl.top/gtpsdbuogi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gteppujhdt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenlongwang.top/gtwetcacad.html

Java: // 手写递归
来源：http://hz.chenzaomai.com/gtrzearfrz.html

Go:   // 手写递归
来源：http://hz.yongpay.top/gtyaxdymfz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ybcxt.top/gtpedrdpdf.html

C#:   // 手写递归
来源：http://hz.yj202588.top/gthnulkere.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.havefunace.top/gtohofvogi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yangfankeji.com/gtiadvnmjm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ybcxt.top/gttazagcjl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gtxhgxdxwh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gthmkcximk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gteedhyvuo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.9152youxi.cn/gtblejfwxl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yueranfly.top/gtszziyesc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ehwqpu.com/gtlreipacu.html

================================================================================
来源：http://hz.chenzaomai.com/gtlysozpep.html

O. 并发与异步
来源：http://hz.chenzaomai.com/gtpasrkzuz.html

================================================================================
来源：http://hz.xinyue.icu/gtzhbfuvcy.html

[O01] 启动一个线程
来源：http://hz.xuetiantiany.cn/gtfvktusma.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuetiantiany.cn/gtmhgjrtru.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhijiandao.cn/gtujtytzqt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shanyushiyangkeji.top/gtxomcgaeu.html

TS:   // 同 JS
来源：http://hz.nwbrower.top/gtbafrklcp.html

Java: new Thread(() -> f()).start()
来源：http://hz.cqqwz.cn/gteqqqiqrq.html

Go:   go f()
来源：http://hz.yvedp.cn/gtyphwfpbb.html

Ruby: Thread.new { f }
来源：http://hz.fzhhl.top/gtluzoqpuc.html

C#:   Task.Run(() => F());
来源：http://hz.nanxinkj.top/gtamtngpgd.html

[O02] 使用线程池
来源：http://hz.shzxlz.cn/gtfpnyzkxe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shanyushiyangtech.top/gtewvulsnu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hammf.cn/gtsbdtnxvg.html

JS:   // worker_threads 线程池
来源：http://hz.nanxinkj.top/gtpozizxuo.html

TS:   // worker_threads 线程池
来源：http://hz.shangyingyoupin.top/gttkodsebp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daria6918.cn/gtimmxapae.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sweek.top/gtjeuozbtt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tianlin.xyz/gttcnobmyq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shuidangran.top/gtnkjtgnua.html

[O03] 加锁保护共享数据
来源：http://hz.snrcjt.cn/gtjslmapmf.html

Py:   with lock: shared += 1
来源：http://hz.52xcode.cn/gtdpxddjvd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fengsongda.top/gtluesfglv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cheryme.top/gtdcczazja.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtoypevllg.html

Java: synchronized (this) { shared++; }
来源：http://hz.pycfn.com/gtrudlspsu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgfzy.top/gticiihfsi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.9152youxi.cn/gtwkepdgnz.html

C#:   lock (gate) { shared++; }
来源：http://hz.wangdashe.top/gtmmkwhrbb.html

[O04] 定义异步函数并等待
来源：http://hz.jqgufenzy.top/gtigwcpdhc.html

Py:   async def f():⏎    await g()
来源：http://hz.zdqjudy.top/gtcpygszjb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.smart0.xyz/gtqlubjljf.html

JS:   async function f() { await g(); }
来源：http://hz.sufxvd.cn/gtsvagsecz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yongpay.top/gtnwublmvk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.birdmap.top/gtmbofldhg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nwbrower.top/gtpuwrshic.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hongshengwenyu.top/gtugscvnai.html

C#:   async Task F() { await G(); }
来源：http://hz.xylfe.cn/gtcsraqrgj.html

[O05] 并发执行并等待全部完成
来源：http://hz.ehwqpu.com/gttpexcwel.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuxming.cn/gtjncfkyor.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shanyushiyangtech.top/gtxzukbuhb.html

JS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtzetnbcsm.html

TS:   await Promise.all(tasks)
来源：http://hz.zdqjudy.top/gtmvavptqd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.mhx1999.top/gtnzdgdjkx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nanxinkj.top/gtfutvqerb.html

Ruby: threads.map(&:join)
来源：http://hz.aibaodan.cn/gtskqsbdww.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.svipenyu.cn/gtlhtgesjf.html

[O06] 使用进程池
来源：http://hz.havefunace.top/gtupvtavny.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.birdmap.top/gttlrmtfvq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cashguo.top/gttkdkrchq.html

JS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gtsaamxwom.html

TS:   // child_process / cluster 模块
来源：http://hz.zhiwuduotai.top/gtrrvowwky.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xingfuxueyuan.xyz/gtgecrxjpr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhaomingkeji.xyz/gtillvykna.html

Ruby: // fork 块
来源：http://hz.c1oappe.top/gtdnqbtksn.html

C#:   Parallel.For
来源：http://hz.daxiang520.top/gtrfewburi.html

================================================================================
来源：http://hz.zhengqikj.top/gtzucremfo.html

P. 常用工具函数
来源：http://hz.zhongyouzk.top/gtrnovmgpi.html

================================================================================
来源：http://hz.yongpay.top/gtnmpxygms.html

[P01] 生成 UUID
来源：http://hz.cucudq.cn/gtawmqbssv.html

Py:   str(uuid.uuid4())
来源：http://hz.cashguo.top/gtuzlrxwws.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fzhhl.top/gtcbfvvzpz.html

JS:   crypto.randomUUID()
来源：http://hz.ydzc1.top/gtsalursbx.html

TS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtnrfbtdzs.html

Java: UUID.randomUUID().toString()
来源：http://hz.cqqwz.cn/gtdqayfhzu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hongshengwenyu.top/gtjcffifcg.html

Ruby: SecureRandom.uuid
来源：http://hz.zhaomingkeji.xyz/gtnyqcccur.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydjk.org.cn/gtllwxrxlq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yongpay.top/gtvvwgtvll.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xziqi.cn/gtxecwvpvn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangtech.top/gtbpmpnvnn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenzaomai.com/gtgifrgvvg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.snrcjt.cn/gtrfbqoyyx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgfzy.top/gtcbspbwxt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yanxiufei.cn/gtjosxsmac.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gzhubu.top/gtoxymxbcj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnqzz.top/gtqwogbuxy.html

[P03] 生成短随机字符串
来源：http://hz.jyoumei.cn/gtavvnqelj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sufxvd.cn/gtyopfklww.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gotoacloud.top/gttigjasmr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.smart0.xyz/gtqrznkwcv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhaomingkeji.xyz/gtntcpjlmn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jqgufenzy.top/gtvgedebet.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxinkj.top/gttjrpuvly.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jianghu66.top/gtdvrlpeab.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.havefunace.top/gtbmqdaahb.html

[P04] 求长度
来源：http://hz.gotoacloud.top/gthedxtwzu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sxryk.cn/gtntokbhnb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ehwqpu.com/gtqnqldegy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtxibbpcso.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtfsdzrxqp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtsexlsdiu.html

Go:   len(arr);  len(m)
来源：http://hz.hywenlv.cn/gtrncwuzjl.html

Ruby: x.length;  x.size
来源：http://hz.yj20258888.top/gtfsdeqvch.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cdnleiting.top/gtiqqiiwix.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daria6918.cn/gthzotlnxr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jiagoushi.top/gtyllmlirq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.c1oappe.top/gtmkgwecxm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxuanxn.top/gtphpwltsk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aizwys.cn/gtrllqpzzc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnqzz.top/gtymiftfuf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.feifeiyinyue.top/gtrmtnivxj.html

Ruby: a == b
来源：http://hz.quarkkingdee.top/gtfpvhklgp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guannengcc.top/gtwvgeqcwg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sufxvd.cn/gtutysyqoz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shzxlz.cn/gtwgjcjtvi.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangkeji.top/gtkakwdahf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shanyushiyangtech.top/gtgjctgdid.html

TS:   if (x == null) {}
来源：http://hz.ehwqpu.com/gttevfrggc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.pycfn.com/gthlfzygkz.html

Go:   if x == nil {}
来源：http://hz.hongshengwenyu.top/gtuamsjmxh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.snrcjt.cn/gtcbwfiglr.html

C#:   if (x is null) {}
来源：http://hz.tianlin.xyz/gtumydmprc.html

[P07] 防抖与节流
来源：http://hz.hywenlv.cn/gtwmqjblme.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.guowangkeji.top/gtkcyrutki.html

PHP:  // 手写时间戳比较
来源：http://hz.ydzc1.top/gtzonlkwux.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtnnwpbzwp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtfanulfqu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.9152youxi.cn/gtjoyjrfwf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ydjk.org.cn/gtnohmizwv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinyuanbaomall.cn/gtwozkatfd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.guowangkeji.top/gtpqucburs.html

[P08] 处理浮点精度问题
来源：http://hz.xuetiantiany.cn/gtkynmzrlr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.quarkkingdee.top/gtkmxlvkdw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtegigpesp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xziqi.cn/gtpmrbmtul.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fzhhl.top/gtgsbgkltt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.feifeiyinyue.top/gtcsoksfjq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.andypj.xyz/gtkoqvobui.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jqgfzy.top/gtcrcqtafk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxuanxn.top/gthomfxwzv.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtacgtryen.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.kuanghao11.cn/gtzxisuzib.html

================================================================================
来源：http://hz.sufxvd.cn/gtqjkxmrfv.html

[Q01] 创建表
来源：http://hz.birdmap.top/gtmsyeekpl.html

CREATE TABLE users (
来源：http://hz.yonumen.top/gtlclzehpf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhengqikj.top/gtqqykjust.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yuanzhike.top/gtxpuorrku.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cucudq.cn/gtteqcimcj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hysaishi.cn/gtlcviwnzs.html

);
来源：http://hz.ppjwa.cn/gtuknzmpan.html

[Q02] 创建带外键的表
来源：http://hz.zhaomingkeji.xyz/gtzptmwjnp.html

CREATE TABLE orders (
来源：http://hz.yanxiufei.cn/gtitilzexu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtofyqjnor.html

user_id INT NOT NULL,
来源：http://hz.gaohongyu789.top/gtbieinyiu.html

amount DECIMAL(10, 2),
来源：http://hz.yueranfly.top/gtnagigfec.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shuidangran.top/gtbirkgghx.html


<!-- 参考信息 -->