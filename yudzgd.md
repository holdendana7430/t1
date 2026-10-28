代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.dianchejie.cn/gttudwzpud.html

JS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtmxoxumlk.html

TS:   console.error("err")
来源：http://hz.aizwys.cn/gtdrqtufee.html

Java: System.err.println("err")
来源：http://hz.zhongyouzk.top/gtcroinphu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhiwuduotai.top/gticfeghsi.html

Ruby: warn "err"
来源：http://hz.xuanzx.com/gtxmqmgqzg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangkeji.top/gtqqgrxdjg.html

[M07] 判断是否为主入口
来源：http://hz.xylfe.cn/gtfrcxrjwu.html

Py:   if __name__ == "__main__":
来源：http://hz.zhoulong.xyz/gtbgncggxf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xziqi.cn/gtnfkkvbcz.html

JS:   require.main === module
来源：http://hz.tian-w.cn/gtjlxtsrlk.html

TS:   require.main === module
来源：http://hz.tian-w.cn/gtdiidrgtv.html

Java: public static void main(String[] args)
来源：http://hz.cucudq.cn/gtolmkwyef.html

Go:   func main()
来源：http://hz.yj20258.top/gtmkwggfaw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gotoacloud.top/gtzlrswphj.html

C#:   static void Main(string[] args)
来源：http://hz.pycfn.com/gtaeqjrdxh.html

[M08] 获取系统与运行时信息
来源：http://hz.chenjidiqi.icu/gtdrxvdodg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.haohaochexian.top/gtftpqizfa.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.bjfxy.top/gtpdcqxfyl.html

JS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtunchewme.html

TS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gtdoydhmul.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.kuanghao11.cn/gtutxzjxys.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhiwuduotai.top/gtehmryqhz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtyswaggoe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cheryme.top/gtoyxkcpby.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgnmnxgan.html

N. 数据结构与算法
来源：http://hz.9152youxi.cn/gtthdyxspw.html

================================================================================
来源：http://hz.yangfankeji.com/gtoxfwqchk.html

[N01] 二分查找（有序数组）
来源：http://hz.chenzaomai.com/gtszevrcfi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258888.top/gtbntjnrqg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.feifeiyinyue.top/gthljutaxg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.mhx1999.top/gtjazlopgf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guannengcc.top/gtddjfjgqm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sweek.top/gtnmtikplz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tian-w.cn/gtnvpdecbs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hfpthk.cn/gtvxybueae.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.316326.xyz/gtaafxhnew.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhiwuduotai.top/gtpmrdccnk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yvedp.cn/gtxwfbbkvz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxuanxn.top/gtbkhirlal.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtywfhwbbu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cqqwz.cn/gtnywdesbi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cucudq.cn/gtukpgszjl.html

Go:   slices.Sort(arr)
来源：http://hz.52xcode.cn/gtbdjmsjdl.html

Ruby: arr.sort
来源：http://hz.xinyue.icu/gtajfmmjqw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhaomingkeji.xyz/gtoexsxgwz.html

[N03] 快速排序（分治示例）
来源：http://hz.zhiwuduotai.top/gtqiqtjtak.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.wangshuangyany.cn/gtnanadpwn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dianchejie.cn/gtzdmltlca.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtqdtcqoln.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tian-w.cn/gtbwmxxlwr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtaihudegk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhongyouzk.top/gtreqahymi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hfpthk.cn/gtkvbeydsi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.daria6918.cn/gtdrmzyszr.html

[N04] 斐波那契数列
来源：http://hz.nwbrower.top/gtowazmyfs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtnqtjcmkt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.smart0.xyz/gtcfoicyrc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtbhtwtydh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtfvcqxwxq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuanzhike.top/gttvrwstbj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xuetiantiany.cn/gtfftabvlq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtswmjrxuw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtkvbffmxn.html

[N05] 最大公约数
来源：http://hz.tanke756.top/gtewyfelcz.html

Py:   math.gcd(a, b)
来源：http://hz.hysaishi.cn/gtvwybhqlf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj20258.top/gtmwyjyeyi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gtephkkjmb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtwmquzqxh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jlsjyb.cn/gtjnmbcxss.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenzaomai.com/gtwckecnhj.html

Ruby: a.gcd(b)
来源：http://hz.jiagoushi.top/gtfwtheash.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shanyushiyangtech.top/gtisqxdotm.html

[N06] 判断回文字符串
来源：http://hz.quarkkingdee.top/gtvnrfddpb.html

Py:   s == s[::-1]
来源：http://hz.hfpthk.cn/gtnggnsfoj.html

PHP:  $s === strrev($s);
来源：http://hz.jiagoushi.top/gtdmhzlams.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtjvnzoyck.html

TS:   s === [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtodpzozah.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shuidangran.top/gtabkufkby.html

Go:   // 双指针从两端比较
来源：http://hz.daxiang520.top/gtucstqlnb.html

Ruby: s == s.reverse
来源：http://hz.dianchejie.cn/gtcxdrlqal.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zycfv.cn/gtchbjyiqr.html

[N07] 两数之和（返回下标）
来源：http://hz.guannengcc.top/gtqdzbnese.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sweek.top/gtcqhofghg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sxryk.cn/gtkpghvcvw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yj202588.top/gttmqywgxp.html

TS:   // 手写 Map<string, number>
来源：http://hz.nanxuanxn.top/gtnmuoriid.html

Java: // 手写 HashMap
来源：http://hz.jianghu66.top/gtornwyfyr.html

Go:   // 手写 map[int]int
来源：http://hz.shuidangran.top/gthrhlhjho.html

Ruby: // 手写 Hash
来源：http://hz.wangshuangyany.cn/gtvhowtzzh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtiguvuxdx.html

[N08] 生成全排列
来源：http://hz.nanxinkj.top/gtfffmwgtn.html

Py:   itertools.permutations(arr)
来源：http://hz.cashguo.top/gtykjujnsz.html

PHP:  // 手写递归交换
来源：http://hz.chenjidiqi.icu/gtdvpcfyvy.html

JS:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtstyimbvj.html

TS:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtuipmdfdz.html

Java: // 手写回溯递归
来源：http://hz.chenlongwang.top/gthrffcusg.html

Go:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtdheythho.html

Ruby: arr.permutation.to_a
来源：http://hz.mhx1999.top/gtyujugzmn.html

C#:   // 手写回溯递归
来源：http://hz.yj20258.top/gtxtwgijcd.html

[N09] 栈与队列
来源：http://hz.xuetiantiany.cn/gtqwfxmdqy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhaomingkeji.xyz/gtzffnvpfg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.kuanghao11.cn/gtxlmymhha.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xylfe.cn/gtryzzpkrd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yongpay.top/gtgataturk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenlongwang.top/gtutvmvwjh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhengqikj.top/gtfrydnlas.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nwbrower.top/gtpdbghwas.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuxming.cn/gtfqlwwfaf.html

[N10] 链表节点定义
来源：http://hz.jinghuilouyu.cn/gtgqqjlive.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jianghu66.top/gtokbidcfm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yangfankeji.com/gtaqtdivfi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aizwys.cn/gtenffzdba.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj20258888.top/gtcmtuxnbs.html

Java: class Node { int v; Node next; }
来源：http://hz.pengpengdd.cyou/gtktrybuhg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pengpengdd.cyou/gtcujwrobw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sweek.top/gtpykzyayj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yvedp.cn/gtzfeqclti.html

[N11] 二叉树中序遍历
来源：http://hz.chenlongwang.top/gtruxtfbfu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.316326.xyz/gtyyutuabx.html

PHP:  // 手写递归函数
来源：http://hz.mhx1999.top/gtzydyfaoe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aizwys.cn/gtzzfmssua.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtqsxcxxdd.html

Java: // 手写递归
来源：http://hz.fzhhl.top/gtvrosbajm.html

Go:   // 手写递归
来源：http://hz.xylfe.cn/gtxoqrmqxi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ydjk.org.cn/gtszhskpuw.html

C#:   // 手写递归
来源：http://hz.sxryk.cn/gtxyflxtdd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jianghu66.top/gtvwpkqovr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxinkj.top/gtjdkacuat.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hfpthk.cn/gtpztoqqob.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yueranfly.top/gtjspepimr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daxiang520.top/gtqjmxslxy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gtilaeftsk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhixingplan.top/gtcpomuztp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yvedp.cn/gtxkncoles.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtmtfekorc.html

================================================================================
来源：http://hz.havefunace.top/gthdlrzcyo.html

O. 并发与异步
来源：http://hz.jqgfzy.top/gtcmjlephw.html

================================================================================
来源：http://hz.zhongyouzk.top/gttqoiihuk.html

[O01] 启动一个线程
来源：http://hz.xuetiantiany.cn/gtnniludll.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.andypj.xyz/gtqtdyjmar.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yuxming.cn/gtdjssnmpl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zycfv.cn/gtraddnowa.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtajoynsvl.html

Java: new Thread(() -> f()).start()
来源：http://hz.jiagoushi.top/gtkfdvqiut.html

Go:   go f()
来源：http://hz.aibaodan.cn/gtfpnpegcw.html

Ruby: Thread.new { f }
来源：http://hz.hammf.cn/gtddwziyez.html

C#:   Task.Run(() => F());
来源：http://hz.zhoulong.xyz/gtkyurpivl.html

[O02] 使用线程池
来源：http://hz.snrcjt.cn/gtwwuqjpsv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yvedp.cn/gtledydlhu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxinkj.top/gtkwuspepw.html

JS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtchdgexvx.html

TS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtntiutzqh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zycfv.cn/gttqjxvffq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.dashuyun.cn/gtgkrilzah.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.vqdsnc.cn/gtffasonew.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tanke756.top/gtqswdswwc.html

[O03] 加锁保护共享数据
来源：http://hz.gogol.net.cn/gtvelvdcte.html

Py:   with lock: shared += 1
来源：http://hz.guannengcc.top/gtbatcepgk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.dashuyun.cn/gtzcjdpogq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ivvv.top/gtthcfedil.html

TS:   // 同 JS
来源：http://hz.smart0.xyz/gtqqqjnyvz.html

Java: synchronized (this) { shared++; }
来源：http://hz.bjfxy.top/gtwmnsuhnn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.guannengcc.top/gtbwyfhrcs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xuetiantiany.cn/gttqmtwxve.html

C#:   lock (gate) { shared++; }
来源：http://hz.guowangkeji.top/gtnnmmncwr.html

[O04] 定义异步函数并等待
来源：http://hz.cashguo.top/gtccsrsdts.html

Py:   async def f():⏎    await g()
来源：http://hz.svipenyu.cn/gtevlgbcdq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pycfn.com/gttldbkhqt.html

JS:   async function f() { await g(); }
来源：http://hz.shuidangran.top/gtsivezlct.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhijiandao.cn/gtivamesrp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.haohaochexian.top/gtlqvznyap.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnqzz.top/gtgwufscdr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxinkj.top/gthngbovnd.html

C#:   async Task F() { await G(); }
来源：http://hz.jyoumei.cn/gtmptzneae.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhaomingkeji.xyz/gtruhbudiy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.iojbl.cn/gtehvrlkhi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tianlin.xyz/gtwuxqlvhs.html

JS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtbyzolqbh.html

TS:   await Promise.all(tasks)
来源：http://hz.aizwys.cn/gtqschwsmq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.c1oappe.top/gtpyrvfakw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuetiantiany.cn/gtgsberkkr.html

Ruby: threads.map(&:join)
来源：http://hz.hongshengwenyu.top/gtmiyniykb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cdnleiting.top/gtbuixlwiw.html

[O06] 使用进程池
来源：http://hz.nanxinkj.top/gtjpfblqkm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangtech.top/gtnhcyflln.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtaipsfqcv.html

JS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtcrukopja.html

TS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtpyminaoc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cdnleiting.top/gtownjqfry.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cdnleiting.top/gtrwvinwps.html

Ruby: // fork 块
来源：http://hz.dashuyun.cn/gtthvioclg.html

C#:   Parallel.For
来源：http://hz.zhijiandao.cn/gtdfdpzocy.html

================================================================================
来源：http://hz.aibaodan.cn/gtkrgjhfhe.html

P. 常用工具函数
来源：http://hz.xingfuxueyuan.xyz/gterihczki.html

================================================================================
来源：http://hz.redwolf501.top/gttdbihzuq.html

[P01] 生成 UUID
来源：http://hz.guowangkeji.top/gtdjwjjsig.html

Py:   str(uuid.uuid4())
来源：http://hz.havefunace.top/gtkttkhlfd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dianchejie.cn/gtxzjfkgvu.html

JS:   crypto.randomUUID()
来源：http://hz.hammf.cn/gtvwpqigke.html

TS:   crypto.randomUUID()
来源：http://hz.jianghu66.top/gtgrmajggx.html

Java: UUID.randomUUID().toString()
来源：http://hz.kuanghao11.cn/gtycubbxht.html

Go:   // 用 github.com/google/uuid
来源：http://hz.haohaochexian.top/gtfcdqrtsw.html

Ruby: SecureRandom.uuid
来源：http://hz.sysykeji.top/gtimmncync.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shzxlz.cn/gtcewcrvca.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhengqikj.top/gttgpjness.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ybcxt.top/gtgyyhioax.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jqgufenzy.top/gtcnucusmt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jqgfzy.top/gtcnkqvwmn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhijiandao.cn/gthphbfgcy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhoulong.xyz/gtpcnwifuj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hnxiangtu.top/gtzowgvswy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.daxiang520.top/gtylhmediw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tanke756.top/gtamnflhht.html

[P03] 生成短随机字符串
来源：http://hz.chenjidiqi.icu/gtjfpjbyie.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnqzz.top/gtwovtowzr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gogol.net.cn/gtgzobqgnm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gogol.net.cn/gtzonwqulu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gtbwrclqiu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guannengcc.top/gtzcfpzkrs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.quarkkingdee.top/gtookkhvwq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ybcxt.top/gtxagjzold.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tanke756.top/gtktjhjrgn.html

[P04] 求长度
来源：http://hz.jyoumei.cn/gtlvsetatz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.aizwys.cn/gtpvlisshc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxinkj.top/gtmtxaocel.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtymufvgom.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhengqikj.top/gtapkrpeuw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yuxming.cn/gtefhrznte.html

Go:   len(arr);  len(m)
来源：http://hz.haohaochexian.top/gtfsxxectf.html

Ruby: x.length;  x.size
来源：http://hz.jqgfzy.top/gtmmvhlaog.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cdnleiting.top/gtbwnjteqr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yuxming.cn/gtvxwmyzni.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.0kj1m.cn/gtupsejetk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yueranfly.top/gtwfqcrkih.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.havefunace.top/gtjxsgattd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gthzcftkqy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.9152youxi.cn/gtouyfkuzh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hammf.cn/gtckqaihzb.html

Ruby: a == b
来源：http://hz.kuanghao11.cn/gtqrxaxthv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guannengcc.top/gtgahrktxr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.mhx1999.top/gtsfsqechj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.andypj.xyz/gtvemfbvyr.html

PHP:  if (empty($x)) {}
来源：http://hz.quarkkingdee.top/gtoukgnafh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jiagoushi.top/gtmutihmyj.html

TS:   if (x == null) {}
来源：http://hz.ehwqpu.com/gtuahxvwxq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtkupbohxm.html

Go:   if x == nil {}
来源：http://hz.316326.xyz/gtrpvcctnf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.iojbl.cn/gtoodkekhq.html

C#:   if (x is null) {}
来源：http://hz.yj20258888.top/gtuqfowwwq.html

[P07] 防抖与节流
来源：http://hz.cashguo.top/gtcltdvqcf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cdnleiting.top/gtiwrthmkc.html

PHP:  // 手写时间戳比较
来源：http://hz.cdnleiting.top/gthydinhra.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.kuanghao11.cn/gtcmbwccxf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tianlin.xyz/gtotmrzbqv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.havefunace.top/gtwqwokpub.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.redwolf501.top/gtnhtrfdvv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenzaomai.com/gtkturlaoo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhongyouzk.top/gtyjnnlaxl.html

[P08] 处理浮点精度问题
来源：http://hz.zhengqikj.top/gtdgjmcsoa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jyoumei.cn/gtlqoxyzbz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigufen.top/gtcykwccpz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ehwqpu.com/gtnfwqegbc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.pengpengdd.cyou/gttrwfrnnl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gotoacloud.top/gtqiglwupd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenlongwang.top/gtkzvmleyu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tanke756.top/gtypokpjwy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yonumen.top/gttartagmf.html

================================================================================
来源：http://hz.havefunace.top/gtonotylyw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhiwuduotai.top/gtplilkjtn.html

================================================================================
来源：http://hz.haohaochexian.top/gtxdrwyyby.html

[Q01] 创建表
来源：http://hz.yvedp.cn/gtawldcyjd.html

CREATE TABLE users (
来源：http://hz.xuetiantiany.cn/gtzmfucpoa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj202588.top/gtchjbghth.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuanzx.com/gteigwbhfg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cheryme.top/gtkdcqutif.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yvedp.cn/gtmfkpvhgm.html

);
来源：http://hz.snrcjt.cn/gtlvffbdot.html

[Q02] 创建带外键的表
来源：http://hz.sysykeji.top/gtutkwfmjp.html

CREATE TABLE orders (
来源：http://hz.cucudq.cn/gtusdjjbtj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gtnlvdimbk.html

user_id INT NOT NULL,
来源：http://hz.fzhhl.top/gthaxjttrg.html

amount DECIMAL(10, 2),
来源：http://hz.xuetiantiany.cn/gtklkmplub.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gaohongyu789.top/gtiuplrivt.html

);
来源：http://hz.jianghu66.top/gtdrgtbhha.html

[Q03] 增加列
来源：http://hz.sysykeji.top/gtxyxiizjr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fengsongda.top/gttjlbirlf.html

[Q04] 修改列类型
来源：http://hz.shangyingyoupin.top/gtcytsppll.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuxming.cn/gtdxpuxton.html

[Q05] 重命名列
来源：http://hz.zhengqikj.top/gtssjozgwm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.quarkkingdee.top/gtjahyekfv.html

[Q06] 删除列
来源：http://hz.c1oappe.top/gtjzwwygmt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenzaomai.com/gtdlnytlfd.html

[Q07] 删除表
来源：http://hz.ybcxt.top/gtljubaatq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnqzz.top/gtkgqgwmlz.html

[Q08] 创建普通索引
来源：http://hz.yangfankeji.com/gtpgphtbld.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ywan-chungtsiang.top/gtygnrzaqq.html

[Q09] 创建唯一索引
来源：http://hz.cqqwz.cn/gtxkorwdli.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhixingplan.top/gttusfpexx.html

[Q10] 插入单行
来源：http://hz.quarkkingdee.top/gtlbycadey.html


<!-- 参考信息 -->