代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ppjwa.cn/gtzkjllwfk.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthjsboycz.html

N. 数据结构与算法
来源：http://hz.wangshuangyany.cn/gtevzignjv.html

================================================================================
来源：http://hz.tianlin.xyz/gtpcqafgmf.html

[N01] 二分查找（有序数组）
来源：http://hz.zhijiandao.cn/gtbtwdxqdn.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.aibaodan.cn/gtseipybhg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.havefunace.top/gtihgwfiiv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtpfqtzmkn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtebehmfjs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xuanzx.com/gtthnawluc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtsbevzhko.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuxming.cn/gtletdpjlz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.mhx1999.top/gtvpopxvdl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yonumen.top/gtmldbvfoe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxuanxn.top/gthbpcyvtt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xingfuxueyuan.xyz/gtmcrnhpkb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtdocmxsvq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtrwbozjzy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.daria6918.cn/gtvsyxpcrf.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gtxiyegbdn.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtmucwhkqm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhengqikj.top/gtarktfyuj.html

[N03] 快速排序（分治示例）
来源：http://hz.xuanzx.com/gtwibxujnd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangkeji.top/gtplgxfppf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.quarkkingdee.top/gtkjrvxzeo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtmffcjhgy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtchyvahiz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.mhx1999.top/gteszukhqe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pycfn.com/gtlslediwp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.wangdashe.top/gtjunikkpt.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ehwqpu.com/gtdzvhcbbd.html

[N04] 斐波那契数列
来源：http://hz.aizwys.cn/gtmyurrrdr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhoulong.xyz/gtnvortzfw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guowangkeji.top/gtlcqzfgxy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtypymjhme.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aizwys.cn/gtniibffhg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.pengpengdd.cyou/gtoizlznzj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tanke756.top/gtkucwzmxy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.dianchejie.cn/gtmapkrsvx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.mhx1999.top/gtlbjhyvhh.html

[N05] 最大公约数
来源：http://hz.cqqwz.cn/gtnvjbhwuh.html

Py:   math.gcd(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtpoxqltwc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.316326.xyz/gtikqdbmqi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtbsoftygd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xingfuxueyuan.xyz/gtjbbefoaf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hammf.cn/gtgjlupvvi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cucudq.cn/gtalxkkvju.html

Ruby: a.gcd(b)
来源：http://hz.daria6918.cn/gtosqdddao.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zycfv.cn/gtpxaqxxsm.html

[N06] 判断回文字符串
来源：http://hz.daria6918.cn/gtvlnnajii.html

Py:   s == s[::-1]
来源：http://hz.shangyingyoupin.top/gtivnvzuzf.html

PHP:  $s === strrev($s);
来源：http://hz.zdqjudy.top/gtgcvzcypk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtbmmuimyu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtkyghavlc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yueranfly.top/gtefxqiarq.html

Go:   // 双指针从两端比较
来源：http://hz.xuetiantiany.cn/gtxomrqmdo.html

Ruby: s == s.reverse
来源：http://hz.zycfv.cn/gthzjlwhra.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.quarkkingdee.top/gtrudsiznm.html

[N07] 两数之和（返回下标）
来源：http://hz.redwolf501.top/gtboppwven.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenlongwang.top/gtsapeskvi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenlongwang.top/gtygqyvwas.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jiagoushi.top/gtseyyqbxa.html

TS:   // 手写 Map<string, number>
来源：http://hz.hysaishi.cn/gtjybaiapj.html

Java: // 手写 HashMap
来源：http://hz.haohaochexian.top/gtdovfrgem.html

Go:   // 手写 map[int]int
来源：http://hz.zhoulong.xyz/gtipcejreh.html

Ruby: // 手写 Hash
来源：http://hz.zhongyouzk.top/gtyecqlvlh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guowangkeji.top/gtxrzcboct.html

[N08] 生成全排列
来源：http://hz.daria6918.cn/gtldzmbwvl.html

Py:   itertools.permutations(arr)
来源：http://hz.feifeiyinyue.top/gtobsetmad.html

PHP:  // 手写递归交换
来源：http://hz.jinqigfzy.top/gtpwuzmvza.html

JS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtqzyeprxu.html

TS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtbwslcpol.html

Java: // 手写回溯递归
来源：http://hz.hnqzz.top/gtcmkehyvl.html

Go:   // 手写回溯递归
来源：http://hz.birdmap.top/gthamzumzv.html

Ruby: arr.permutation.to_a
来源：http://hz.jqgufenzy.top/gtfqioosxz.html

C#:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtrjihaaed.html

[N09] 栈与队列
来源：http://hz.jianghu66.top/gtnovcgmcz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinghuilouyu.cn/gtyvecmwdq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.svipenyu.cn/gtejfmwjzi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yonumen.top/gttpbqpwtn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenlongwang.top/gtrujbwywl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ppjwa.cn/gtjvshxzce.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sxryk.cn/gtapmqhahn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sufxvd.cn/gtggmnguor.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zycfv.cn/gtdnnuovph.html

[N10] 链表节点定义
来源：http://hz.cashguo.top/gtdxxzoqjg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.pengpengdd.cyou/gtypcrbkuc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.feifeiyinyue.top/gtilfuwfqn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sxryk.cn/gtctitbnux.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sweek.top/gtlwykhfhs.html

Java: class Node { int v; Node next; }
来源：http://hz.gaohongyu789.top/gtutsxqtez.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.9152youxi.cn/gtwqsimmsu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xziqi.cn/gtyiptmhih.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shanyushiyangkeji.top/gtkbmnalnd.html

[N11] 二叉树中序遍历
来源：http://hz.dashuyun.cn/gthefjhtki.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jqgufenzy.top/gthleblros.html

PHP:  // 手写递归函数
来源：http://hz.daria6918.cn/gtveijokvr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gtdndttmoj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gtbdljbcvi.html

Java: // 手写递归
来源：http://hz.gzhubu.top/gtoqnkciad.html

Go:   // 手写递归
来源：http://hz.mhx1999.top/gtdxnyclpu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cucudq.cn/gtmnszpjmx.html

C#:   // 手写递归
来源：http://hz.havefunace.top/gtcnndxyum.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tian-w.cn/gtqtkxowvh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sysykeji.top/gtqulkvkri.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yonumen.top/gtfkfjlllg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhijiandao.cn/gtzcewfqnz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtkppulroz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtrkfhkbeg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinghuilouyu.cn/gtyiqzqrcc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hnqzz.top/gthbayygxy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtngibillz.html

================================================================================
来源：http://hz.jianghu66.top/gtaeafbach.html

O. 并发与异步
来源：http://hz.c1oappe.top/gtgjkfgdjz.html

================================================================================
来源：http://hz.smart0.xyz/gtpzgzkofz.html

[O01] 启动一个线程
来源：http://hz.andypj.xyz/gtmugrsblv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigufen.top/gtksofegxm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinyuanbaomall.cn/gtawpzpuod.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nanxinkj.top/gttqjsdzbz.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtlzjwefuz.html

Java: new Thread(() -> f()).start()
来源：http://hz.c1oappe.top/gtmnbluttq.html

Go:   go f()
来源：http://hz.pengpengdd.cyou/gtyciebxxv.html

Ruby: Thread.new { f }
来源：http://hz.gaohongyu789.top/gtefnxczsg.html

C#:   Task.Run(() => F());
来源：http://hz.yuxming.cn/gtzixlaxlp.html

[O02] 使用线程池
来源：http://hz.dashuyun.cn/gtfaiyokoq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jianghu66.top/gtufjhpmfn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtedxevyvg.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gtrgtrbdxj.html

TS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtrzyokucv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangkeji.top/gtzwwcskma.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sweek.top/gtemshafiv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuxming.cn/gthoujaeag.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigufen.top/gtbhgxmzmd.html

[O03] 加锁保护共享数据
来源：http://hz.aizwys.cn/gtwxuiscjy.html

Py:   with lock: shared += 1
来源：http://hz.snrcjt.cn/gtvkvscmqx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.pycfn.com/gtjxuwrkak.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.vqdsnc.cn/gtaniqjljw.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtpoddtviw.html

Java: synchronized (this) { shared++; }
来源：http://hz.zycfv.cn/gtdkhgfkub.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zdqjudy.top/gtklngwtit.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nanxuanxn.top/gtucfydhas.html

C#:   lock (gate) { shared++; }
来源：http://hz.jlsjyb.cn/gtezphtcll.html

[O04] 定义异步函数并等待
来源：http://hz.jinyuanbaomall.cn/gtlekmofmq.html

Py:   async def f():⏎    await g()
来源：http://hz.aizwys.cn/gtfoxpombo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shzxlz.cn/gtcjiadjwf.html

JS:   async function f() { await g(); }
来源：http://hz.birdmap.top/gtujugopbp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dashuyun.cn/gtrcherrbr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jiagoushi.top/gtuebibtym.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nanxuanxn.top/gtrikhdseh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xylfe.cn/gtuorqabde.html

C#:   async Task F() { await G(); }
来源：http://hz.pycfn.com/gtlhowrycn.html

[O05] 并发执行并等待全部完成
来源：http://hz.daria6918.cn/gtbjgburjd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yongpay.top/gtvwxijsxy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zycfv.cn/gtpiidxamn.html

JS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gtomwkgebv.html

TS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtzpduzptr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jianghu66.top/gttrqcprvq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dianchejie.cn/gtwcnowaqv.html

Ruby: threads.map(&:join)
来源：http://hz.sufxvd.cn/gtqsqmldnw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.pycfn.com/gtvjogbgww.html

[O06] 使用进程池
来源：http://hz.tianlin.xyz/gtiqwqowam.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangdashe.top/gtqrtpydnp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuetiantiany.cn/gttoogmgxx.html

JS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtbelpemms.html

TS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gthxjmhwze.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.wangdashe.top/gticklenzo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenjidiqi.icu/gteloqepve.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtdvenqfyx.html

C#:   Parallel.For
来源：http://hz.yuanzhike.top/gtekaejqtn.html

================================================================================
来源：http://hz.xylfe.cn/gtpkycnmlu.html

P. 常用工具函数
来源：http://hz.zhoulong.xyz/gtymcqtbdh.html

================================================================================
来源：http://hz.mhx1999.top/gtfpguyzsa.html

[P01] 生成 UUID
来源：http://hz.ywan-chungtsiang.top/gtnrfthdax.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgufenzy.top/gthfpzuilu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daxiang520.top/gtyatvomqq.html

JS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtwhttwcrq.html

TS:   crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gttbqbpjmu.html

Java: UUID.randomUUID().toString()
来源：http://hz.andypj.xyz/gtynhuufhi.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gaohongyu789.top/gtnjmdmxpk.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gthqpfwiqo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenjidiqi.icu/gtjuydhqou.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nanxinkj.top/gtraftwrga.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hfpthk.cn/gtlpsbtdhc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.haohaochexian.top/gtwbrzkwcb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jqgfzy.top/gtxcxityhu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aizwys.cn/gttfzevwja.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yongpay.top/gtvrcoumux.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhaomingkeji.xyz/gthosdilxd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cashguo.top/gtadqgtryv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenlongwang.top/gtrkcxombw.html

[P03] 生成短随机字符串
来源：http://hz.hnqzz.top/gtndbpdcok.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenlongwang.top/gtjfdesnoq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dashuyun.cn/gtsbhzbhbm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258888.top/gtmqqwsadq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtwcjdirfr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.svipenyu.cn/gtibsopust.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cqqwz.cn/gtprthpfxy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hysaishi.cn/gtlpwawkrf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhiwuduotai.top/gtucrkrxje.html

[P04] 求长度
来源：http://hz.jinghuilouyu.cn/gtpknzeqba.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daria6918.cn/gtlpnffkkn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daria6918.cn/gtpwjcstgd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtuzdddxsu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gtfzowenvx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jiagoushi.top/gtvwzglfcm.html

Go:   len(arr);  len(m)
来源：http://hz.yvedp.cn/gturlbddri.html

Ruby: x.length;  x.size
来源：http://hz.ywan-chungtsiang.top/gtmauxwgke.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.smart0.xyz/gtqoixnqrn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xinyue.icu/gtolzqoghu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.guowangkeji.top/gthwahxpat.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangtech.top/gtzgbraapl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnqzz.top/gtpoccrdur.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jianghu66.top/gtxrxlwjjk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.bjfxy.top/gteuogxgqc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tianlin.xyz/gtcdlmuzcb.html

Ruby: a == b
来源：http://hz.jqgfzy.top/gtpgsbjukb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sysykeji.top/gtjscwttxl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jlsjyb.cn/gttgiwgjhh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhongyouzk.top/gtsbrddgyq.html

PHP:  if (empty($x)) {}
来源：http://hz.cucudq.cn/gtcneossnq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nwbrower.top/gtkcguhlhl.html

TS:   if (x == null) {}
来源：http://hz.ppjwa.cn/gthuepkkhm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtqnloezvx.html

Go:   if x == nil {}
来源：http://hz.fzhhl.top/gtfgobcqma.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.haohaochexian.top/gthtqwfbia.html

C#:   if (x is null) {}
来源：http://hz.nanxuanxn.top/gtpngfkeey.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtrxjsuvzn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hnqzz.top/gtbnmtpxmi.html

PHP:  // 手写时间戳比较
来源：http://hz.yuxming.cn/gtqputerbg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtsurjxmlv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtyamxozze.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.bjfxy.top/gtkonkfztt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenjidiqi.icu/gtggbcphnf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nanxuanxn.top/gtseknwqbx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinghuilouyu.cn/gtenitgvdt.html

[P08] 处理浮点精度问题
来源：http://hz.dashuyun.cn/gtxobvojya.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jyoumei.cn/gthanthtbk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nanxinkj.top/gtmryjiwny.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pengpengdd.cyou/gtiugdpswq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.guowangkeji.top/gtohlnvobs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinyuanbaomall.cn/gtafutdzca.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258.top/gtgldrwcwj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jlsjyb.cn/gtbivvizqp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jyoumei.cn/gtnmqsxrnt.html

================================================================================
来源：http://hz.sysykeji.top/gtsrwhxphc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.9152youxi.cn/gtfflzpcqd.html

================================================================================
来源：http://hz.yuxming.cn/gtyhbyxusg.html

[Q01] 创建表
来源：http://hz.cdnleiting.top/gtamzeznhr.html

CREATE TABLE users (
来源：http://hz.yuxming.cn/gtrvhzoplr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hysaishi.cn/gtgzxiouaq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.guannengcc.top/gtabpayixx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gtzogzhemj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ywan-chungtsiang.top/gtrogysrbf.html

);
来源：http://hz.ivvv.top/gtpbvtxawy.html

[Q02] 创建带外键的表
来源：http://hz.chenzaomai.com/gtgyvdokpi.html

CREATE TABLE orders (
来源：http://hz.shanyushiyangtech.top/gttrwlqapx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhoulong.xyz/gtyiifnjyu.html

user_id INT NOT NULL,
来源：http://hz.havefunace.top/gtaxufygtr.html

amount DECIMAL(10, 2),
来源：http://hz.yuanzhike.top/gtcdcnamwz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cashguo.top/gtbwfzjhue.html

);
来源：http://hz.quarkkingdee.top/gtqkkhcviy.html

[Q03] 增加列
来源：http://hz.fengsongda.top/gtvlzgscdi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cashguo.top/gthobdrlyl.html

[Q04] 修改列类型
来源：http://hz.cheryme.top/gthfefobse.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zdqjudy.top/gtsdcogvhu.html

[Q05] 重命名列
来源：http://hz.cqqwz.cn/gthijstrpv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgfzy.top/gtabyzssss.html

[Q06] 删除列
来源：http://hz.jinqigufen.top/gtkmmcktot.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nanxinkj.top/gtorgdzoii.html

[Q07] 删除表
来源：http://hz.shzxlz.cn/gtejkemduu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.iojbl.cn/gtrmhupklc.html

[Q08] 创建普通索引
来源：http://hz.zhijiandao.cn/gtqyzqeirz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yongpay.top/gtouiuozos.html

[Q09] 创建唯一索引
来源：http://hz.dianchejie.cn/gtzbjleaht.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nwbrower.top/gtmtvkgslo.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtladaidaw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sxryk.cn/gtuihxuwkl.html

[Q11] 一次插入多行
来源：http://hz.tanke756.top/gtwcjmqzjr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fzhhl.top/gtstmfnsze.html

[Q12] 插入后取自增 ID
来源：http://hz.hongshengwenyu.top/gtkeqnhqbr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sufxvd.cn/gtauzqpldr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gaohongyu789.top/gtzuxxwfoa.html

[Q13] 忽略重复插入
来源：http://hz.jqgufenzy.top/gtojpzkqak.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxuanxn.top/gtkusyqugr.html

[Q14] 存在则更新（upsert）
来源：http://hz.kuanghao11.cn/gtchpmwiet.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fengsongda.top/gtcliowzgl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.redwolf501.top/gttjyqfxma.html

[Q15] 查询全部
来源：http://hz.aibaodan.cn/gtojqzeapf.html

SELECT * FROM users;
来源：http://hz.jinghuilouyu.cn/gtnjpouxxm.html

[Q16] 查询指定列
来源：http://hz.dianchejie.cn/gtoetsdpwc.html

SELECT id, name FROM users;
来源：http://hz.cqqwz.cn/gtuodpxvcw.html

[Q17] 条件查询
来源：http://hz.ydzc1.top/gthkheysfv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yanxiufei.cn/gtavwvjqkn.html

[Q18] 模糊匹配
来源：http://hz.zhixingplan.top/gtmcnrsggv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.havefunace.top/gtmoodtilz.html

[Q19] 范围查询
来源：http://hz.feifeiyinyue.top/gtboukvdns.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.kuanghao11.cn/gtokfpuekf.html

[Q20] IN 列表
来源：http://hz.shangyingyoupin.top/gthuwumkrf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xinyue.icu/gtlmrqpabs.html

[Q21] 空值判断
来源：http://hz.yonumen.top/gtfiqwvsiy.html


<!-- 参考信息 -->