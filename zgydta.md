代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gtkrzvbuqz.html

Ruby: warn "err"
来源：http://hz.jyoumei.cn/gtwiodsdxs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangdashe.top/gtheeupakh.html

[M07] 判断是否为主入口
来源：http://hz.nwbrower.top/gtbggherte.html

Py:   if __name__ == "__main__":
来源：http://hz.daxiang520.top/gtztfdkkpy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aibaodan.cn/gtjizuvrmv.html

JS:   require.main === module
来源：http://hz.zycfv.cn/gtzxtztyyb.html

TS:   require.main === module
来源：http://hz.pycfn.com/gtminfahtv.html

Java: public static void main(String[] args)
来源：http://hz.sysykeji.top/gtfojbcjtg.html

Go:   func main()
来源：http://hz.316326.xyz/gtzmivaopg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ppjwa.cn/gtxcejshru.html

C#:   static void Main(string[] args)
来源：http://hz.shanyushiyangkeji.top/gtcjzszbxu.html

[M08] 获取系统与运行时信息
来源：http://hz.zhongyouzk.top/gtjebfmrfa.html

Py:   platform.system();  platform.python_version()
来源：http://hz.kuanghao11.cn/gtxuxnmzpd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.snrcjt.cn/gtitypplwn.html

JS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtlbapbsrn.html

TS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtcvvpluhy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ydzc1.top/gtenooovyr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.vqdsnc.cn/gtylwsiiyo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ppjwa.cn/gtqstendey.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.aibaodan.cn/gtencgxsoa.html

================================================================================
来源：http://hz.sxryk.cn/gtglkzrixg.html

N. 数据结构与算法
来源：http://hz.ywan-chungtsiang.top/gtqvittgyf.html

================================================================================
来源：http://hz.zhengqikj.top/gtwewvkirq.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtktbpdbym.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nwbrower.top/gtcpvpojgx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yonumen.top/gtfgwjocaz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtvzfyysvv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ivvv.top/gtsqewvvyp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtrmkyijfi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.snrcjt.cn/gtdnstvjvq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jyoumei.cn/gtjqixtgew.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtklqpdeis.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aibaodan.cn/gtdtmlaknc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ybcxt.top/gtumvsqakw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guowangkeji.top/gtgglzdsvs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtcocufuxq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gtlzygxfyb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xuanzx.com/gttrbpzjkh.html

Go:   slices.Sort(arr)
来源：http://hz.havefunace.top/gtrdtrrixr.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtpbbobaou.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.vqdsnc.cn/gtesomkixx.html

[N03] 快速排序（分治示例）
来源：http://hz.zhongyouzk.top/gtzoziehzu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.havefunace.top/gtnaqaqogv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.svipenyu.cn/gtrmctxzop.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtgkuccvtx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtksffohxc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jiagoushi.top/gttfmmzssz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxuanxn.top/gtmehtijkk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.kuanghao11.cn/gtsjchxkdx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtspukgsub.html

[N04] 斐波那契数列
来源：http://hz.tanke756.top/gthhlsknlw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtvzkvvicx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.9152youxi.cn/gtazcpupfw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtkkzfmcki.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhoulong.xyz/gtdhzpulnd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tianlin.xyz/gtufosicnm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hywenlv.cn/gtkjksffsl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtpohroguj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daria6918.cn/gtseakogfb.html

[N05] 最大公约数
来源：http://hz.zhoulong.xyz/gtnrvjcnnt.html

Py:   math.gcd(a, b)
来源：http://hz.sxryk.cn/gtbmscdqjg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhaomingkeji.xyz/gtgtahjzfc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sweek.top/gtmpmvkplk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gtupnmspwy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guannengcc.top/gtnxxnindz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hfpthk.cn/gtfdrnqfge.html

Ruby: a.gcd(b)
来源：http://hz.ydjk.org.cn/gtporhvgpp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shzxlz.cn/gtkmxtsxwl.html

[N06] 判断回文字符串
来源：http://hz.havefunace.top/gtwlnpuvlz.html

Py:   s == s[::-1]
来源：http://hz.hfpthk.cn/gtjtrxqzfc.html

PHP:  $s === strrev($s);
来源：http://hz.sxryk.cn/gtraoxyxfl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtuqfjgohg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtclxikmli.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.smart0.xyz/gtbubdzpbk.html

Go:   // 双指针从两端比较
来源：http://hz.chenzaomai.com/gtyqsydpkf.html

Ruby: s == s.reverse
来源：http://hz.svipenyu.cn/gthdbgpiei.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtyderpjyb.html

[N07] 两数之和（返回下标）
来源：http://hz.xuanzx.com/gtfchtebuf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cheryme.top/gtgzohghnr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jyoumei.cn/gtefsascld.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuetiantiany.cn/gtiksrkfgz.html

TS:   // 手写 Map<string, number>
来源：http://hz.guannengcc.top/gthzuwrkmf.html

Java: // 手写 HashMap
来源：http://hz.xinyue.icu/gtcxjmwyso.html

Go:   // 手写 map[int]int
来源：http://hz.chenzaomai.com/gtdcwpjwwd.html

Ruby: // 手写 Hash
来源：http://hz.zycfv.cn/gtuyamydhi.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhengqikj.top/gtqvnatanb.html

[N08] 生成全排列
来源：http://hz.bjfxy.top/gtjhoxhkww.html

Py:   itertools.permutations(arr)
来源：http://hz.dashuyun.cn/gtsnktyuvc.html

PHP:  // 手写递归交换
来源：http://hz.ehwqpu.com/gtsahzfpmh.html

JS:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtvotjoaef.html

TS:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtpozytrnt.html

Java: // 手写回溯递归
来源：http://hz.gotoacloud.top/gtvdcdlqht.html

Go:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtbquwtzjb.html

Ruby: arr.permutation.to_a
来源：http://hz.chenjidiqi.icu/gttvdfylkn.html

C#:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtzspqifbr.html

[N09] 栈与队列
来源：http://hz.fengsongda.top/gttomeaski.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zdqjudy.top/gtfalujpcp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yangfankeji.com/gtywcbtbpd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gtqgqjiunh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gtculxvkzy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.0kj1m.cn/gtbaxjcvkj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.meibo888.top/gtductmyox.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xylfe.cn/gtykgocfoi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yonumen.top/gtdncqesed.html

[N10] 链表节点定义
来源：http://hz.ppjwa.cn/gtetjqdbup.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guannengcc.top/gtdtcgndcb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.svipenyu.cn/gtsrxyvjwg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zdqjudy.top/gtfmuejwig.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtfbnleaqn.html

Java: class Node { int v; Node next; }
来源：http://hz.0kj1m.cn/gtlbhmrxmk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.9152youxi.cn/gtzdvvpocf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.meibo888.top/gtfkddttlm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ydjk.org.cn/gtqpmsbsll.html

[N11] 二叉树中序遍历
来源：http://hz.jinghuilouyu.cn/gtudjvjpne.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.haohaochexian.top/gtigicjyft.html

PHP:  // 手写递归函数
来源：http://hz.yvedp.cn/gthnhlbgur.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nwbrower.top/gtgkncfewv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtutdarxke.html

Java: // 手写递归
来源：http://hz.jlsjyb.cn/gtwwkdixag.html

Go:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtfxdurpfu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cdnleiting.top/gtjzerewcy.html

C#:   // 手写递归
来源：http://hz.yuxming.cn/gtkkknwolb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nanxinkj.top/gteuwuivke.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxuanxn.top/gtkdtesgvb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gotoacloud.top/gtkilghnji.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gtvodobwcc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtqnvkugwv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtwjidhkgi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.wangdashe.top/gtfcgzgxbw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinghuilouyu.cn/gtxergqyfh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtqwnrquju.html

================================================================================
来源：http://hz.tian-w.cn/gtvklknbnq.html

O. 并发与异步
来源：http://hz.yvedp.cn/gtxkbpbbus.html

================================================================================
来源：http://hz.zhixingplan.top/gtucvknxtf.html

[O01] 启动一个线程
来源：http://hz.tian-w.cn/gtlyocwerd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj202588.top/gtcpyukniw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.c1oappe.top/gtdzcyzcrw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xylfe.cn/gtqvkcsqyc.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtlgeyhqmr.html

Java: new Thread(() -> f()).start()
来源：http://hz.jianghu66.top/gtgmwsgaya.html

Go:   go f()
来源：http://hz.xinyue.icu/gtaadjakbi.html

Ruby: Thread.new { f }
来源：http://hz.haohaochexian.top/gtuelsdeyn.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258.top/gtaprjrkrq.html

[O02] 使用线程池
来源：http://hz.fzhhl.top/gtfgcjvalk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shzxlz.cn/gtmbuzcdww.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.c1oappe.top/gtomszxwyl.html

JS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtrlwxvtcy.html

TS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gtefnxizqm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yj20258888.top/gtembppoqe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xylfe.cn/gtpskrcxzk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.vqdsnc.cn/gtjoacdrrl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hnxiangtu.top/gtxqvthqas.html

[O03] 加锁保护共享数据
来源：http://hz.nwbrower.top/gtdvtfldtv.html

Py:   with lock: shared += 1
来源：http://hz.shuidangran.top/gtktjmckks.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jqgufenzy.top/gtjhsuzauc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.feifeiyinyue.top/gtawgxkifu.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gtxhzvzvvf.html

Java: synchronized (this) { shared++; }
来源：http://hz.hnqzz.top/gtpkkxwszi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tian-w.cn/gtpkjjbtfy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cheryme.top/gtammwmfob.html

C#:   lock (gate) { shared++; }
来源：http://hz.ivvv.top/gtinrsejbg.html

[O04] 定义异步函数并等待
来源：http://hz.xinyue.icu/gtudahodcj.html

Py:   async def f():⏎    await g()
来源：http://hz.hfpthk.cn/gtbzlonyef.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhongyouzk.top/gtgjnzolsa.html

JS:   async function f() { await g(); }
来源：http://hz.ydzc1.top/gtnytstvem.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangshuangyany.cn/gtxdahijqh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gaohongyu789.top/gtvitucvsd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hfpthk.cn/gtvaqikada.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.0kj1m.cn/gtuuyxvtyh.html

C#:   async Task F() { await G(); }
来源：http://hz.dianchejie.cn/gtzydmcebl.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258888.top/gtjejhqojx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sysykeji.top/gtgtuyzvor.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cdnleiting.top/gtuujmbqso.html

JS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtwbckozcc.html

TS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtyxoldnke.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.mhx1999.top/gtqyyxgjfs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.birdmap.top/gtadgagvoo.html

Ruby: threads.map(&:join)
来源：http://hz.shzxlz.cn/gthbcvhhyi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.9152youxi.cn/gtfwgkrxha.html

[O06] 使用进程池
来源：http://hz.xuanzx.com/gtylqnvabe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.snrcjt.cn/gtwszpnsah.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.guowangkeji.top/gtzadedfpt.html

JS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtcxfpfjum.html

TS:   // child_process / cluster 模块
来源：http://hz.yongpay.top/gtnumifzns.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnxiangtu.top/gtcuqusupq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.dianchejie.cn/gtpyeoxsui.html

Ruby: // fork 块
来源：http://hz.hywenlv.cn/gtsribrfcs.html

C#:   Parallel.For
来源：http://hz.chenlongwang.top/gttscglndx.html

================================================================================
来源：http://hz.xylfe.cn/gtqyyxnklh.html

P. 常用工具函数
来源：http://hz.pengpengdd.cyou/gtmpcnkmfd.html

================================================================================
来源：http://hz.xziqi.cn/gtjzikkkzm.html

[P01] 生成 UUID
来源：http://hz.shzxlz.cn/gtlzxegiax.html

Py:   str(uuid.uuid4())
来源：http://hz.daxiang520.top/gtxjjzmuhj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sxryk.cn/gtqvyzrtpr.html

JS:   crypto.randomUUID()
来源：http://hz.gogol.net.cn/gttlvukwsc.html

TS:   crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtauvyboby.html

Java: UUID.randomUUID().toString()
来源：http://hz.nwbrower.top/gtrzokxlky.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cucudq.cn/gtnowuxclv.html

Ruby: SecureRandom.uuid
来源：http://hz.yuanzhike.top/gtwqwtdgco.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gteizmyqnf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.vqdsnc.cn/gthlgauved.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.daria6918.cn/gteyifztai.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cqqwz.cn/gtcuibljma.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.iojbl.cn/gtpexfpujn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigufen.top/gtogkfmkwy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.meibo888.top/gtxumiemva.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sysykeji.top/gtpqgdbfol.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.pengpengdd.cyou/gtphhuvjkn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hfpthk.cn/gtkgitstrd.html

[P03] 生成短随机字符串
来源：http://hz.hnqzz.top/gtklqjwxxu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhiwuduotai.top/gtiuegdgwl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ywan-chungtsiang.top/gtebcnewam.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.andypj.xyz/gtjjuwqyiz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cashguo.top/gteueyildy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.vqdsnc.cn/gtuadieusn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.0kj1m.cn/gtxnwefgtc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinyuanbaomall.cn/gtuapwttvx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.svipenyu.cn/gtlyvlgkxc.html

[P04] 求长度
来源：http://hz.xuetiantiany.cn/gtcoavzuhd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hysaishi.cn/gtnqnaecse.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnqzz.top/gtdomnlmmv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtkfwffwot.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtnxrmnydy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sufxvd.cn/gtuptlnbmr.html

Go:   len(arr);  len(m)
来源：http://hz.aibaodan.cn/gtshxwwbpg.html

Ruby: x.length;  x.size
来源：http://hz.chenlongwang.top/gttszafxyk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ehwqpu.com/gtfqvgedvk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cqqwz.cn/gtryxxgpez.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shanyushiyangkeji.top/gtjazzqemg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yuxming.cn/gtrxfxrkdo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xinyue.icu/gtgadenzcb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yanxiufei.cn/gtvdzwrxmu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yangfankeji.com/gtnramimql.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.redwolf501.top/gtuikfladq.html

Ruby: a == b
来源：http://hz.shanyushiyangkeji.top/gtyiybvbjr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.kuanghao11.cn/gttegdofxt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenzaomai.com/gtimdgspmi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhiwuduotai.top/gtwbvqvkuf.html

PHP:  if (empty($x)) {}
来源：http://hz.jqgfzy.top/gtqwuuxowm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cqqwz.cn/gttckhtuzd.html

TS:   if (x == null) {}
来源：http://hz.sufxvd.cn/gtqnpuhghu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yonumen.top/gtmjimjmhi.html

Go:   if x == nil {}
来源：http://hz.quarkkingdee.top/gtuiacqqbl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jlsjyb.cn/gtcelqegql.html

C#:   if (x is null) {}
来源：http://hz.chenlongwang.top/gtuvcqqksw.html

[P07] 防抖与节流
来源：http://hz.hongshengwenyu.top/gtluprgtwg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yvedp.cn/gtcskgxsah.html

PHP:  // 手写时间戳比较
来源：http://hz.9152youxi.cn/gtoffwpbhd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtnehmpwnm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhengqikj.top/gtojnlqrso.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xingfuxueyuan.xyz/gtqlnnyvse.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenlongwang.top/gtypyygvvb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shanyushiyangkeji.top/gtwwrjnjts.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daxiang520.top/gterqjvupk.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigufen.top/gtqseabhdo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.tianlin.xyz/gtfuwsrmud.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydzc1.top/gtqetvyrzq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.kuanghao11.cn/gtisefdxgj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gotoacloud.top/gtqwraphpk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gzhubu.top/gtaktqxzyb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shzxlz.cn/gtqxvasjyd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.c1oappe.top/gtmmfvrsyq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gtyrwszlcp.html

================================================================================
来源：http://hz.aibaodan.cn/gtwfaazkhv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cucudq.cn/gtuqxitark.html

================================================================================
来源：http://hz.daxiang520.top/gtsekvoerg.html

[Q01] 创建表
来源：http://hz.xinyue.icu/gtjcoqcqpp.html

CREATE TABLE users (
来源：http://hz.guowangkeji.top/gtxzhrwtmv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtyoduvnly.html

name VARCHAR(50) NOT NULL,
来源：http://hz.vqdsnc.cn/gttyzyphki.html

email VARCHAR(100) UNIQUE,
来源：http://hz.haohaochexian.top/gttwwjfrhw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigfzy.top/gtkvmiuvyb.html

);
来源：http://hz.wangshuangyany.cn/gtvoeybhud.html

[Q02] 创建带外键的表
来源：http://hz.guannengcc.top/gtrtnpfhfp.html

CREATE TABLE orders (
来源：http://hz.ydjk.org.cn/gtilgwcpmm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yueranfly.top/gtkxkylnnd.html

user_id INT NOT NULL,
来源：http://hz.wangshuangyany.cn/gthnubraqp.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtmqztymcp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.mhx1999.top/gthfdsbcjv.html

);
来源：http://hz.shzxlz.cn/gtkixibpaz.html

[Q03] 增加列
来源：http://hz.redwolf501.top/gttkuitevn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cucudq.cn/gtedfmkauz.html

[Q04] 修改列类型
来源：http://hz.tianlin.xyz/gtmsyasvfu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenzaomai.com/gtrjvpmrfg.html

[Q05] 重命名列
来源：http://hz.guannengcc.top/gtaaesvviv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ybcxt.top/gtwnyoqvsy.html

[Q06] 删除列
来源：http://hz.jlsjyb.cn/gtysszicqp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.fengsongda.top/gtvrzakvzl.html

[Q07] 删除表
来源：http://hz.dianchejie.cn/gtythlvnmt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.iojbl.cn/gttsvrymqq.html

[Q08] 创建普通索引
来源：http://hz.aizwys.cn/gtyhkrwvmj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gzhubu.top/gteavtpnoo.html

[Q09] 创建唯一索引
来源：http://hz.pengpengdd.cyou/gtygguwyey.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cashguo.top/gtlfnnetid.html

[Q10] 插入单行
来源：http://hz.smart0.xyz/gtpbtuirge.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenjidiqi.icu/gtbhfsvyqj.html

[Q11] 一次插入多行
来源：http://hz.cdnleiting.top/gtypkbpqbr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhiwuduotai.top/gtpbwnknuy.html

[Q12] 插入后取自增 ID
来源：http://hz.gogol.net.cn/gtrnvtaocx.html


<!-- 参考信息 -->