代发 wailian999

Java: public static void main(String[] args)
来源：http://hz.zhijiandao.cn/gtmtorvuib.html

Go:   func main()
来源：http://hz.zhijiandao.cn/gthzajbpjs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenjidiqi.icu/gtwstsdeea.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtrzcwbshb.html

[M08] 获取系统与运行时信息
来源：http://hz.jlsjyb.cn/gtkrukkpgv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.birdmap.top/gtyvyekqrl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.aizwys.cn/gtzmrmwwtt.html

JS:   process.platform;  process.version
来源：http://hz.yangfankeji.com/gtqmayksyp.html

TS:   process.platform;  process.version
来源：http://hz.ywan-chungtsiang.top/gtxhminydv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.feifeiyinyue.top/gtncyprspa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tian-w.cn/gtfpuqfvlj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgfzy.top/gtgchvcifd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hongshengwenyu.top/gtdrmtfbqf.html

================================================================================
来源：http://hz.haohaochexian.top/gtqwmookqo.html

N. 数据结构与算法
来源：http://hz.tianlin.xyz/gtomxghlhi.html

================================================================================
来源：http://hz.mhx1999.top/gtqjvjbkcu.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtzceofryg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zdqjudy.top/gtzcwspdiz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.feifeiyinyue.top/gtfleonxdo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtpcjumaad.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ivvv.top/gtsykezhzj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ivvv.top/gtwqjmkvql.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gogol.net.cn/gtkhbinmbk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinyuanbaomall.cn/gttcbindam.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtfzgtgkpe.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jiagoushi.top/gtlemcyvhz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shuidangran.top/gtimwvaand.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nwbrower.top/gtfndxjtjd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtjzhzrwag.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtzrqpbyzm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hammf.cn/gtovbhlwcl.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gtngcfqoud.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gttpnasohi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxinkj.top/gthatcsorv.html

[N03] 快速排序（分治示例）
来源：http://hz.kuanghao11.cn/gtwzleueof.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.52xcode.cn/gtycnvknnf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daria6918.cn/gtkmzywwvh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtpydsuvle.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hfpthk.cn/gtghkvpzyr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dashuyun.cn/gtwewyxmex.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yonumen.top/gtrjlxjxsf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.bjfxy.top/gtbpvqbpcn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenjidiqi.icu/gtnesgiuaz.html

[N04] 斐波那契数列
来源：http://hz.shanyushiyangtech.top/gtdquocnhg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtbfuddaco.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ydzc1.top/gtyntoagex.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yongpay.top/gtmfkczlbn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gzhubu.top/gtruxffrlw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shuidangran.top/gtwjvdtsis.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.bjfxy.top/gtzzciczdm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gtzjwfztvp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenlongwang.top/gtpxepkxuv.html

[N05] 最大公约数
来源：http://hz.yuanzhike.top/gtqzzziyac.html

Py:   math.gcd(a, b)
来源：http://hz.shangyingyoupin.top/gtjeduifyv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.quarkkingdee.top/gtstubyqyh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhengqikj.top/gtscnrsvno.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.mhx1999.top/gtceaujpiy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenlongwang.top/gtktxstahe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gogol.net.cn/gtgobdensd.html

Ruby: a.gcd(b)
来源：http://hz.jinghuilouyu.cn/gtfhltgcqa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj202588.top/gtybwxooqf.html

[N06] 判断回文字符串
来源：http://hz.xingfuxueyuan.xyz/gtsrzjkfip.html

Py:   s == s[::-1]
来源：http://hz.daxiang520.top/gtrpckaazi.html

PHP:  $s === strrev($s);
来源：http://hz.chenjidiqi.icu/gtyyomnkco.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtvmaeorpn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtunflyaju.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zdqjudy.top/gtioyhqsot.html

Go:   // 双指针从两端比较
来源：http://hz.zhoulong.xyz/gtqunjavza.html

Ruby: s == s.reverse
来源：http://hz.sweek.top/gtywafnvsn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sxryk.cn/gtfkzjmojr.html

[N07] 两数之和（返回下标）
来源：http://hz.svipenyu.cn/gtlgavclnv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.iojbl.cn/gtiwwxajki.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shuidangran.top/gtwotoginj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gogol.net.cn/gtaibekjez.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuxming.cn/gthesonmtn.html

Java: // 手写 HashMap
来源：http://hz.sxryk.cn/gtflermzgy.html

Go:   // 手写 map[int]int
来源：http://hz.yj20258.top/gtqqtizbzy.html

Ruby: // 手写 Hash
来源：http://hz.hysaishi.cn/gtyfentwhq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xuanzx.com/gttfcaaiue.html

[N08] 生成全排列
来源：http://hz.sxryk.cn/gtxedgsmlg.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigufen.top/gttvaiavsv.html

PHP:  // 手写递归交换
来源：http://hz.xuetiantiany.cn/gtiviqjgnu.html

JS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtsiszsqtd.html

TS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtczdfpvdx.html

Java: // 手写回溯递归
来源：http://hz.hnqzz.top/gtwzruxnrr.html

Go:   // 手写回溯递归
来源：http://hz.hnqzz.top/gttzchiblb.html

Ruby: arr.permutation.to_a
来源：http://hz.52xcode.cn/gtznrqjlau.html

C#:   // 手写回溯递归
来源：http://hz.yonumen.top/gtliqbjhbv.html

[N09] 栈与队列
来源：http://hz.yj202588.top/gtyhumuyzk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.andypj.xyz/gtfuqszwqo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinghuilouyu.cn/gtrpaeiajs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sxryk.cn/gthivusjey.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sysykeji.top/gteojnfass.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhoulong.xyz/gtefhoteku.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigufen.top/gtmdhwypkk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jlsjyb.cn/gtvgepzdlm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.havefunace.top/gtyjvpwugo.html

[N10] 链表节点定义
来源：http://hz.jianghu66.top/gtsxakwjvc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhiwuduotai.top/gtqtyfbccp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.c1oappe.top/gtrrqijbgb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tanke756.top/gtdlwtxzjp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tanke756.top/gtgzmlzwni.html

Java: class Node { int v; Node next; }
来源：http://hz.daria6918.cn/gtzcgdadur.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yuxming.cn/gtzumylyhj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigufen.top/gtsjljwklr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.aibaodan.cn/gtkoxremkx.html

[N11] 二叉树中序遍历
来源：http://hz.tian-w.cn/gtygoxpwgj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhaomingkeji.xyz/gtejnvjbkg.html

PHP:  // 手写递归函数
来源：http://hz.ydjk.org.cn/gtgljtxvwb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guannengcc.top/gtkqfvxbki.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydjk.org.cn/gtbeqlwnku.html

Java: // 手写递归
来源：http://hz.daxiang520.top/gtwqvvqopi.html

Go:   // 手写递归
来源：http://hz.zhoulong.xyz/gteiveslpu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.birdmap.top/gtqjfyneex.html

C#:   // 手写递归
来源：http://hz.ivvv.top/gttfkpeimz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.mhx1999.top/gtvktxvary.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.dashuyun.cn/gtiogxpwwj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gaohongyu789.top/gtihyaookp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gtlaktmuct.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gtzuinlssy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtcvxvnjka.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhixingplan.top/gtpmwimaav.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aizwys.cn/gtnmtuopjg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtkjmvoqfo.html

================================================================================
来源：http://hz.cqqwz.cn/gtgeepcunt.html

O. 并发与异步
来源：http://hz.fengsongda.top/gtuwqfeyog.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtjlvuowhl.html

[O01] 启动一个线程
来源：http://hz.sweek.top/gtuemmosoe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj20258888.top/gtefuzknxn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sweek.top/gtlasjtaht.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.smart0.xyz/gtlxppqjxe.html

TS:   // 同 JS
来源：http://hz.0kj1m.cn/gtlvcmkheb.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangshuangyany.cn/gtjqyrnlyj.html

Go:   go f()
来源：http://hz.mhx1999.top/gtblsxnhlu.html

Ruby: Thread.new { f }
来源：http://hz.sufxvd.cn/gtitodmghm.html

C#:   Task.Run(() => F());
来源：http://hz.xuanzx.com/gtargijpve.html

[O02] 使用线程池
来源：http://hz.wangshuangyany.cn/gtmztkwovf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.316326.xyz/gtazaahyjk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.0kj1m.cn/gtwyxyqqau.html

JS:   // worker_threads 线程池
来源：http://hz.gzhubu.top/gteqtglbsm.html

TS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtrielyezo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuxming.cn/gteammyado.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xinyue.icu/gttiueqatq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.vqdsnc.cn/gtonbtpzqq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhijiandao.cn/gtxxrpmehs.html

[O03] 加锁保护共享数据
来源：http://hz.dashuyun.cn/gtxyqoclbs.html

Py:   with lock: shared += 1
来源：http://hz.yj20258.top/gteyyvhjvd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nanxuanxn.top/gtnamuqtvv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cqqwz.cn/gtjnlkflej.html

TS:   // 同 JS
来源：http://hz.fzhhl.top/gtuqgruvze.html

Java: synchronized (this) { shared++; }
来源：http://hz.jiagoushi.top/gtsdzrwtsh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daria6918.cn/gtiqlomcqg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sufxvd.cn/gtqbzmmisv.html

C#:   lock (gate) { shared++; }
来源：http://hz.wangshuangyany.cn/gtakunnehu.html

[O04] 定义异步函数并等待
来源：http://hz.shzxlz.cn/gtkynwveqo.html

Py:   async def f():⏎    await g()
来源：http://hz.ybcxt.top/gtxpkfczlg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.aizwys.cn/gtiaoblowv.html

JS:   async function f() { await g(); }
来源：http://hz.chenlongwang.top/gtttivdyos.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.feifeiyinyue.top/gtdpxxobfm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yj20258888.top/gttqydyvdv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cqqwz.cn/gtagxfgxvv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenzaomai.com/gtskrxggkb.html

C#:   async Task F() { await G(); }
来源：http://hz.yongpay.top/gtebcypzxv.html

[O05] 并发执行并等待全部完成
来源：http://hz.kuanghao11.cn/gtqfwzgqni.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aibaodan.cn/gtghbgifsl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tianlin.xyz/gtoiuswoce.html

JS:   await Promise.all(tasks)
来源：http://hz.hnqzz.top/gtdzpofcdi.html

TS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gttvsprwzy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhengqikj.top/gtzyjtbuaq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hfpthk.cn/gtfqecvfjb.html

Ruby: threads.map(&:join)
来源：http://hz.jinyuanbaomall.cn/gtgczbmlor.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hywenlv.cn/gteyppdlao.html

[O06] 使用进程池
来源：http://hz.jinqigufen.top/gtvggxupft.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.meibo888.top/gtnepouhzg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zycfv.cn/gtpztvamfe.html

JS:   // child_process / cluster 模块
来源：http://hz.zdqjudy.top/gttpncyhud.html

TS:   // child_process / cluster 模块
来源：http://hz.fengsongda.top/gtedpeacwv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.52xcode.cn/gtdyzpnyul.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pengpengdd.cyou/gtbrxkvmkb.html

Ruby: // fork 块
来源：http://hz.wangshuangyany.cn/gtqiphifct.html

C#:   Parallel.For
来源：http://hz.gotoacloud.top/gtkxqjunox.html

================================================================================
来源：http://hz.dianchejie.cn/gtoqsnxvzs.html

P. 常用工具函数
来源：http://hz.hammf.cn/gthfhhbley.html

================================================================================
来源：http://hz.jianghu66.top/gttixfdnng.html

[P01] 生成 UUID
来源：http://hz.fengsongda.top/gtqbkcuccx.html

Py:   str(uuid.uuid4())
来源：http://hz.cashguo.top/gtodpeefrn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhoulong.xyz/gtcjixeydy.html

JS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtisfanszs.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtfnlirgqz.html

Java: UUID.randomUUID().toString()
来源：http://hz.hongshengwenyu.top/gtsswizpco.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xinyue.icu/gtdxtfxyrx.html

Ruby: SecureRandom.uuid
来源：http://hz.cheryme.top/gtetbvtdom.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenzaomai.com/gtnhzdurpt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.c1oappe.top/gtzvqgdaof.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gogol.net.cn/gttitambxm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.c1oappe.top/gtwvvjlbic.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ppjwa.cn/gtbefkdwci.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258888.top/gtxepblbwq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xinyue.icu/gthvzzgyek.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.quarkkingdee.top/gtuewiauih.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigufen.top/gtnpxjqjmk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jiagoushi.top/gtiqwsorpm.html

[P03] 生成短随机字符串
来源：http://hz.ppjwa.cn/gtszavtkly.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ivvv.top/gtmyjgnukl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhoulong.xyz/gtoktmipmf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tanke756.top/gtuinqhuri.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.52xcode.cn/gtfoabqyzm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.pengpengdd.cyou/gtngvexwax.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hfpthk.cn/gteuzqactw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigfzy.top/gtscselzds.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhijiandao.cn/gtxokdupqz.html

[P04] 求长度
来源：http://hz.aibaodan.cn/gtwecfpocf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tanke756.top/gtaocombet.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gtdzhemnhj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gtogkkgcex.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtlzihbghf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtxetcwylz.html

Go:   len(arr);  len(m)
来源：http://hz.zycfv.cn/gtoyolarqx.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gtdqdrifdx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yvedp.cn/gtscxmcdtc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dashuyun.cn/gttuvzrfmy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.316326.xyz/gtijzqacdy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenzaomai.com/gtqjsrxsza.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hywenlv.cn/gtpujwtpfn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hfpthk.cn/gtpmsqwmdy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj20258.top/gtbiqrkyto.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinghuilouyu.cn/gtasutxivf.html

Ruby: a == b
来源：http://hz.ydzc1.top/gtryadarck.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj202588.top/gtdujvsghs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zycfv.cn/gtxowabnse.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yvedp.cn/gtvwtrvvtz.html

PHP:  if (empty($x)) {}
来源：http://hz.zhongyouzk.top/gthgkghqda.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.52xcode.cn/gtsptrawbl.html

TS:   if (x == null) {}
来源：http://hz.yanxiufei.cn/gtkjlxamfc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hywenlv.cn/gtglblhynz.html

Go:   if x == nil {}
来源：http://hz.svipenyu.cn/gtdiwpwmjt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yonumen.top/gtlbngmfyf.html

C#:   if (x is null) {}
来源：http://hz.cheryme.top/gtpnrgphoe.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gtnddjsalo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.haohaochexian.top/gtgbucgidf.html

PHP:  // 手写时间戳比较
来源：http://hz.hammf.cn/gtxtxnfvbp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtginmmqfj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtwmuhadue.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigufen.top/gtnvqrzdnv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenzaomai.com/gtduxlvzzd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shanyushiyangtech.top/gtnknznytx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.316326.xyz/gthlcyccro.html

[P08] 处理浮点精度问题
来源：http://hz.jiagoushi.top/gtfubmfteu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jianghu66.top/gthzaaegcf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.iojbl.cn/gtmhvoszbl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ybcxt.top/gtjhxqwtsv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinqigufen.top/gtfpbixrzn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shanyushiyangtech.top/gtevhkieeo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinqigfzy.top/gtsryhvqie.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guowangkeji.top/gtjfoxikkx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ivvv.top/gtcofidiji.html

================================================================================
来源：http://hz.bjfxy.top/gtmgetdggk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xylfe.cn/gtbswnroqs.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtuacevqrt.html

[Q01] 创建表
来源：http://hz.guannengcc.top/gtziarvgvx.html

CREATE TABLE users (
来源：http://hz.iojbl.cn/gtjbmyptzo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtfsqebnio.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jqgufenzy.top/gtizctqwjz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shuidangran.top/gtmcophjuz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cheryme.top/gthznlhuhb.html

);
来源：http://hz.chenzaomai.com/gtldvmjwnv.html

[Q02] 创建带外键的表
来源：http://hz.snrcjt.cn/gttphcrcdo.html

CREATE TABLE orders (
来源：http://hz.hnqzz.top/gtdbuzeobz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtjjjobxhw.html

user_id INT NOT NULL,
来源：http://hz.cheryme.top/gtmbgwmjdx.html

amount DECIMAL(10, 2),
来源：http://hz.feifeiyinyue.top/gtdxmcuogo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yonumen.top/gtlusufayz.html

);
来源：http://hz.jinyuanbaomall.cn/gttfogrjem.html

[Q03] 增加列
来源：http://hz.0kj1m.cn/gtqcmpaseu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinghuilouyu.cn/gtohpujbwc.html

[Q04] 修改列类型
来源：http://hz.jinqigfzy.top/gtmlcrkzmp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.mhx1999.top/gtapfcmdjv.html

[Q05] 重命名列
来源：http://hz.shzxlz.cn/gtonjdvxlh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cqqwz.cn/gtfnklshkd.html

[Q06] 删除列
来源：http://hz.jinyuanbaomall.cn/gtvsejhnlk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinqigfzy.top/gtiwcnibit.html

[Q07] 删除表
来源：http://hz.dianchejie.cn/gtrbibkovu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj20258.top/gtifubrejb.html

[Q08] 创建普通索引
来源：http://hz.cqqwz.cn/gtsqxubkmc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.smart0.xyz/gtdmgeupew.html

[Q09] 创建唯一索引
来源：http://hz.ydzc1.top/gtlgatunhx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fzhhl.top/gthxqxnwjs.html

[Q10] 插入单行
来源：http://hz.zycfv.cn/gtrvasdlrt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.pycfn.com/gtkkixqnws.html

[Q11] 一次插入多行
来源：http://hz.ivvv.top/gtbwqnygtz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shangyingyoupin.top/gtoghzfsno.html

[Q12] 插入后取自增 ID
来源：http://hz.gotoacloud.top/gtksfsfefu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenlongwang.top/gtopwjumjo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.svipenyu.cn/gtzsjixalo.html

[Q13] 忽略重复插入
来源：http://hz.gaohongyu789.top/gttyzkmtnq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhiwuduotai.top/gtbvakrwzu.html

[Q14] 存在则更新（upsert）
来源：http://hz.guowangkeji.top/gtgnxrzxfm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangshuangyany.cn/gtqnctogjf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yangfankeji.com/gtfdrurtph.html

[Q15] 查询全部
来源：http://hz.yonumen.top/gtyejucjym.html


<!-- 参考信息 -->