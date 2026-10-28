代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj20258.top/gtzhkxjagb.html

JS:   console.error("err")
来源：http://hz.xuanzx.com/gtiqgxpoyk.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gtehrmajut.html

Java: System.err.println("err")
来源：http://hz.daxiang520.top/gtogkjigpi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xinyue.icu/gtgojmkjow.html

Ruby: warn "err"
来源：http://hz.jinqigufen.top/gtrnwyagmr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gaohongyu789.top/gtnrnnrpea.html

[M07] 判断是否为主入口
来源：http://hz.9152youxi.cn/gtexpdrqdv.html

Py:   if __name__ == "__main__":
来源：http://hz.dashuyun.cn/gtmkutaquo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhaomingkeji.xyz/gtdypywaeq.html

JS:   require.main === module
来源：http://hz.ppjwa.cn/gteinyxcoz.html

TS:   require.main === module
来源：http://hz.52xcode.cn/gtuhevwlbj.html

Java: public static void main(String[] args)
来源：http://hz.zhixingplan.top/gtvcoxbesm.html

Go:   func main()
来源：http://hz.xuanzx.com/gtsdoyiybj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cheryme.top/gtyjqqzhtm.html

C#:   static void Main(string[] args)
来源：http://hz.gzhubu.top/gtustkuiuu.html

[M08] 获取系统与运行时信息
来源：http://hz.bjfxy.top/gtnpckeefg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.snrcjt.cn/gtutuinwul.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.andypj.xyz/gtrbwpylfm.html

JS:   process.platform;  process.version
来源：http://hz.gaohongyu789.top/gtmwgfcqcc.html

TS:   process.platform;  process.version
来源：http://hz.jinyuanbaomall.cn/gtjlstsnte.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhoulong.xyz/gtnkztgfjv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sysykeji.top/gtjvtjwbdf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sxryk.cn/gtblppqpvx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gzhubu.top/gtfeudbijj.html

================================================================================
来源：http://hz.zhixingplan.top/gtzvgcixsk.html

N. 数据结构与算法
来源：http://hz.jinqigufen.top/gtvireyipt.html

================================================================================
来源：http://hz.yonumen.top/gtwjjmmfut.html

[N01] 二分查找（有序数组）
来源：http://hz.tianlin.xyz/gtnytmbhzn.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zycfv.cn/gturxhpdwx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhixingplan.top/gtxqdyafyk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtrsfyubze.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yangfankeji.com/gtbbclkxxw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.fzhhl.top/gtboxybhaa.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sysykeji.top/gtibmirilo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhijiandao.cn/gtwxkoimro.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtnfioaayb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yanxiufei.cn/gtkgfavkmd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yongpay.top/gtzwvlzazt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cucudq.cn/gtmukalfrx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtinqoopja.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gtgzstipgn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangtech.top/gtgewrrptl.html

Go:   slices.Sort(arr)
来源：http://hz.shuidangran.top/gtmusbsjoq.html

Ruby: arr.sort
来源：http://hz.cashguo.top/gtprclzoyg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.meibo888.top/gtgetwwigo.html

[N03] 快速排序（分治示例）
来源：http://hz.snrcjt.cn/gtnfvhbzid.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258.top/gtkwyarjqi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hongshengwenyu.top/gtgzchhelz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gtxithaxio.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtsdobnasg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cdnleiting.top/gthaquwsdi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yueranfly.top/gteguaylbo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gtbebwzohp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tian-w.cn/gtumxvupmc.html

[N04] 斐波那契数列
来源：http://hz.wangdashe.top/gtfiqmedax.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.daxiang520.top/gtkvytggdr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hywenlv.cn/gtvppascce.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtftggperv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtvmwflcwe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ydjk.org.cn/gthilreyey.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yongpay.top/gtqwtickfz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gzhubu.top/gtkhjinmxf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.pycfn.com/gttwmifdvj.html

[N05] 最大公约数
来源：http://hz.havefunace.top/gtsoepygsp.html

Py:   math.gcd(a, b)
来源：http://hz.zhongyouzk.top/gtuzytdovm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ydzc1.top/gtnzxqxvcm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtxlhwldxi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ppjwa.cn/gtfvafplec.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shzxlz.cn/gttvhuicdb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenlongwang.top/gtzepwntwh.html

Ruby: a.gcd(b)
来源：http://hz.zycfv.cn/gtaprinede.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.fzhhl.top/gtryaxnddb.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtggbasbnu.html

Py:   s == s[::-1]
来源：http://hz.hammf.cn/gtcxnszcey.html

PHP:  $s === strrev($s);
来源：http://hz.wangshuangyany.cn/gtkujpboge.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtyfwmflui.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtdkyxdopf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hysaishi.cn/gtazkdcxqe.html

Go:   // 双指针从两端比较
来源：http://hz.aibaodan.cn/gtmymrgbcu.html

Ruby: s == s.reverse
来源：http://hz.hongshengwenyu.top/gtffuklmai.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sysykeji.top/gtauqzdltt.html

[N07] 两数之和（返回下标）
来源：http://hz.xziqi.cn/gtcojhfmjt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ivvv.top/gtrxlfuobg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhaomingkeji.xyz/gtyczpptbx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.chenjidiqi.icu/gtdoiaadog.html

TS:   // 手写 Map<string, number>
来源：http://hz.ppjwa.cn/gtjaxuljzw.html

Java: // 手写 HashMap
来源：http://hz.haohaochexian.top/gtehunwsyc.html

Go:   // 手写 map[int]int
来源：http://hz.jinqigufen.top/gtualhmnyn.html

Ruby: // 手写 Hash
来源：http://hz.redwolf501.top/gtmhxxidea.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenzaomai.com/gtjmabizve.html

[N08] 生成全排列
来源：http://hz.zhoulong.xyz/gtylwbdlnr.html

Py:   itertools.permutations(arr)
来源：http://hz.kuanghao11.cn/gtusbuvyad.html

PHP:  // 手写递归交换
来源：http://hz.xinyue.icu/gthuipszdu.html

JS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtnjkywnjg.html

TS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gttsymmphf.html

Java: // 手写回溯递归
来源：http://hz.mhx1999.top/gtugqbrxjo.html

Go:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtkjftuyai.html

Ruby: arr.permutation.to_a
来源：http://hz.yvedp.cn/gthtiivior.html

C#:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtkrytclya.html

[N09] 栈与队列
来源：http://hz.sysykeji.top/gtlisdahiq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jyoumei.cn/gtozafbgwv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenlongwang.top/gtuvuvoexf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hfpthk.cn/gtretdpbog.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fengsongda.top/gtogkfwjoq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nwbrower.top/gtjamhknzx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gttdtoqvlo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ivvv.top/gtxypwnxiz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xinyue.icu/gtlwgdjroi.html

[N10] 链表节点定义
来源：http://hz.pengpengdd.cyou/gtdquspwub.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daria6918.cn/gtqhtomcbc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zycfv.cn/gtasscyunu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zycfv.cn/gtqjggkvcu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tianlin.xyz/gtokfrugxt.html

Java: class Node { int v; Node next; }
来源：http://hz.guannengcc.top/gtswqpeqrv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigfzy.top/gtjxntfgfv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dashuyun.cn/gtuufoxyzo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ivvv.top/gtszwpqsvp.html

[N11] 二叉树中序遍历
来源：http://hz.nanxinkj.top/gtkotqmviu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jqgfzy.top/gtxzancttn.html

PHP:  // 手写递归函数
来源：http://hz.guannengcc.top/gtsigdbsft.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ppjwa.cn/gtppcpbycp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hammf.cn/gtlfkpldkr.html

Java: // 手写递归
来源：http://hz.iojbl.cn/gtyohefzhg.html

Go:   // 手写递归
来源：http://hz.jianghu66.top/gtawoipuey.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.fengsongda.top/gtztoabzlp.html

C#:   // 手写递归
来源：http://hz.yonumen.top/gtzwlsovfi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xylfe.cn/gtyminopdm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinqigufen.top/gtnwnxydww.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cdnleiting.top/gtuzoqvfml.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gtphobgbym.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hfpthk.cn/gtpbievzyw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtcuupcuik.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yvedp.cn/gtnlxywswr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.fzhhl.top/gtfpdmxwlj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guannengcc.top/gtjywszbnh.html

================================================================================
来源：http://hz.yj20258.top/gtgtbsflyp.html

O. 并发与异步
来源：http://hz.jlsjyb.cn/gtbvlwdsjw.html

================================================================================
来源：http://hz.cdnleiting.top/gtypvdpmqs.html

[O01] 启动一个线程
来源：http://hz.shzxlz.cn/gtynrtpifo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xziqi.cn/gtwehpckwq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.316326.xyz/gtyylrsdws.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zdqjudy.top/gthcrabify.html

TS:   // 同 JS
来源：http://hz.bjfxy.top/gttybdkptn.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigufen.top/gtaefbticy.html

Go:   go f()
来源：http://hz.jianghu66.top/gtyripltui.html

Ruby: Thread.new { f }
来源：http://hz.havefunace.top/gtnfmvcepl.html

C#:   Task.Run(() => F());
来源：http://hz.9152youxi.cn/gtmcsdnhfy.html

[O02] 使用线程池
来源：http://hz.nanxuanxn.top/gtyacjwfrv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hammf.cn/gtbjpjugnt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgufenzy.top/gtrdieolqi.html

JS:   // worker_threads 线程池
来源：http://hz.ydzc1.top/gtygbinumi.html

TS:   // worker_threads 线程池
来源：http://hz.shangyingyoupin.top/gtygahbufi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daxiang520.top/gtvlpvltlx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ywan-chungtsiang.top/gtkdggjtyh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxuanxn.top/gtdkskypjy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.svipenyu.cn/gtdbrghbsa.html

[O03] 加锁保护共享数据
来源：http://hz.tianlin.xyz/gthqoutukk.html

Py:   with lock: shared += 1
来源：http://hz.gaohongyu789.top/gthtkxdlqe.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.daria6918.cn/gtsbquukky.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cdnleiting.top/gtybwoffpc.html

TS:   // 同 JS
来源：http://hz.sxryk.cn/gtmdgpnbmv.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtbdhhhfae.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aibaodan.cn/gtdnzidjry.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ydjk.org.cn/gtyxbpcjdk.html

C#:   lock (gate) { shared++; }
来源：http://hz.shzxlz.cn/gtpqayfmyo.html

[O04] 定义异步函数并等待
来源：http://hz.havefunace.top/gtirftcfuy.html

Py:   async def f():⏎    await g()
来源：http://hz.hnqzz.top/gtknmcpmry.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuetiantiany.cn/gtbhhnbqdj.html

JS:   async function f() { await g(); }
来源：http://hz.yueranfly.top/gtnpatuqpp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hongshengwenyu.top/gtrfwjspow.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinqigufen.top/gtpidkhlho.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hammf.cn/gtfrifnhgk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.mhx1999.top/gthylbzndv.html

C#:   async Task F() { await G(); }
来源：http://hz.jianghu66.top/gtvzsdyfnh.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigufen.top/gtzkxreyah.html

Py:   asyncio.gather(*tasks)
来源：http://hz.andypj.xyz/gttxepuhle.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xziqi.cn/gtxnjeoysw.html

JS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtwkhhezuc.html

TS:   await Promise.all(tasks)
来源：http://hz.ppjwa.cn/gtbpcumyux.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.daria6918.cn/gtvixzysby.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.c1oappe.top/gthxiockmm.html

Ruby: threads.map(&:join)
来源：http://hz.chenzaomai.com/gtxdtyfczx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shzxlz.cn/gtaszhofkd.html

[O06] 使用进程池
来源：http://hz.pycfn.com/gtbcpftecy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.0kj1m.cn/gtjbnscgmn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jqgufenzy.top/gtecbrjnbw.html

JS:   // child_process / cluster 模块
来源：http://hz.zdqjudy.top/gtictwmadt.html

TS:   // child_process / cluster 模块
来源：http://hz.ydjk.org.cn/gtnflbmrqn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnxiangtu.top/gtwukwteem.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.daxiang520.top/gtodwhyauo.html

Ruby: // fork 块
来源：http://hz.cheryme.top/gtuodplnen.html

C#:   Parallel.For
来源：http://hz.zhengqikj.top/gtxyaibaoy.html

================================================================================
来源：http://hz.cdnleiting.top/gtwnvdqyjk.html

P. 常用工具函数
来源：http://hz.52xcode.cn/gtugimjcsb.html

================================================================================
来源：http://hz.xziqi.cn/gtfcoqqshn.html

[P01] 生成 UUID
来源：http://hz.yanxiufei.cn/gtzfztcmrc.html

Py:   str(uuid.uuid4())
来源：http://hz.guannengcc.top/gthllkhzlw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.snrcjt.cn/gthqjagbdg.html

JS:   crypto.randomUUID()
来源：http://hz.daria6918.cn/gtekzqcozv.html

TS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtvmiegwfh.html

Java: UUID.randomUUID().toString()
来源：http://hz.gzhubu.top/gtyrocazlo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenlongwang.top/gtctqsoeti.html

Ruby: SecureRandom.uuid
来源：http://hz.tian-w.cn/gtiamrotqq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhengqikj.top/gtmmdzpawp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gtkeaymlvu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ehwqpu.com/gtfmczatar.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aizwys.cn/gtjobptuyk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhongyouzk.top/gtluvnjppr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.feifeiyinyue.top/gtbioxeclv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258888.top/gteqyighej.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.birdmap.top/gtnqgciibv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.c1oappe.top/gtrnnvasld.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gogol.net.cn/gtzxlldkch.html

[P03] 生成短随机字符串
来源：http://hz.9152youxi.cn/gtxfxjwjun.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgfzy.top/gtyjogevmu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.52xcode.cn/gtjjjnwrba.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xylfe.cn/gtjbgyedpz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.c1oappe.top/gtnfpsvsgo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yangfankeji.com/gtwoomwvja.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhoulong.xyz/gtzjpcprut.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jianghu66.top/gtbyxlrswr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fengsongda.top/gtmcgjkefc.html

[P04] 求长度
来源：http://hz.sxryk.cn/gtretyiskz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nanxinkj.top/gtpiwdoxsj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtessncbdw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gthossmkoi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtmvpdjkjy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yangfankeji.com/gtvpywfguo.html

Go:   len(arr);  len(m)
来源：http://hz.jqgfzy.top/gtttycbaax.html

Ruby: x.length;  x.size
来源：http://hz.ppjwa.cn/gtwscutfwl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hysaishi.cn/gthewooufi.html

[P05] 判断两个对象内容是否相等
来源：http://hz.meibo888.top/gtzpangurf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.feifeiyinyue.top/gttwbprxwb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.dianchejie.cn/gtkafoixdf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gaohongyu789.top/gtvoalmtzr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jyoumei.cn/gtesjlrzmn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yangfankeji.com/gtmsbbrrvb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yongpay.top/gtdrhxpiha.html

Ruby: a == b
来源：http://hz.yueranfly.top/gteuvptxrb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.birdmap.top/gtbkifvsqz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.andypj.xyz/gtmpnsqdty.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gotoacloud.top/gtajqsvozq.html

PHP:  if (empty($x)) {}
来源：http://hz.shuidangran.top/gtniwycufh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xingfuxueyuan.xyz/gtxzzhypck.html

TS:   if (x == null) {}
来源：http://hz.zhixingplan.top/gtykvjvcef.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daria6918.cn/gtkgvzdlhv.html

Go:   if x == nil {}
来源：http://hz.xingfuxueyuan.xyz/gtqksllkue.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aizwys.cn/gtyrciuouq.html

C#:   if (x is null) {}
来源：http://hz.hnqzz.top/gtsoaffpky.html

[P07] 防抖与节流
来源：http://hz.cucudq.cn/gtfehzobym.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zdqjudy.top/gtqbiaacuj.html

PHP:  // 手写时间戳比较
来源：http://hz.andypj.xyz/gtljgbotyt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtstadinfb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtqpawydhn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.havefunace.top/gtgyvgingi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.daria6918.cn/gtqmbjhayw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.c1oappe.top/gtkoqflkea.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.bjfxy.top/gtxeiynwrj.html

[P08] 处理浮点精度问题
来源：http://hz.wangdashe.top/gtqyfdckos.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.feifeiyinyue.top/gtliaafzug.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydjk.org.cn/gtwkzpsdcl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangdashe.top/gtkkosflyk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gotoacloud.top/gtuaheximv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jiagoushi.top/gtbhrlyzxx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nanxinkj.top/gtddhvpnaz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhoulong.xyz/gtficnqsmg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.quarkkingdee.top/gtmfganvuy.html

================================================================================
来源：http://hz.hnxiangtu.top/gtpggzysxh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tanke756.top/gtkzvqauyd.html

================================================================================
来源：http://hz.jqgfzy.top/gtypyfozvw.html

[Q01] 创建表
来源：http://hz.feifeiyinyue.top/gtqxnmqeje.html

CREATE TABLE users (
来源：http://hz.sufxvd.cn/gtqsyddukh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gtghokgshq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hnxiangtu.top/gtnmewzfwb.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigufen.top/gtbbqgymyy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gtkpxkebrt.html

);
来源：http://hz.ppjwa.cn/gtzooqjanm.html

[Q02] 创建带外键的表
来源：http://hz.nanxinkj.top/gtmtwbasyj.html

CREATE TABLE orders (
来源：http://hz.fzhhl.top/gtneggnhkl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtprtceckf.html

user_id INT NOT NULL,
来源：http://hz.xylfe.cn/gtamtnvtcv.html

amount DECIMAL(10, 2),
来源：http://hz.sxryk.cn/gtchmfisih.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigufen.top/gtgrguxcvb.html

);
来源：http://hz.ppjwa.cn/gteeqgjeti.html

[Q03] 增加列
来源：http://hz.zhiwuduotai.top/gtjwofnhdg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jyoumei.cn/gtrdedsjtt.html

[Q04] 修改列类型
来源：http://hz.smart0.xyz/gtkihpxuej.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhengqikj.top/gtuexccavr.html

[Q05] 重命名列
来源：http://hz.sysykeji.top/gtmwwvdujg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxuanxn.top/gtvoncwilj.html

[Q06] 删除列
来源：http://hz.zhoulong.xyz/gtipwvrocb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.feifeiyinyue.top/gtimeszbsf.html

[Q07] 删除表
来源：http://hz.ivvv.top/gtgxxohevf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sweek.top/gtqeutphfu.html

[Q08] 创建普通索引
来源：http://hz.cqqwz.cn/gtgcsdtfuo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.meibo888.top/gtinvwrfjd.html

[Q09] 创建唯一索引
来源：http://hz.kuanghao11.cn/gthdxqdksl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhijiandao.cn/gtunoulsol.html

[Q10] 插入单行
来源：http://hz.ybcxt.top/gtbzjsutio.html


<!-- 参考信息 -->