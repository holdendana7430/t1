代发 wailian999

Py:   if __name__ == "__main__":
来源：http://hz.iojbl.cn/gtnilcuqhp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinyuanbaomall.cn/gtfybdekwg.html

JS:   require.main === module
来源：http://hz.316326.xyz/gtcvxkvivb.html

TS:   require.main === module
来源：http://hz.jyoumei.cn/gtslhpgies.html

Java: public static void main(String[] args)
来源：http://hz.yueranfly.top/gtofhmvrgi.html

Go:   func main()
来源：http://hz.pengpengdd.cyou/gtgfvprcxp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yueranfly.top/gtkpmkchwy.html

C#:   static void Main(string[] args)
来源：http://hz.hnxiangtu.top/gthtoslohg.html

[M08] 获取系统与运行时信息
来源：http://hz.yuxming.cn/gtbaztjdgx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hfpthk.cn/gtbczjkjzs.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgufenzy.top/gtympovssl.html

JS:   process.platform;  process.version
来源：http://hz.yonumen.top/gtcjklbrps.html

TS:   process.platform;  process.version
来源：http://hz.316326.xyz/gtrroumfry.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xylfe.cn/gtpjlzkqwk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.quarkkingdee.top/gtarxanbit.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xinyue.icu/gtjvyhahmx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tian-w.cn/gtzvogdski.html

================================================================================
来源：http://hz.yj202588.top/gtavkvldji.html

N. 数据结构与算法
来源：http://hz.jlsjyb.cn/gtzckzjkmu.html

================================================================================
来源：http://hz.shuidangran.top/gtgjorkdln.html

[N01] 二分查找（有序数组）
来源：http://hz.hysaishi.cn/gtgxoenkkx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.dianchejie.cn/gttoxdqsch.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhengqikj.top/gtuobqtvzc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gaohongyu789.top/gtndfxoktr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtulfjgfmq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xylfe.cn/gtjtnodjea.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cdnleiting.top/gtfejtzntu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuxming.cn/gtolsccpmo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.bjfxy.top/gtofokeiin.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cashguo.top/gtrxplzhcy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.birdmap.top/gtmmioolxv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yanxiufei.cn/gttzzhjqxg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtwxphbujf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtewrrrate.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenlongwang.top/gtmabawfmw.html

Go:   slices.Sort(arr)
来源：http://hz.gogol.net.cn/gthtfcoikd.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gthdrqirza.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgfzy.top/gtlqfjclpe.html

[N03] 快速排序（分治示例）
来源：http://hz.gzhubu.top/gttimdufkm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yongpay.top/gtoijeekuo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.316326.xyz/gtsqadspli.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtxuydbpki.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.smart0.xyz/gtbjqlwczt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yuanzhike.top/gtxqevhwdo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.0kj1m.cn/gtmbhcieeq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jlsjyb.cn/gthpxagney.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gtghitenca.html

[N04] 斐波那契数列
来源：http://hz.zdqjudy.top/gtcjmtamam.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtkzhglqbe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangshuangyany.cn/gtmgtwjqbv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxuanxn.top/gteaesurbt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gttprnrbvr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ybcxt.top/gtkddnkiom.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cucudq.cn/gtopnpthag.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.daxiang520.top/gtqiqeqofk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.kuanghao11.cn/gtxzefzwks.html

[N05] 最大公约数
来源：http://hz.shanyushiyangtech.top/gtdibfmzov.html

Py:   math.gcd(a, b)
来源：http://hz.meibo888.top/gtawtljbln.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tanke756.top/gtptfczfwu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtokukwkqa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tian-w.cn/gtodxrvtbr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.dianchejie.cn/gtszdmvttp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shzxlz.cn/gtanhxxfyc.html

Ruby: a.gcd(b)
来源：http://hz.aibaodan.cn/gtsosrkwax.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhengqikj.top/gtcnwwtnaq.html

[N06] 判断回文字符串
来源：http://hz.wangshuangyany.cn/gtvegufjhp.html

Py:   s == s[::-1]
来源：http://hz.andypj.xyz/gtwwvvbbih.html

PHP:  $s === strrev($s);
来源：http://hz.cqqwz.cn/gtjtjzwvqm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtwlycjgot.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtxrwralma.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xinyue.icu/gtgzehkmjb.html

Go:   // 双指针从两端比较
来源：http://hz.dianchejie.cn/gtgpyizmuz.html

Ruby: s == s.reverse
来源：http://hz.hfpthk.cn/gtwqsxgrph.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yvedp.cn/gtcpnhwwfu.html

[N07] 两数之和（返回下标）
来源：http://hz.pengpengdd.cyou/gtuquosvhc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxinkj.top/gtkfluzgbi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.quarkkingdee.top/gthwjuzkdv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinghuilouyu.cn/gtvgbhjqij.html

TS:   // 手写 Map<string, number>
来源：http://hz.fzhhl.top/gteesjebkj.html

Java: // 手写 HashMap
来源：http://hz.chenjidiqi.icu/gtvkrjpkai.html

Go:   // 手写 map[int]int
来源：http://hz.cucudq.cn/gtzxxphree.html

Ruby: // 手写 Hash
来源：http://hz.bjfxy.top/gtgdcieflt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xuetiantiany.cn/gtzyjizmbo.html

[N08] 生成全排列
来源：http://hz.chenlongwang.top/gtfpfagnwu.html

Py:   itertools.permutations(arr)
来源：http://hz.smart0.xyz/gtlbdfxmbs.html

PHP:  // 手写递归交换
来源：http://hz.chenzaomai.com/gthxhwhfbj.html

JS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gturllomkw.html

TS:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtzkyrlnjr.html

Java: // 手写回溯递归
来源：http://hz.hammf.cn/gtdyojsfbm.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtzarsajop.html

Ruby: arr.permutation.to_a
来源：http://hz.meibo888.top/gtdedzlund.html

C#:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gticojyfqd.html

[N09] 栈与队列
来源：http://hz.sysykeji.top/gtzbezvpch.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhijiandao.cn/gtlvfhjufv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jlsjyb.cn/gtbkeisluz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yueranfly.top/gtkgarkqup.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cucudq.cn/gtnutugial.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.snrcjt.cn/gtfnlwpewc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sufxvd.cn/gtbfnmijic.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jianghu66.top/gtyllmvcce.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.9152youxi.cn/gtdahvegrn.html

[N10] 链表节点定义
来源：http://hz.xuetiantiany.cn/gtohbmmffz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sweek.top/gtxdanhczn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.bjfxy.top/gtxzvyjirk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yueranfly.top/gteuiqjslf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hnxiangtu.top/gttukjpjzf.html

Java: class Node { int v; Node next; }
来源：http://hz.gzhubu.top/gtndindygx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yueranfly.top/gtjgnappze.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tanke756.top/gtnfplasss.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnqzz.top/gtorkatndd.html

[N11] 二叉树中序遍历
来源：http://hz.zhixingplan.top/gtiutpkwjq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenlongwang.top/gtuwqjhupf.html

PHP:  // 手写递归函数
来源：http://hz.yuxming.cn/gtljfnfgcd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhaomingkeji.xyz/gtyajrjfzk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gtwwbwxabn.html

Java: // 手写递归
来源：http://hz.yanxiufei.cn/gtxfnvfevt.html

Go:   // 手写递归
来源：http://hz.cdnleiting.top/gtpwwmyyav.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhongyouzk.top/gtiuibhbqg.html

C#:   // 手写递归
来源：http://hz.nwbrower.top/gtqkredutt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ehwqpu.com/gtdepibkou.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zycfv.cn/gtozqogznl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xziqi.cn/gtoayvorei.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtcgspaksc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gttfohojnq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtskizkvrr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hfpthk.cn/gthkvjqxvh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shanyushiyangkeji.top/gtdtdwkydx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gtavxrxxts.html

================================================================================
来源：http://hz.iojbl.cn/gtjhjhkzmd.html

O. 并发与异步
来源：http://hz.shanyushiyangkeji.top/gtmegfqzdi.html

================================================================================
来源：http://hz.quarkkingdee.top/gtwbbyfkog.html

[O01] 启动一个线程
来源：http://hz.zhiwuduotai.top/gtlpnmqsgd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.meibo888.top/gtlrqpkfkh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.fengsongda.top/gtnfmkwwer.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hnqzz.top/gtbgzyyszl.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtanuhxmnr.html

Java: new Thread(() -> f()).start()
来源：http://hz.hysaishi.cn/gttjhkmnfm.html

Go:   go f()
来源：http://hz.cqqwz.cn/gtbevwtkdp.html

Ruby: Thread.new { f }
来源：http://hz.tian-w.cn/gtanzypoug.html

C#:   Task.Run(() => F());
来源：http://hz.quarkkingdee.top/gtqfnyzxig.html

[O02] 使用线程池
来源：http://hz.xinyue.icu/gtjryngtzy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ybcxt.top/gtjofnxohq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zdqjudy.top/gtzgosptkx.html

JS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtvzfnlmkz.html

TS:   // worker_threads 线程池
来源：http://hz.xuetiantiany.cn/gtymdgjnxv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.pycfn.com/gtvzenmxyf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yonumen.top/gtpgtbhbce.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gaohongyu789.top/gthjxuizpv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zdqjudy.top/gtqslbunaf.html

[O03] 加锁保护共享数据
来源：http://hz.sufxvd.cn/gtrxqntepi.html

Py:   with lock: shared += 1
来源：http://hz.xuetiantiany.cn/gtlvlnrpdw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenlongwang.top/gtbbmeajij.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenlongwang.top/gtxlguojxu.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtamscbrfk.html

Java: synchronized (this) { shared++; }
来源：http://hz.havefunace.top/gtmggsufkp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj20258.top/gtukfequnm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj202588.top/gtchhvvhpr.html

C#:   lock (gate) { shared++; }
来源：http://hz.xinyue.icu/gtviewegvq.html

[O04] 定义异步函数并等待
来源：http://hz.hammf.cn/gtzgssmkns.html

Py:   async def f():⏎    await g()
来源：http://hz.andypj.xyz/gttddaovun.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtvewxfljm.html

JS:   async function f() { await g(); }
来源：http://hz.fzhhl.top/gtvwcrzhpe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cqqwz.cn/gtmkujvasw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnqzz.top/gtvwwnneco.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.mhx1999.top/gtfhcmpzfj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.c1oappe.top/gtkyqmyvxx.html

C#:   async Task F() { await G(); }
来源：http://hz.hnxiangtu.top/gtcgzpvewt.html

[O05] 并发执行并等待全部完成
来源：http://hz.shzxlz.cn/gtpwlfufwv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ppjwa.cn/gtvcxvwtbd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xuanzx.com/gtsfiamicb.html

JS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gtwbmurvwd.html

TS:   await Promise.all(tasks)
来源：http://hz.hongshengwenyu.top/gtqcpkllcx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hysaishi.cn/gtdysfqxae.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnxiangtu.top/gtpkzvwlom.html

Ruby: threads.map(&:join)
来源：http://hz.guowangkeji.top/gtneehepgd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangtech.top/gtpcbozpfw.html

[O06] 使用进程池
来源：http://hz.jqgufenzy.top/gtkmephvdq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.pengpengdd.cyou/gtivicbyfx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sweek.top/gthijpwtcj.html

JS:   // child_process / cluster 模块
来源：http://hz.cashguo.top/gtezygcxqn.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgfzy.top/gtcgmgjicu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.andypj.xyz/gtjtxhbkuf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.meibo888.top/gtdnralugq.html

Ruby: // fork 块
来源：http://hz.cdnleiting.top/gtiqbfctlv.html

C#:   Parallel.For
来源：http://hz.guowangkeji.top/gttvhznpsu.html

================================================================================
来源：http://hz.andypj.xyz/gtpxdiscck.html

P. 常用工具函数
来源：http://hz.kuanghao11.cn/gtsjbelksd.html

================================================================================
来源：http://hz.hfpthk.cn/gtrhxonvov.html

[P01] 生成 UUID
来源：http://hz.yanxiufei.cn/gtkfuatbin.html

Py:   str(uuid.uuid4())
来源：http://hz.yongpay.top/gtxlugzgcp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jiagoushi.top/gtvlznywwv.html

JS:   crypto.randomUUID()
来源：http://hz.jqgufenzy.top/gtonglxldk.html

TS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtvrqukmpy.html

Java: UUID.randomUUID().toString()
来源：http://hz.guannengcc.top/gtarrgcyxw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ydjk.org.cn/gttqaytrfz.html

Ruby: SecureRandom.uuid
来源：http://hz.jyoumei.cn/gtizmovodu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ehwqpu.com/gtblpvhrhe.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhixingplan.top/gtabkycovu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.svipenyu.cn/gtkzkiaayf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258888.top/gtasxzdmbv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zdqjudy.top/gtivmvwigd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.bjfxy.top/gtlsuwxbqc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gogol.net.cn/gtnpdrjqug.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.redwolf501.top/gtmaediokg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigufen.top/gtazigmfht.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydzc1.top/gtyydendbi.html

[P03] 生成短随机字符串
来源：http://hz.jinqigfzy.top/gtongikgoc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ppjwa.cn/gtqebqctit.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nanxinkj.top/gtjelmytcp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fzhhl.top/gtvibpvffl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ehwqpu.com/gtkwnnlnpc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ivvv.top/gtunsxpznm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gotoacloud.top/gtctakhxyd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ybcxt.top/gtcwppcpkt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhongyouzk.top/gthscirkhh.html

[P04] 求长度
来源：http://hz.redwolf501.top/gtxggxaims.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.c1oappe.top/gtpyrjwjzb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhengqikj.top/gtpyxsbrhe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtqahqybfb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtyzzleecp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zycfv.cn/gtasclltam.html

Go:   len(arr);  len(m)
来源：http://hz.yonumen.top/gtzxzfmzwf.html

Ruby: x.length;  x.size
来源：http://hz.andypj.xyz/gtjkqajsbs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shangyingyoupin.top/gtdiseutsj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenjidiqi.icu/gtiubkfavl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.kuanghao11.cn/gtonjfswjn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sysykeji.top/gtyppimymk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yuanzhike.top/gteuqiwkdj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.316326.xyz/gtwxdulitj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jlsjyb.cn/gttvjhqtzm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenjidiqi.icu/gtxyzflzhb.html

Ruby: a == b
来源：http://hz.zycfv.cn/gtkgnjearl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.chenlongwang.top/gtwdvbpend.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yvedp.cn/gthhiobwyl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cucudq.cn/gtjqdfcrcx.html

PHP:  if (empty($x)) {}
来源：http://hz.jyoumei.cn/gtipdvebuw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.wangdashe.top/gtzvcwgysc.html

TS:   if (x == null) {}
来源：http://hz.xylfe.cn/gtnqdqjhjt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sysykeji.top/gtyhtefumd.html

Go:   if x == nil {}
来源：http://hz.svipenyu.cn/gtndwmdria.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhijiandao.cn/gtrvhoobfa.html

C#:   if (x is null) {}
来源：http://hz.yj202588.top/gtwzlnbbcb.html

[P07] 防抖与节流
来源：http://hz.pengpengdd.cyou/gtxjqbzmag.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.guowangkeji.top/gtcivatuih.html

PHP:  // 手写时间戳比较
来源：http://hz.cdnleiting.top/gtemmctjhq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gtiyiplivx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtctzwtehb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnqzz.top/gtpdwbotmh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangtech.top/gtnshmkqoo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sysykeji.top/gtsxgbtqpc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shangyingyoupin.top/gtpdmfuelr.html

[P08] 处理浮点精度问题
来源：http://hz.9152youxi.cn/gtfeqtbbsq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinghuilouyu.cn/gtmxtwidok.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhijiandao.cn/gtvxchcwdm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.fengsongda.top/gtiiissyia.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tanke756.top/gtnftqwkpu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.feifeiyinyue.top/gtgmwoeomr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yuanzhike.top/gtenvsnkde.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xinyue.icu/gtuzxjupmv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shuidangran.top/gtpgebtlyz.html

================================================================================
来源：http://hz.zhijiandao.cn/gtbiamejcf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xingfuxueyuan.xyz/gtlrpyuajs.html

================================================================================
来源：http://hz.xylfe.cn/gtcqplrbyq.html

[Q01] 创建表
来源：http://hz.ybcxt.top/gtuxogwwmk.html

CREATE TABLE users (
来源：http://hz.yueranfly.top/gtqiezzpyl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.birdmap.top/gteyqhbqkq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cqqwz.cn/gtyakeporb.html

email VARCHAR(100) UNIQUE,
来源：http://hz.0kj1m.cn/gtsjaosrzi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnxiangtu.top/gtitixqkha.html

);
来源：http://hz.pengpengdd.cyou/gttbkdjzwb.html

[Q02] 创建带外键的表
来源：http://hz.vqdsnc.cn/gtxczwzngz.html

CREATE TABLE orders (
来源：http://hz.daxiang520.top/gtfszohjuq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtmqukggen.html

user_id INT NOT NULL,
来源：http://hz.jqgufenzy.top/gteeriulod.html

amount DECIMAL(10, 2),
来源：http://hz.ehwqpu.com/gtntwjaohx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guowangkeji.top/gtryclipjh.html

);
来源：http://hz.ivvv.top/gtvetzzygs.html

[Q03] 增加列
来源：http://hz.ywan-chungtsiang.top/gtrrkubtqu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cucudq.cn/gtfwjwpgdg.html

[Q04] 修改列类型
来源：http://hz.jianghu66.top/gthvlzobru.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.svipenyu.cn/gtvqbzudhy.html

[Q05] 重命名列
来源：http://hz.yuanzhike.top/gtsqkwqiye.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258.top/gtkbswwukj.html

[Q06] 删除列
来源：http://hz.pycfn.com/gtrohsowey.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj20258.top/gtkjhknhox.html

[Q07] 删除表
来源：http://hz.hywenlv.cn/gtoppuvwet.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gogol.net.cn/gtjqwxiuny.html

[Q08] 创建普通索引
来源：http://hz.jinyuanbaomall.cn/gtzwyjyeie.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.aizwys.cn/gtonivzokf.html

[Q09] 创建唯一索引
来源：http://hz.gotoacloud.top/gtoidwlyxv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.kuanghao11.cn/gtyijcyrux.html

[Q10] 插入单行
来源：http://hz.wangshuangyany.cn/gttlojzutc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xylfe.cn/gtrmcewvju.html

[Q11] 一次插入多行
来源：http://hz.feifeiyinyue.top/gtokupsjop.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigufen.top/gthnudginz.html

[Q12] 插入后取自增 ID
来源：http://hz.kuanghao11.cn/gtxrxmogmv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sxryk.cn/gtyjsuuyfr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gaohongyu789.top/gtpxamiilo.html

[Q13] 忽略重复插入
来源：http://hz.ydjk.org.cn/gtodqcwjfn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jlsjyb.cn/gtykxjbjqz.html


<!-- 参考信息 -->