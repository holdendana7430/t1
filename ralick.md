代发 wailian999

Java: public static void main(String[] args)
来源：http://hz.aibaodan.cn/gtgvlmutuu.html

Go:   func main()
来源：http://hz.zhengqikj.top/gtjrnjmzbr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtdjthahtv.html

C#:   static void Main(string[] args)
来源：http://hz.gaohongyu789.top/gtsnwouups.html

[M08] 获取系统与运行时信息
来源：http://hz.yanxiufei.cn/gtprgwslup.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hysaishi.cn/gtgprvngex.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tian-w.cn/gtcvbcaeri.html

JS:   process.platform;  process.version
来源：http://hz.sysykeji.top/gtniuniohu.html

TS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtxeipfqha.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fzhhl.top/gtfivdufnv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jlsjyb.cn/gticlnxxmb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jiagoushi.top/gteblrprbn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhaomingkeji.xyz/gtaxyhbbda.html

================================================================================
来源：http://hz.0kj1m.cn/gtltovfmlk.html

N. 数据结构与算法
来源：http://hz.mhx1999.top/gtxvcxwxnc.html

================================================================================
来源：http://hz.smart0.xyz/gtvnvrdkpt.html

[N01] 二分查找（有序数组）
来源：http://hz.tianlin.xyz/gtnzskelih.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gogol.net.cn/gtepxspypm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydjk.org.cn/gtwbzloprz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtbwdtwfxc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuanzhike.top/gtprnjrnld.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.fengsongda.top/gthhoevyjg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cqqwz.cn/gtyuyicjki.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtahpwbhbe.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jianghu66.top/gtubserqfs.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jiagoushi.top/gtkiryerjg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtepzjpcsp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hongshengwenyu.top/gtuvcuisow.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtsmgltjqw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtrxjyhhtq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.birdmap.top/gtcgotdgmr.html

Go:   slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtruohdlso.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtfppzyhpj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cdnleiting.top/gtwmchlsgs.html

[N03] 快速排序（分治示例）
来源：http://hz.tanke756.top/gtnftmginl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.bjfxy.top/gtscbmqpxy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.havefunace.top/gtluqbawuf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jlsjyb.cn/gtawuviqgl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtsvujxyas.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nanxuanxn.top/gtjaqippjp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xylfe.cn/gtsmcuybwk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.c1oappe.top/gtwwntemdo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gtqtoitcop.html

[N04] 斐波那契数列
来源：http://hz.jinqigufen.top/gtaqlvkfpu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gthvnuzwlw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tanke756.top/gtotqcduqp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtwfdudzaq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.bjfxy.top/gtmuqfzwnm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.aibaodan.cn/gtvwooaqmp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yueranfly.top/gtqqzvlvhy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.redwolf501.top/gtwixnokoh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.redwolf501.top/gtfrlgpiid.html

[N05] 最大公约数
来源：http://hz.yangfankeji.com/gtkktepnzn.html

Py:   math.gcd(a, b)
来源：http://hz.hysaishi.cn/gtnjxnubqa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.kuanghao11.cn/gtylkrgdju.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gtymkvnhvr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtydrynfkl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.kuanghao11.cn/gtmhibkgmu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gttrauogoj.html

Ruby: a.gcd(b)
来源：http://hz.0kj1m.cn/gtyexglrdt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gtmlxnjfrn.html

[N06] 判断回文字符串
来源：http://hz.haohaochexian.top/gtpjbyhnwt.html

Py:   s == s[::-1]
来源：http://hz.dashuyun.cn/gtkhtmypvu.html

PHP:  $s === strrev($s);
来源：http://hz.chenlongwang.top/gtfccmnktx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtililekbm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtdegyaeae.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.snrcjt.cn/gtwuoxxmhn.html

Go:   // 双指针从两端比较
来源：http://hz.ivvv.top/gtykxvchvr.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangtech.top/gtakwapyaa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nanxinkj.top/gtjtxiqwei.html

[N07] 两数之和（返回下标）
来源：http://hz.xingfuxueyuan.xyz/gtplsokbhw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guowangkeji.top/gtiqqwyxym.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.wangdashe.top/gtisysnyln.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.bjfxy.top/gtuxkzllmm.html

TS:   // 手写 Map<string, number>
来源：http://hz.0kj1m.cn/gtdhbvdfjh.html

Java: // 手写 HashMap
来源：http://hz.jqgfzy.top/gtibnxoysz.html

Go:   // 手写 map[int]int
来源：http://hz.jqgufenzy.top/gtjouxbmfp.html

Ruby: // 手写 Hash
来源：http://hz.ivvv.top/gtltnopnjr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.mhx1999.top/gtlsibdtpb.html

[N08] 生成全排列
来源：http://hz.bjfxy.top/gtpjwivzve.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangtech.top/gtmmujmvls.html

PHP:  // 手写递归交换
来源：http://hz.vqdsnc.cn/gtvbtfyjgr.html

JS:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtoshheyvf.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtrcrgsowt.html

Java: // 手写回溯递归
来源：http://hz.yueranfly.top/gtyooznfzb.html

Go:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtppmqgbnr.html

Ruby: arr.permutation.to_a
来源：http://hz.havefunace.top/gtqmynoyva.html

C#:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtcnfennkz.html

[N09] 栈与队列
来源：http://hz.jqgfzy.top/gtaxtkudlb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtdvppehem.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydzc1.top/gtgtbrgpwr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cqqwz.cn/gtflobavjm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ehwqpu.com/gtwvahknpr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daxiang520.top/gtlncdgwlt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.birdmap.top/gtlusjpypj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tianlin.xyz/gtgcbsrbsj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zycfv.cn/gtmodyaxme.html

[N10] 链表节点定义
来源：http://hz.yj20258.top/gtdvrhgntl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.birdmap.top/gtrysvomac.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sysykeji.top/gtrsyairlw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cdnleiting.top/gtsuncejtl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dianchejie.cn/gtwuxncfku.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gttobtoucm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.snrcjt.cn/gtxhmiwben.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.feifeiyinyue.top/gtrefvlfwt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cashguo.top/gtyhmpmdic.html

[N11] 二叉树中序遍历
来源：http://hz.gotoacloud.top/gtnvftijai.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nanxuanxn.top/gtysoxetjn.html

PHP:  // 手写递归函数
来源：http://hz.jqgfzy.top/gtlrqmoprx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtnbmqzcyw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigfzy.top/gtxfemrtwn.html

Java: // 手写递归
来源：http://hz.jinqigufen.top/gthyfwgnxg.html

Go:   // 手写递归
来源：http://hz.zhiwuduotai.top/gtjsllawdu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tanke756.top/gtxwwyvowk.html

C#:   // 手写递归
来源：http://hz.redwolf501.top/gtqnozjuxa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tanke756.top/gtiaspvlay.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yangfankeji.com/gtrqkfzmrl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.316326.xyz/gtrmlkeueb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jiagoushi.top/gtryqcdvtr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gtsdzthbhq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtlipfcdmq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.redwolf501.top/gtprxerkrv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yuanzhike.top/gttealyjrl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gttsjgkfwm.html

================================================================================
来源：http://hz.mhx1999.top/gttlrdrgmp.html

O. 并发与异步
来源：http://hz.nwbrower.top/gtthmusrbh.html

================================================================================
来源：http://hz.yj202588.top/gtwjjacmul.html

[O01] 启动一个线程
来源：http://hz.hfpthk.cn/gtyjtgrucc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yongpay.top/gtqouwwsud.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tanke756.top/gtzlcchwqm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.52xcode.cn/gtrumjmles.html

TS:   // 同 JS
来源：http://hz.shangyingyoupin.top/gtqmyjbkxe.html

Java: new Thread(() -> f()).start()
来源：http://hz.yonumen.top/gtypeoficy.html

Go:   go f()
来源：http://hz.ppjwa.cn/gtfemtungt.html

Ruby: Thread.new { f }
来源：http://hz.xuetiantiany.cn/gtmmbpnbei.html

C#:   Task.Run(() => F());
来源：http://hz.dashuyun.cn/gthvjlajxr.html

[O02] 使用线程池
来源：http://hz.gzhubu.top/gtpbwbxora.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.mhx1999.top/gtfspsqfih.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.kuanghao11.cn/gthfnehdbl.html

JS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtlorbmhtc.html

TS:   // worker_threads 线程池
来源：http://hz.ivvv.top/gtczlfakrc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.52xcode.cn/gtlemyhntt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xingfuxueyuan.xyz/gtwjktrjoq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuxming.cn/gtkvllcafc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nanxinkj.top/gtrtfpofit.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258888.top/gtogrttnkx.html

Py:   with lock: shared += 1
来源：http://hz.yuanzhike.top/gtnmgnostv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhongyouzk.top/gtstsymcqj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangshuangyany.cn/gtwyareyit.html

TS:   // 同 JS
来源：http://hz.jqgufenzy.top/gtfdgydahi.html

Java: synchronized (this) { shared++; }
来源：http://hz.xinyue.icu/gtfouxdgcg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gzhubu.top/gtytgrhfik.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zycfv.cn/gtorctcdvl.html

C#:   lock (gate) { shared++; }
来源：http://hz.jiagoushi.top/gtxzftxset.html

[O04] 定义异步函数并等待
来源：http://hz.bjfxy.top/gtvhnjbtjg.html

Py:   async def f():⏎    await g()
来源：http://hz.yj202588.top/gtixqzhrqn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuxming.cn/gtkltggnbc.html

JS:   async function f() { await g(); }
来源：http://hz.sweek.top/gtqnpmhofh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gteijxeqhr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.vqdsnc.cn/gtocrflcyl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xinyue.icu/gtawddptjc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yangfankeji.com/gtsirunftc.html

C#:   async Task F() { await G(); }
来源：http://hz.jinqigfzy.top/gtrpozuxzy.html

[O05] 并发执行并等待全部完成
来源：http://hz.cashguo.top/gtllnqbpgc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jiagoushi.top/gtdpqkfwrg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yueranfly.top/gtawnynymz.html

JS:   await Promise.all(tasks)
来源：http://hz.nanxuanxn.top/gtuwyhqyxx.html

TS:   await Promise.all(tasks)
来源：http://hz.pengpengdd.cyou/gttjrooozi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sysykeji.top/gtqpmhnufs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jianghu66.top/gtafkkmsce.html

Ruby: threads.map(&:join)
来源：http://hz.wangdashe.top/gtsuiytfqc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cucudq.cn/gtgebuokss.html

[O06] 使用进程池
来源：http://hz.gzhubu.top/gtnfpqfjrw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnqzz.top/gtwmafsung.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sufxvd.cn/gtkylesahe.html

JS:   // child_process / cluster 模块
来源：http://hz.wangshuangyany.cn/gtyssgybqg.html

TS:   // child_process / cluster 模块
来源：http://hz.hammf.cn/gtpsuxjbhn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenzaomai.com/gtnbikbdtq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fzhhl.top/gtoiootkgb.html

Ruby: // fork 块
来源：http://hz.hfpthk.cn/gtagbhorpr.html

C#:   Parallel.For
来源：http://hz.shzxlz.cn/gtglsnbngn.html

================================================================================
来源：http://hz.yuxming.cn/gtjrzukkdc.html

P. 常用工具函数
来源：http://hz.mhx1999.top/gtfumbekyl.html

================================================================================
来源：http://hz.daxiang520.top/gtedpyxnex.html

[P01] 生成 UUID
来源：http://hz.hnqzz.top/gtraasjuoo.html

Py:   str(uuid.uuid4())
来源：http://hz.xuetiantiany.cn/gtdshzncre.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.snrcjt.cn/gtwrraynze.html

JS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtkbhszaoh.html

TS:   crypto.randomUUID()
来源：http://hz.yj20258888.top/gtelmehsmq.html

Java: UUID.randomUUID().toString()
来源：http://hz.sysykeji.top/gtfysqjstg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jiagoushi.top/gtqnfxglpn.html

Ruby: SecureRandom.uuid
来源：http://hz.ydzc1.top/gtsyrsceho.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yonumen.top/gtiwdpadmv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.pengpengdd.cyou/gtbtxbsmfj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258888.top/gtkpjfgyhc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ivvv.top/gtgkusxjaq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ybcxt.top/gtdvgmedsa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xinyue.icu/gtcktnsggv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.fengsongda.top/gtfhalsxhk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinyuanbaomall.cn/gttzqcrnoh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tian-w.cn/gtbjpuabbi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.aizwys.cn/gttxilqnvf.html

[P03] 生成短随机字符串
来源：http://hz.hfpthk.cn/gtvdufpfcp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydzc1.top/gtczsyglwq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnqzz.top/gtchoveqta.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtrkwgoyly.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtuzybvini.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cheryme.top/gtrxtgujhg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgufenzy.top/gtxairtedw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tian-w.cn/gthakrfaoz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258.top/gtkoxsycco.html

[P04] 求长度
来源：http://hz.sweek.top/gtosshmonn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj202588.top/gtpbsxwlmq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtrhakbecu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtngfcfxvv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.9152youxi.cn/gtrctfugkm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.vqdsnc.cn/gtpttxuyqj.html

Go:   len(arr);  len(m)
来源：http://hz.feifeiyinyue.top/gttwwljsuj.html

Ruby: x.length;  x.size
来源：http://hz.jinqigufen.top/gtanionzkt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.0kj1m.cn/gtvxfnkugl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj20258.top/gtgljprohp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gotoacloud.top/gtinxqkqie.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.bjfxy.top/gtxmrhmhog.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hfpthk.cn/gttgaaezll.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cashguo.top/gtresskkij.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ydzc1.top/gtxgyislvc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhoulong.xyz/gtwelbbnyu.html

Ruby: a == b
来源：http://hz.ivvv.top/gtvutqwsxl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nanxuanxn.top/gtabfbrrwy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fengsongda.top/gtjsbqpadm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jqgfzy.top/gtvgnkuyhf.html

PHP:  if (empty($x)) {}
来源：http://hz.cdnleiting.top/gthieuyqom.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.svipenyu.cn/gtnhacsuua.html

TS:   if (x == null) {}
来源：http://hz.shzxlz.cn/gtilqmbtgs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenlongwang.top/gtfcrbctcc.html

Go:   if x == nil {}
来源：http://hz.ppjwa.cn/gtoymnxjnq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zdqjudy.top/gtbvnntcbs.html

C#:   if (x is null) {}
来源：http://hz.svipenyu.cn/gtwsgbjlmn.html

[P07] 防抖与节流
来源：http://hz.ppjwa.cn/gtgelqxkug.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.52xcode.cn/gtvylxudsy.html

PHP:  // 手写时间戳比较
来源：http://hz.wangdashe.top/gttudtvqcj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtjmvpvjql.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtjxwihkmv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xuetiantiany.cn/gtrjnpqjuj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sysykeji.top/gtpyggumxn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pengpengdd.cyou/gtoqkadjeb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.havefunace.top/gtxvokrtvh.html

[P08] 处理浮点精度问题
来源：http://hz.xingfuxueyuan.xyz/gtzfajxwcd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhengqikj.top/gtirpjctjx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.0kj1m.cn/gtsaziinsg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.c1oappe.top/gtyjygrblv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gogol.net.cn/gtojnjcelz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gzhubu.top/gtdoynqyug.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.bjfxy.top/gttsrbcree.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.fengsongda.top/gtmwbvbnhb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.iojbl.cn/gtupvyloch.html

================================================================================
来源：http://hz.andypj.xyz/gtrdsrnrtn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.mhx1999.top/gteuagamiy.html

================================================================================
来源：http://hz.zycfv.cn/gtkkyhvlqg.html

[Q01] 创建表
来源：http://hz.ppjwa.cn/gtcbboekyu.html

CREATE TABLE users (
来源：http://hz.redwolf501.top/gtnwirvitv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtqgielvod.html

name VARCHAR(50) NOT NULL,
来源：http://hz.vqdsnc.cn/gtxckeicve.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aibaodan.cn/gtqajuvpip.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuxming.cn/gtxfqiitaf.html

);
来源：http://hz.xziqi.cn/gtdzabknjj.html

[Q02] 创建带外键的表
来源：http://hz.gaohongyu789.top/gtkpauygkz.html

CREATE TABLE orders (
来源：http://hz.shuidangran.top/gtiaxokusw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gtmftjkfjm.html

user_id INT NOT NULL,
来源：http://hz.yj202588.top/gttbmdkhaa.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigfzy.top/gtwvnkcwlr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hnxiangtu.top/gtgdodpuwi.html

);
来源：http://hz.xingfuxueyuan.xyz/gtrcekttzy.html

[Q03] 增加列
来源：http://hz.xylfe.cn/gttjvmnrkj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sufxvd.cn/gtohdegkmr.html

[Q04] 修改列类型
来源：http://hz.mhx1999.top/gtymvslzgy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ybcxt.top/gtobntrlzg.html

[Q05] 重命名列
来源：http://hz.hywenlv.cn/gtprrnsafk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258.top/gtfbvqwuhi.html

[Q06] 删除列
来源：http://hz.52xcode.cn/gtwmsekfos.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zdqjudy.top/gtjyuijolf.html

[Q07] 删除表
来源：http://hz.hfpthk.cn/gtijcfjgzl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangdashe.top/gtzkvyvzem.html

[Q08] 创建普通索引
来源：http://hz.yuanzhike.top/gtpgdwcanh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zycfv.cn/gttqsucovp.html

[Q09] 创建唯一索引
来源：http://hz.iojbl.cn/gtpbdvypzv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xziqi.cn/gtrcglljtz.html

[Q10] 插入单行
来源：http://hz.xziqi.cn/gtqvmlzaai.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuxming.cn/gtsddhpurj.html

[Q11] 一次插入多行
来源：http://hz.mhx1999.top/gtmualeojh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangdashe.top/gtlogftsdc.html

[Q12] 插入后取自增 ID
来源：http://hz.cheryme.top/gtjncnojjs.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuxming.cn/gtxdgbpgqn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhijiandao.cn/gtxpmjzhfd.html

[Q13] 忽略重复插入
来源：http://hz.316326.xyz/gtzdjfvioq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhengqikj.top/gtlzzcxjao.html

[Q14] 存在则更新（upsert）
来源：http://hz.hywenlv.cn/gtmcgvfbzg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fzhhl.top/gtnshunmdr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hnxiangtu.top/gtygcdzvut.html

[Q15] 查询全部
来源：http://hz.havefunace.top/gtfawjcopg.html


<!-- 参考信息 -->