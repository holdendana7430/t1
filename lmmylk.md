代发 wailian999

Java: public static void main(String[] args)
来源：http://hz.zycfv.cn/gtjcurcyhl.html

Go:   func main()
来源：http://hz.guowangkeji.top/gtccymwtdl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtopdjbang.html

C#:   static void Main(string[] args)
来源：http://hz.ywan-chungtsiang.top/gthjscfsqt.html

[M08] 获取系统与运行时信息
来源：http://hz.redwolf501.top/gtxelsldfy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.kuanghao11.cn/gtumjzkjwq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sysykeji.top/gtjuxarcuy.html

JS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gtxpbtatbp.html

TS:   process.platform;  process.version
来源：http://hz.aizwys.cn/gtzpmogsjj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.snrcjt.cn/gtjkfacmgu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sweek.top/gtvrjtjrap.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yuanzhike.top/gtecmpxmsk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuanzx.com/gtdxathdrj.html

================================================================================
来源：http://hz.ehwqpu.com/gtzbsihqpg.html

N. 数据结构与算法
来源：http://hz.hywenlv.cn/gtmnzjntfg.html

================================================================================
来源：http://hz.ehwqpu.com/gtwemufcnm.html

[N01] 二分查找（有序数组）
来源：http://hz.gzhubu.top/gtxiolwlqd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtempqqsxj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.quarkkingdee.top/gtibdsmajx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gtvosaukfi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hfpthk.cn/gtujhupawl.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yanxiufei.cn/gtphtewaab.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.9152youxi.cn/gtyuyydtof.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.redwolf501.top/gtluriwctu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.c1oappe.top/gtyakvcsyi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxinkj.top/gtdyscvfti.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuxming.cn/gtlynrpjld.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.mhx1999.top/gtusjixdyb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gtlupfawqg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtnkeffyid.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dianchejie.cn/gtpvtrvnyb.html

Go:   slices.Sort(arr)
来源：http://hz.yonumen.top/gtzjennxcj.html

Ruby: arr.sort
来源：http://hz.sweek.top/gtpveznuyh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnxiangtu.top/gtyeqmveca.html

[N03] 快速排序（分治示例）
来源：http://hz.yongpay.top/gtpwweifmw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yanxiufei.cn/gtjiigkhkd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.andypj.xyz/gtlggihyyi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtlmvbayas.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtyjuoavwt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.birdmap.top/gtxmeqbpjg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxuanxn.top/gtfndcarmv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yonumen.top/gtjyfeszks.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhixingplan.top/gtyyhjgxdx.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gtqllsjgoj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtuoraxcxj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shangyingyoupin.top/gtwihfcbrh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtpfdypief.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtyrkqclpp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuetiantiany.cn/gtbakzhubg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinyuanbaomall.cn/gtaxxbrmpb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pengpengdd.cyou/gtsvdpakzv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jianghu66.top/gtrshbjxvc.html

[N05] 最大公约数
来源：http://hz.9152youxi.cn/gtypfrnemn.html

Py:   math.gcd(a, b)
来源：http://hz.cheryme.top/gtbccjkzpb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhijiandao.cn/gtvbasddul.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sweek.top/gtbldjsafa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fengsongda.top/gtdonmsqmj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.0kj1m.cn/gtndccoejk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.snrcjt.cn/gtnpelhege.html

Ruby: a.gcd(b)
来源：http://hz.jiagoushi.top/gtoiirqpoc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cashguo.top/gtxbtpfnzv.html

[N06] 判断回文字符串
来源：http://hz.vqdsnc.cn/gtjmbdorem.html

Py:   s == s[::-1]
来源：http://hz.nanxuanxn.top/gtbvzczdzk.html

PHP:  $s === strrev($s);
来源：http://hz.iojbl.cn/gtnoqtbyho.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtvivsotsu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtmlpyymdi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.bjfxy.top/gtwureqnzd.html

Go:   // 双指针从两端比较
来源：http://hz.ybcxt.top/gtqoqjcxpt.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangkeji.top/gtsayuvbvl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.meibo888.top/gtnpltyfdr.html

[N07] 两数之和（返回下标）
来源：http://hz.jqgufenzy.top/gtirettolb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.redwolf501.top/gtzoynqtha.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jiagoushi.top/gttbliuxvo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinqigufen.top/gtuydmwobe.html

TS:   // 手写 Map<string, number>
来源：http://hz.52xcode.cn/gtqskqvlux.html

Java: // 手写 HashMap
来源：http://hz.wangshuangyany.cn/gtonbrgnoe.html

Go:   // 手写 map[int]int
来源：http://hz.aibaodan.cn/gtyebkmjwh.html

Ruby: // 手写 Hash
来源：http://hz.ppjwa.cn/gttomuxsiv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.havefunace.top/gtficsimoz.html

[N08] 生成全排列
来源：http://hz.tanke756.top/gtafbuntdo.html

Py:   itertools.permutations(arr)
来源：http://hz.aibaodan.cn/gtwutuenca.html

PHP:  // 手写递归交换
来源：http://hz.zhaomingkeji.xyz/gtlacxizve.html

JS:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtosgovjgt.html

TS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtjtiiqhyc.html

Java: // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtuxtoyfld.html

Go:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtsaqfmysp.html

Ruby: arr.permutation.to_a
来源：http://hz.sufxvd.cn/gtogwgygja.html

C#:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gteeqymamv.html

[N09] 栈与队列
来源：http://hz.pycfn.com/gtokshvgtv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xinyue.icu/gttapehvtn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fzhhl.top/gtyqnjfsyp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gaohongyu789.top/gtyoteoiod.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fzhhl.top/gthezjroqb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zdqjudy.top/gtfszznnso.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ppjwa.cn/gtobbxjmkm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nwbrower.top/gtqpgmeonn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangkeji.top/gtdmgnedtr.html

[N10] 链表节点定义
来源：http://hz.jinqigfzy.top/gtgnkxcaxl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jiagoushi.top/gtwazxwnyn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cucudq.cn/gtpbhxzaeo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.quarkkingdee.top/gtectogshb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigufen.top/gtmytsnlzj.html

Java: class Node { int v; Node next; }
来源：http://hz.jianghu66.top/gtbkikooln.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.aizwys.cn/gtqwevfhab.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xinyue.icu/gtasmyzsuw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.vqdsnc.cn/gtosoilyvs.html

[N11] 二叉树中序遍历
来源：http://hz.zhoulong.xyz/gtmddfthdh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hammf.cn/gtjqdlihfu.html

PHP:  // 手写递归函数
来源：http://hz.cqqwz.cn/gtbfpjkial.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj202588.top/gtxbdblujm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gthcovreqz.html

Java: // 手写递归
来源：http://hz.vqdsnc.cn/gtujqqmnhx.html

Go:   // 手写递归
来源：http://hz.yvedp.cn/gtssvbkdlv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.bjfxy.top/gtinqcuaqx.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gtgwcpjybd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zdqjudy.top/gtulvimsmh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhaomingkeji.xyz/gtypjysqpg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zycfv.cn/gtnblkocbs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtcirwsyjm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtjaagchxk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtgaxdmngi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.kuanghao11.cn/gtjunurcue.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.vqdsnc.cn/gtfuwaownf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenzaomai.com/gtususebdy.html

================================================================================
来源：http://hz.yongpay.top/gtdezhvwzg.html

O. 并发与异步
来源：http://hz.xuetiantiany.cn/gtlkrzgfad.html

================================================================================
来源：http://hz.snrcjt.cn/gtoryatbgd.html

[O01] 启动一个线程
来源：http://hz.yj202588.top/gtjyqgxihz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.redwolf501.top/gtsflnyken.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ehwqpu.com/gtiknjomrm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tanke756.top/gttagyidzi.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gtklkxjtsa.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxinkj.top/gtweobulep.html

Go:   go f()
来源：http://hz.smart0.xyz/gtmrjypauv.html

Ruby: Thread.new { f }
来源：http://hz.snrcjt.cn/gtgcwjntyv.html

C#:   Task.Run(() => F());
来源：http://hz.havefunace.top/gthaveeiuk.html

[O02] 使用线程池
来源：http://hz.jqgfzy.top/gtddzcvcdv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yonumen.top/gtudaufwuf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.haohaochexian.top/gtevsomvqc.html

JS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gtmkznxvvr.html

TS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gtclstdkzh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nanxinkj.top/gtgdacyale.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangshuangyany.cn/gtvaxlxzfn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.bjfxy.top/gtiusdmeey.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.quarkkingdee.top/gtmbezghye.html

[O03] 加锁保护共享数据
来源：http://hz.316326.xyz/gtlbavsmka.html

Py:   with lock: shared += 1
来源：http://hz.jiagoushi.top/gtyjgwkfeq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhijiandao.cn/gtjhvdqtln.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.316326.xyz/gtpwlszfok.html

TS:   // 同 JS
来源：http://hz.jlsjyb.cn/gthslnnwob.html

Java: synchronized (this) { shared++; }
来源：http://hz.xylfe.cn/gtzzfseopd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hammf.cn/gtugtvmbew.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nanxinkj.top/gtzpwfczyx.html

C#:   lock (gate) { shared++; }
来源：http://hz.0kj1m.cn/gtsevisgow.html

[O04] 定义异步函数并等待
来源：http://hz.zhoulong.xyz/gtnodxdjhz.html

Py:   async def f():⏎    await g()
来源：http://hz.xylfe.cn/gtnsljdieg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yongpay.top/gtbtjoizrf.html

JS:   async function f() { await g(); }
来源：http://hz.xziqi.cn/gtyjfexssm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tianlin.xyz/gtfdrkbtey.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.wangdashe.top/gtpdimynrv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.wangdashe.top/gtmamawfxh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cqqwz.cn/gtdyhnckpr.html

C#:   async Task F() { await G(); }
来源：http://hz.ywan-chungtsiang.top/gtulmhonii.html

[O05] 并发执行并等待全部完成
来源：http://hz.cqqwz.cn/gtzwbfkaoj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zycfv.cn/gtpaglagko.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sxryk.cn/gtfdalmdeo.html

JS:   await Promise.all(tasks)
来源：http://hz.nanxinkj.top/gtsyyfsbtp.html

TS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gtuucudwed.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yongpay.top/gtpluervng.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xziqi.cn/gtobnttgkw.html

Ruby: threads.map(&:join)
来源：http://hz.jinghuilouyu.cn/gtlbgledpj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ywan-chungtsiang.top/gtrkfzvpcm.html

[O06] 使用进程池
来源：http://hz.chenlongwang.top/gtwckiqvia.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenlongwang.top/gtcnotaxhi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jiagoushi.top/gtqowmwnll.html

JS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gthwzoupco.html

TS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtlsaoyhgw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tian-w.cn/gtizyjpaxz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangdashe.top/gtypmjivoz.html

Ruby: // fork 块
来源：http://hz.0kj1m.cn/gtctjjhopr.html

C#:   Parallel.For
来源：http://hz.ydzc1.top/gtvavnawjp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxoouetkn.html

P. 常用工具函数
来源：http://hz.tianlin.xyz/gtyeobonoc.html

================================================================================
来源：http://hz.cdnleiting.top/gtokldhptz.html

[P01] 生成 UUID
来源：http://hz.shanyushiyangtech.top/gtmdjxtjwx.html

Py:   str(uuid.uuid4())
来源：http://hz.jinqigfzy.top/gttgxbmmmh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xinyue.icu/gtuaolqewh.html

JS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtgbvsuiio.html

TS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtwnljedpo.html

Java: UUID.randomUUID().toString()
来源：http://hz.svipenyu.cn/gtuyqiydbb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ywan-chungtsiang.top/gtefdfvmlz.html

Ruby: SecureRandom.uuid
来源：http://hz.dashuyun.cn/gtswjzvowj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.smart0.xyz/gtxuntktqr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sufxvd.cn/gtaozvtxeq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shzxlz.cn/gtkhumihsl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gogol.net.cn/gtuzmqnfei.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.iojbl.cn/gthbekgrwv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.kuanghao11.cn/gtpsmcztrr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinghuilouyu.cn/gtlsuypebr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ehwqpu.com/gtmxarzzrl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tanke756.top/gtkdinpxpi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxuanxn.top/gtsgytfrsr.html

[P03] 生成短随机字符串
来源：http://hz.shuidangran.top/gtihsvdzlo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sweek.top/gtukrlgrtm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yongpay.top/gtfcncyxxw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangshuangyany.cn/gtsmkrrbcz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydjk.org.cn/gtmsroskcg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.aibaodan.cn/gtnpycufwd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.quarkkingdee.top/gtztiirkly.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tian-w.cn/gtppbtesqh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ydjk.org.cn/gtyevbvseq.html

[P04] 求长度
来源：http://hz.chenzaomai.com/gtnuxzrnnr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sxryk.cn/gtgqainygf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhengqikj.top/gtsvoidlpa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtucjtjsei.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtwcphykwn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yongpay.top/gtsgfpnqio.html

Go:   len(arr);  len(m)
来源：http://hz.feifeiyinyue.top/gtfjebhtas.html

Ruby: x.length;  x.size
来源：http://hz.yj20258.top/gtgvbducdh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shanyushiyangkeji.top/gtsrnysksw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yonumen.top/gtkvuzninm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hnqzz.top/gthbrkxdbk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fzhhl.top/gtepautphx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jyoumei.cn/gtgcrewlht.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cqqwz.cn/gtkzxgskux.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.tian-w.cn/gtappzzyrl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hnqzz.top/gtgjdacciy.html

Ruby: a == b
来源：http://hz.meibo888.top/gtsjmkmeos.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.pycfn.com/gtbwdwyaig.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenzaomai.com/gtpiujnpfo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yuxming.cn/gtmpcpshab.html

PHP:  if (empty($x)) {}
来源：http://hz.hammf.cn/gtgxwwpdoi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.dashuyun.cn/gthnkiesft.html

TS:   if (x == null) {}
来源：http://hz.fengsongda.top/gtbfotblyz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj20258.top/gthtfnwdrr.html

Go:   if x == nil {}
来源：http://hz.yj20258888.top/gthdcwbeeo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cqqwz.cn/gteqzsyzro.html

C#:   if (x is null) {}
来源：http://hz.52xcode.cn/gtuugwnlzp.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gttfewyokv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.aizwys.cn/gthjjalpdt.html

PHP:  // 手写时间戳比较
来源：http://hz.feifeiyinyue.top/gtwvwbtubq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtqiaokeeo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gthqiituha.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zdqjudy.top/gtbksbcifm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.smart0.xyz/gtvucvveub.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.c1oappe.top/gtleskjuyc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhijiandao.cn/gtptoirupz.html

[P08] 处理浮点精度问题
来源：http://hz.smart0.xyz/gteegbjwgy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhixingplan.top/gtxbidgahk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.quarkkingdee.top/gtauahkywg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.aizwys.cn/gtxrwazftr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nwbrower.top/gtkbqdircw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.quarkkingdee.top/gtpqqagzvg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ppjwa.cn/gteifmfspj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shzxlz.cn/gtgaikwcse.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cheryme.top/gtxqtugntj.html

================================================================================
来源：http://hz.redwolf501.top/gtbfzicmzx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.svipenyu.cn/gtfwvdizzz.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtzmqrrzqt.html

[Q01] 创建表
来源：http://hz.shzxlz.cn/gtxauhemyn.html

CREATE TABLE users (
来源：http://hz.yonumen.top/gthxsfgjoy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhixingplan.top/gtzdffmvnl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhoulong.xyz/gtuureadmo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cheryme.top/gtidvfxhbu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gtczsbbjgw.html

);
来源：http://hz.dashuyun.cn/gthnrsjkdh.html

[Q02] 创建带外键的表
来源：http://hz.316326.xyz/gttjnkgulg.html

CREATE TABLE orders (
来源：http://hz.hysaishi.cn/gtkomdjhbu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gtswwujqaf.html

user_id INT NOT NULL,
来源：http://hz.xuanzx.com/gthmdpcclk.html

amount DECIMAL(10, 2),
来源：http://hz.andypj.xyz/gtnwbabpti.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hongshengwenyu.top/gtdsfmsrqz.html

);
来源：http://hz.vqdsnc.cn/gtspxllrbr.html

[Q03] 增加列
来源：http://hz.xziqi.cn/gtpqbcoequ.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gotoacloud.top/gtugdcyotj.html

[Q04] 修改列类型
来源：http://hz.zhiwuduotai.top/gtdseeozoh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.havefunace.top/gtbquvefhb.html

[Q05] 重命名列
来源：http://hz.yonumen.top/gtorehoxpm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hammf.cn/gtwwvgxtwc.html

[Q06] 删除列
来源：http://hz.sufxvd.cn/gtbhsfbupo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenlongwang.top/gterqqoola.html

[Q07] 删除表
来源：http://hz.andypj.xyz/gtjurviqux.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gzhubu.top/gtapiawktl.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gtvdtqiygr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tanke756.top/gtrweqacwq.html

[Q09] 创建唯一索引
来源：http://hz.zhixingplan.top/gtjexixcfj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sufxvd.cn/gtnyevlwww.html

[Q10] 插入单行
来源：http://hz.yanxiufei.cn/gtavgvltoi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jlsjyb.cn/gtqiycnosn.html

[Q11] 一次插入多行
来源：http://hz.tian-w.cn/gtyajnldjt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhijiandao.cn/gtgtnpcmki.html

[Q12] 插入后取自增 ID
来源：http://hz.shangyingyoupin.top/gtjarpmdpd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xinyue.icu/gtvlfzqovb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cheryme.top/gtkvtipvtt.html

[Q13] 忽略重复插入
来源：http://hz.ppjwa.cn/gtgmsurpnx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gogol.net.cn/gtdredumvl.html

[Q14] 存在则更新（upsert）
来源：http://hz.sweek.top/gtnadeeltv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhijiandao.cn/gtzfuxyfsk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jiagoushi.top/gtlkpxjkns.html

[Q15] 查询全部
来源：http://hz.yangfankeji.com/gtorplrvzk.html


<!-- 参考信息 -->