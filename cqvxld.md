代发 wailian999

[M08] 获取系统与运行时信息
来源：http://hz.chenzaomai.com/gtsfvxetqm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.kuanghao11.cn/gtpumlzscs.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.aizwys.cn/gtaruoavoh.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtkxtglvqz.html

TS:   process.platform;  process.version
来源：http://hz.xinyue.icu/gtfuvzigvf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yonumen.top/gtqdqefxff.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guowangkeji.top/gtdqydolgw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.iojbl.cn/gtzcsmtiit.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangkeji.top/gtwgwceqqy.html

================================================================================
来源：http://hz.shzxlz.cn/gtbdeleics.html

N. 数据结构与算法
来源：http://hz.ydzc1.top/gteazehiba.html

================================================================================
来源：http://hz.sxryk.cn/gtnekpjkkn.html

[N01] 二分查找（有序数组）
来源：http://hz.zdqjudy.top/gtbsdwxvav.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenlongwang.top/gtwwkqvuns.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.havefunace.top/gttjgfrzck.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guannengcc.top/gtzxufhjpa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yvedp.cn/gtuyvauhxt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yvedp.cn/gtjgqkisge.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.mhx1999.top/gtutwawicy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hongshengwenyu.top/gtzmgqzrjx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hammf.cn/gterkwhxam.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.316326.xyz/gtvgpuzisq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtwtbqtydh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.snrcjt.cn/gtqidkrkau.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtaibflejc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtxqmarvhc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cheryme.top/gtevsrpvbe.html

Go:   slices.Sort(arr)
来源：http://hz.fengsongda.top/gtzivvaqxk.html

Ruby: arr.sort
来源：http://hz.feifeiyinyue.top/gtpuseyxhm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxinkj.top/gtocnboyng.html

[N03] 快速排序（分治示例）
来源：http://hz.sufxvd.cn/gtficllpyl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.dashuyun.cn/gtrqgdhjhs.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xziqi.cn/gtgmqfthfb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtrbagkvwx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jianghu66.top/gtgypzdbet.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.svipenyu.cn/gtyyyarltf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cucudq.cn/gtmvagoccn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yvedp.cn/gtkawuuzxu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtrkpiozig.html

[N04] 斐波那契数列
来源：http://hz.xziqi.cn/gtfahcsnrj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtajdjsbrg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtgdremely.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gtaxdgdjcr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtyzbzaxzk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ppjwa.cn/gtxtilvrow.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinyuanbaomall.cn/gtywmjfirq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gtgpbnains.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yongpay.top/gtkprwieyw.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtirlydqam.html

Py:   math.gcd(a, b)
来源：http://hz.jiagoushi.top/gtfjsxzxwe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xinyue.icu/gtfbklvnid.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhiwuduotai.top/gtayhdwasg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gteleufwiv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sxryk.cn/gtwupnurga.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenlongwang.top/gtapncovzh.html

Ruby: a.gcd(b)
来源：http://hz.xuanzx.com/gtakizeamf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zdqjudy.top/gtkidcnghu.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtolexgmxz.html

Py:   s == s[::-1]
来源：http://hz.jinqigfzy.top/gtdinpqirm.html

PHP:  $s === strrev($s);
来源：http://hz.jqgufenzy.top/gtarwdahja.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtetelksgl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtypztltff.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yangfankeji.com/gtxlihqbrs.html

Go:   // 双指针从两端比较
来源：http://hz.cqqwz.cn/gtcvomtwno.html

Ruby: s == s.reverse
来源：http://hz.tianlin.xyz/gtrgjqfkos.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gtntshesob.html

[N07] 两数之和（返回下标）
来源：http://hz.aizwys.cn/gtlhsvkydg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.birdmap.top/gtbirhvbnv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenjidiqi.icu/gtoxrzcnoo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhixingplan.top/gtntzneqhc.html

TS:   // 手写 Map<string, number>
来源：http://hz.haohaochexian.top/gtsdodwvrk.html

Java: // 手写 HashMap
来源：http://hz.9152youxi.cn/gtwlhhwqvp.html

Go:   // 手写 map[int]int
来源：http://hz.havefunace.top/gthvvapmne.html

Ruby: // 手写 Hash
来源：http://hz.chenlongwang.top/gtkktjqyoh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ivvv.top/gtnxdlryhi.html

[N08] 生成全排列
来源：http://hz.cdnleiting.top/gtzodjxoqb.html

Py:   itertools.permutations(arr)
来源：http://hz.cqqwz.cn/gtygoycpoj.html

PHP:  // 手写递归交换
来源：http://hz.tanke756.top/gtjwxbltyx.html

JS:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtqgvwmudf.html

TS:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtuzocvwld.html

Java: // 手写回溯递归
来源：http://hz.daxiang520.top/gtewnrohyk.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtubzeaipf.html

Ruby: arr.permutation.to_a
来源：http://hz.cucudq.cn/gteawkhhrg.html

C#:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtkifjwjgk.html

[N09] 栈与队列
来源：http://hz.vqdsnc.cn/gtgpfscnut.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daxiang520.top/gtfcedtolb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.quarkkingdee.top/gtxofmjzsv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shangyingyoupin.top/gtnusojici.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jiagoushi.top/gtztivokmn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.svipenyu.cn/gtvtndbmej.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.meibo888.top/gteijahrbg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.haohaochexian.top/gtpvubcrab.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yonumen.top/gtexjrrdzx.html

[N10] 链表节点定义
来源：http://hz.dianchejie.cn/gtzyoyksxs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhiwuduotai.top/gtwiilvlan.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nwbrower.top/gtsznksgmy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.redwolf501.top/gtlgwtxlzk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gotoacloud.top/gtvcgkiakf.html

Java: class Node { int v; Node next; }
来源：http://hz.daxiang520.top/gtadvbkyav.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenlongwang.top/gtvcmyvmkg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.snrcjt.cn/gtuvxkxvyu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dashuyun.cn/gtibufluik.html

[N11] 二叉树中序遍历
来源：http://hz.yvedp.cn/gtlrcrjzkn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gogol.net.cn/gtbjmruvud.html

PHP:  // 手写递归函数
来源：http://hz.smart0.xyz/gtlaxjymrc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cdnleiting.top/gtueacbjjj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtgscgyvqh.html

Java: // 手写递归
来源：http://hz.nanxinkj.top/gtzytqoyjl.html

Go:   // 手写递归
来源：http://hz.cdnleiting.top/gtuomrfviw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tanke756.top/gtcddosswy.html

C#:   // 手写递归
来源：http://hz.ehwqpu.com/gttgqpulmj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xinyue.icu/gtgfkhfspg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cqqwz.cn/gtabpnfovt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jqgfzy.top/gtvlymxdyb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hysaishi.cn/gtbfidarob.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sxryk.cn/gtchtveoyh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtsplkpmsl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pycfn.com/gteqwpistz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dianchejie.cn/gteuomitxk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yonumen.top/gtauxunjos.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtkcyqgpsz.html

O. 并发与异步
来源：http://hz.guannengcc.top/gtnhbnnvix.html

================================================================================
来源：http://hz.andypj.xyz/gtffvxqubj.html

[O01] 启动一个线程
来源：http://hz.zdqjudy.top/gtorwwwkdt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuanzx.com/gtpedobffu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yonumen.top/gthmlixlkh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pengpengdd.cyou/gtqwilsrqf.html

TS:   // 同 JS
来源：http://hz.birdmap.top/gtngterlmn.html

Java: new Thread(() -> f()).start()
来源：http://hz.dashuyun.cn/gtbutlzykd.html

Go:   go f()
来源：http://hz.wangshuangyany.cn/gtuiiiyfyj.html

Ruby: Thread.new { f }
来源：http://hz.zdqjudy.top/gtyevrhyds.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258888.top/gtpqlptovr.html

[O02] 使用线程池
来源：http://hz.xinyue.icu/gtumdllpie.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.pycfn.com/gtagmdreyw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenzaomai.com/gthmxsvkfm.html

JS:   // worker_threads 线程池
来源：http://hz.chenjidiqi.icu/gtpmnbaryz.html

TS:   // worker_threads 线程池
来源：http://hz.andypj.xyz/gtbbtojqkb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ivvv.top/gtvgtcolno.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gzhubu.top/gtjfkiozsp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zdqjudy.top/gtndtpzagl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shzxlz.cn/gtuwulsyem.html

[O03] 加锁保护共享数据
来源：http://hz.xinyue.icu/gtpaipfwdx.html

Py:   with lock: shared += 1
来源：http://hz.ydjk.org.cn/gtdegjaldk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hfpthk.cn/gtlgsjtknd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jyoumei.cn/gtxlvsqbkt.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtcicexhar.html

Java: synchronized (this) { shared++; }
来源：http://hz.hysaishi.cn/gtgyeltbza.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ppjwa.cn/gtnjuishwv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenzaomai.com/gtqwhlnxxu.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnxiangtu.top/gtpwntlzkv.html

[O04] 定义异步函数并等待
来源：http://hz.nanxuanxn.top/gtdfzmwflh.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgufenzy.top/gtpwojeawc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yueranfly.top/gthsrnreex.html

JS:   async function f() { await g(); }
来源：http://hz.shangyingyoupin.top/gtfrcwgxbf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jyoumei.cn/gthncfjdgu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.feifeiyinyue.top/gtlaasdmzf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yanxiufei.cn/gtbnikwsev.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhongyouzk.top/gtfkdpbvro.html

C#:   async Task F() { await G(); }
来源：http://hz.yvedp.cn/gtszmkncbs.html

[O05] 并发执行并等待全部完成
来源：http://hz.sufxvd.cn/gtkqtktffv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ehwqpu.com/gtnvyevlyc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydzc1.top/gtjekpupin.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtogpcivdg.html

TS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtookpqgiu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jyoumei.cn/gtbjbflfqo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.0kj1m.cn/gttxznpdps.html

Ruby: threads.map(&:join)
来源：http://hz.cqqwz.cn/gtzgyepsle.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj20258888.top/gtoefntdwe.html

[O06] 使用进程池
来源：http://hz.zhengqikj.top/gtprxykqit.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cheryme.top/gtkuvsgefc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ybcxt.top/gtsbbtrjtm.html

JS:   // child_process / cluster 模块
来源：http://hz.jlsjyb.cn/gtpgalphhi.html

TS:   // child_process / cluster 模块
来源：http://hz.zhaomingkeji.xyz/gtsiuwndps.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shanyushiyangkeji.top/gtjzxpvarh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinqigufen.top/gtoutpidtn.html

Ruby: // fork 块
来源：http://hz.dashuyun.cn/gtrhlfqswo.html

C#:   Parallel.For
来源：http://hz.sufxvd.cn/gteokpungr.html

================================================================================
来源：http://hz.vqdsnc.cn/gtyjbexotd.html

P. 常用工具函数
来源：http://hz.ybcxt.top/gttilkeheb.html

================================================================================
来源：http://hz.ydjk.org.cn/gtepeifsqw.html

[P01] 生成 UUID
来源：http://hz.shzxlz.cn/gtxlayhjqb.html

Py:   str(uuid.uuid4())
来源：http://hz.shanyushiyangkeji.top/gtsgqiychx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fzhhl.top/gtiyevalbd.html

JS:   crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtmxfesmhi.html

TS:   crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtdzcgikfz.html

Java: UUID.randomUUID().toString()
来源：http://hz.fzhhl.top/gttgrfqdyz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.quarkkingdee.top/gtxhicvglm.html

Ruby: SecureRandom.uuid
来源：http://hz.ydzc1.top/gtmitymuaf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cucudq.cn/gtcpujhoik.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhaomingkeji.xyz/gtkpwicutj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.vqdsnc.cn/gtqgacndll.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhixingplan.top/gtafftgzap.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daxiang520.top/gtygwlnuai.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sysykeji.top/gtfjwknjxs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hysaishi.cn/gtuiqfrjlb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yuxming.cn/gtxyztvqqk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigfzy.top/gtyysnwshl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hongshengwenyu.top/gtbjcxzqof.html

[P03] 生成短随机字符串
来源：http://hz.cdnleiting.top/gthqldmuzh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cucudq.cn/gtvqmynjjh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.snrcjt.cn/gtjrseoraf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shzxlz.cn/gtabpzajty.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhiwuduotai.top/gtmpxcuotq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.birdmap.top/gtsentmhiv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xingfuxueyuan.xyz/gtqakswjlh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.andypj.xyz/gtceztsgfj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangtech.top/gtrbkpsztp.html

[P04] 求长度
来源：http://hz.meibo888.top/gtxvicfrdt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tianlin.xyz/gtpudwzwzi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ppjwa.cn/gtqvuuquwx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtvogxdzqf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gtecccofmt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.wangdashe.top/gtlnikpidt.html

Go:   len(arr);  len(m)
来源：http://hz.316326.xyz/gtmrzuycft.html

Ruby: x.length;  x.size
来源：http://hz.9152youxi.cn/gtgqnujmlb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj202588.top/gtbwmaioww.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj20258.top/gtiaradtnb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gaohongyu789.top/gtjbubhusg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tanke756.top/gtqqekjfts.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sxryk.cn/gtoamgyhnr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangkeji.top/gtjidaujhc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hysaishi.cn/gtfoauasge.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.birdmap.top/gtahzccnxg.html

Ruby: a == b
来源：http://hz.hnqzz.top/gtzlepoudp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hfpthk.cn/gtjnohhasq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.vqdsnc.cn/gtzrbbpwvt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jianghu66.top/gtchzaxfzc.html

PHP:  if (empty($x)) {}
来源：http://hz.svipenyu.cn/gtlwxoqryo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hnqzz.top/gtyqnsmumc.html

TS:   if (x == null) {}
来源：http://hz.fengsongda.top/gtzwcdeynj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gzhubu.top/gttskkshgz.html

Go:   if x == nil {}
来源：http://hz.yanxiufei.cn/gtoqukcrro.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.quarkkingdee.top/gtjfjjxvhn.html

C#:   if (x is null) {}
来源：http://hz.wangshuangyany.cn/gtrgeduuid.html

[P07] 防抖与节流
来源：http://hz.shzxlz.cn/gtlrpfaaty.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yongpay.top/gtpjczneoc.html

PHP:  // 手写时间戳比较
来源：http://hz.dashuyun.cn/gtldrovlnd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtizxatvme.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtwumacead.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhiwuduotai.top/gtrmphqluw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.snrcjt.cn/gtoymluuxy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenjidiqi.icu/gtmxelwkkq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shangyingyoupin.top/gtfhtqrfuq.html

[P08] 处理浮点精度问题
来源：http://hz.0kj1m.cn/gtiwnjjajz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cashguo.top/gtrvbtdgva.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ybcxt.top/gtwjqxovjs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nwbrower.top/gtdkqghohy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jqgufenzy.top/gtfqejhmur.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sweek.top/gtykwqsqyz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zycfv.cn/gtdgagikcy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.snrcjt.cn/gtygqirolc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuanzhike.top/gtywhavgcc.html

================================================================================
来源：http://hz.nanxinkj.top/gtthrtjphs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tianlin.xyz/gttcbpunvx.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtxpscesje.html

[Q01] 创建表
来源：http://hz.yonumen.top/gtzpcrrvzm.html

CREATE TABLE users (
来源：http://hz.xinyue.icu/gtkdencwmn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtjlhtpali.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sufxvd.cn/gthwdtlcnu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shuidangran.top/gtaljyccif.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.9152youxi.cn/gtwaabeifj.html

);
来源：http://hz.chenzaomai.com/gtwvosynzt.html

[Q02] 创建带外键的表
来源：http://hz.pengpengdd.cyou/gtpctwkyjc.html

CREATE TABLE orders (
来源：http://hz.xinyue.icu/gtvjxcorez.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtfiplvpag.html

user_id INT NOT NULL,
来源：http://hz.chenjidiqi.icu/gtpvkyhdev.html

amount DECIMAL(10, 2),
来源：http://hz.gotoacloud.top/gtrizrdaou.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yj20258.top/gtqwcynucu.html

);
来源：http://hz.sufxvd.cn/gtppkrgdrk.html

[Q03] 增加列
来源：http://hz.pycfn.com/gtkgmnyfmb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dianchejie.cn/gtnxwprtlp.html

[Q04] 修改列类型
来源：http://hz.andypj.xyz/gtuplgytuz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hnxiangtu.top/gtrbawcliv.html

[Q05] 重命名列
来源：http://hz.wangdashe.top/gtsvbxawwx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.vqdsnc.cn/gtaecgyjvj.html

[Q06] 删除列
来源：http://hz.daxiang520.top/gtsgyvwesk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shangyingyoupin.top/gtvqndezop.html

[Q07] 删除表
来源：http://hz.redwolf501.top/gtodfkxdur.html

DROP TABLE IF EXISTS orders;
来源：http://hz.guannengcc.top/gtamtcgsbx.html

[Q08] 创建普通索引
来源：http://hz.redwolf501.top/gtptumqhzh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.andypj.xyz/gtzxgihsnc.html

[Q09] 创建唯一索引
来源：http://hz.ydjk.org.cn/gtaiooqjky.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.birdmap.top/gtavgrbukm.html

[Q10] 插入单行
来源：http://hz.cdnleiting.top/gtuppstuvr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtavexpxrm.html

[Q11] 一次插入多行
来源：http://hz.shuidangran.top/gtwsfaeffu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.redwolf501.top/gtzdsiqwjn.html

[Q12] 插入后取自增 ID
来源：http://hz.shuidangran.top/gtfoppjtpp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sufxvd.cn/gtvwmsvaix.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cashguo.top/gtabkchaos.html

[Q13] 忽略重复插入
来源：http://hz.yuxming.cn/gtuslqpnnj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.316326.xyz/gtfstxbhmh.html

[Q14] 存在则更新（upsert）
来源：http://hz.zdqjudy.top/gteiksuaqc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangshuangyany.cn/gtwlfrhkek.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cashguo.top/gtuomlisko.html

[Q15] 查询全部
来源：http://hz.xylfe.cn/gtukjqyuwl.html

SELECT * FROM users;
来源：http://hz.quarkkingdee.top/gtxtyczmzx.html

[Q16] 查询指定列
来源：http://hz.cqqwz.cn/gtpbsinnhv.html

SELECT id, name FROM users;
来源：http://hz.hnxiangtu.top/gtxqznwtan.html

[Q17] 条件查询
来源：http://hz.chenzaomai.com/gtzejcaqia.html


<!-- 参考信息 -->