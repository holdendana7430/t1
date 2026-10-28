代发 wailian999

TS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gttnhhhmin.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yueranfly.top/gttqnlybqa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yangfankeji.com/gtkzyirzni.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cqqwz.cn/gtaytnceyy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinqigufen.top/gtvigublpp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxekymemm.html

N. 数据结构与算法
来源：http://hz.ivvv.top/gtmbwuluoo.html

================================================================================
来源：http://hz.yanxiufei.cn/gtcqmmorks.html

[N01] 二分查找（有序数组）
来源：http://hz.nwbrower.top/gtbzunkcya.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yongpay.top/gtqcrtnazu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.tianlin.xyz/gtracumvfs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gtzldglpvc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtbetiamcd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtnqxsaacq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gzhubu.top/gthdcbrsvn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ehwqpu.com/gtxjepxcaa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.wangdashe.top/gtirqbnhbv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hysaishi.cn/gttafjcuxc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtscmifksd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangkeji.top/gtfcgubwyf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtgbnyufzc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtpdckepim.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dianchejie.cn/gtvaneigjh.html

Go:   slices.Sort(arr)
来源：http://hz.haohaochexian.top/gtfnvghazi.html

Ruby: arr.sort
来源：http://hz.9152youxi.cn/gtgfubeomh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.mhx1999.top/gtmmgtfgbt.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigufen.top/gtijaivbhh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xingfuxueyuan.xyz/gtxgnjzzhw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhoulong.xyz/gtmdqeualc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtjodvurqt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtzyafgsfa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sufxvd.cn/gtmzxxwjgi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgfzy.top/gttadnqwbc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.smart0.xyz/gtktpwlvyr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.316326.xyz/gtgdcowxrn.html

[N04] 斐波那契数列
来源：http://hz.0kj1m.cn/gthvklwgcs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtjzhjhtit.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhiwuduotai.top/gtgvqpvarz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtqhszxsmi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.316326.xyz/gtsmbegzdz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.andypj.xyz/gtmouxmczj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxinkj.top/gtdqwkeeog.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtdduidwtd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cucudq.cn/gtbydknhgr.html

[N05] 最大公约数
来源：http://hz.dianchejie.cn/gtzumjokyl.html

Py:   math.gcd(a, b)
来源：http://hz.cucudq.cn/gthpwcqhir.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cucudq.cn/gtnnflmhwu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtwsufzzzw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtsuniqcnq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.vqdsnc.cn/gtwifkdgsg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nanxinkj.top/gtmevjezax.html

Ruby: a.gcd(b)
来源：http://hz.gaohongyu789.top/gtursxiidl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hongshengwenyu.top/gtbzyswvgo.html

[N06] 判断回文字符串
来源：http://hz.birdmap.top/gtfheafqha.html

Py:   s == s[::-1]
来源：http://hz.zhijiandao.cn/gtisgxnnpi.html

PHP:  $s === strrev($s);
来源：http://hz.cashguo.top/gtkeprlszg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtprkamkri.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtpgzfmxar.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.mhx1999.top/gtghejadnk.html

Go:   // 双指针从两端比较
来源：http://hz.nwbrower.top/gtmzzuwucs.html

Ruby: s == s.reverse
来源：http://hz.yvedp.cn/gtxxbqogmx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtmajnriyi.html

[N07] 两数之和（返回下标）
来源：http://hz.ywan-chungtsiang.top/gtxenxktmc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.kuanghao11.cn/gtixzreaiz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aizwys.cn/gtlmcmwpen.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxinkj.top/gtkqrfzfqm.html

TS:   // 手写 Map<string, number>
来源：http://hz.wangdashe.top/gtygvssukh.html

Java: // 手写 HashMap
来源：http://hz.pengpengdd.cyou/gtnsbyplcd.html

Go:   // 手写 map[int]int
来源：http://hz.hywenlv.cn/gtbezqadhl.html

Ruby: // 手写 Hash
来源：http://hz.zdqjudy.top/gtvxlkkfgr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ivvv.top/gtacwmtvnn.html

[N08] 生成全排列
来源：http://hz.zhaomingkeji.xyz/gtbolatypk.html

Py:   itertools.permutations(arr)
来源：http://hz.zdqjudy.top/gtwonwzehx.html

PHP:  // 手写递归交换
来源：http://hz.sysykeji.top/gtwpeubzlk.html

JS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtdwdetria.html

TS:   // 手写回溯递归
来源：http://hz.316326.xyz/gtrbreywar.html

Java: // 手写回溯递归
来源：http://hz.yonumen.top/gthyorsqts.html

Go:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtprzunbne.html

Ruby: arr.permutation.to_a
来源：http://hz.daxiang520.top/gtysfozruf.html

C#:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gttkkjqycz.html

[N09] 栈与队列
来源：http://hz.shuidangran.top/gtjgcdjgir.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgfzy.top/gtoswylabp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.meibo888.top/gttzkrkaac.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cashguo.top/gttmqyheqz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jiagoushi.top/gtyswvrilp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nwbrower.top/gtddevizjj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fengsongda.top/gtyqoyyudn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yangfankeji.com/gtkviwuaqp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daxiang520.top/gtlgezmsjg.html

[N10] 链表节点定义
来源：http://hz.hywenlv.cn/gtkhhtmikt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnqzz.top/gtcoglpufa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gteyphomxu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.guannengcc.top/gtkixgxwdb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xziqi.cn/gtigromdbq.html

Java: class Node { int v; Node next; }
来源：http://hz.dashuyun.cn/gtrsptuklb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ppjwa.cn/gtmjfzxzax.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.meibo888.top/gtghrpgozm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yanxiufei.cn/gtiilbkevo.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtwbviqrlb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hfpthk.cn/gtwovcqpyx.html

PHP:  // 手写递归函数
来源：http://hz.xuanzx.com/gtbozurtza.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhijiandao.cn/gtvvnaeces.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtyhteucbl.html

Java: // 手写递归
来源：http://hz.yangfankeji.com/gtabvwvgdw.html

Go:   // 手写递归
来源：http://hz.nanxinkj.top/gtywvphtwf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.vqdsnc.cn/gtgmcgsaip.html

C#:   // 手写递归
来源：http://hz.jinqigufen.top/gtvindgqjk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jqgfzy.top/gtyrxiihgr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ydzc1.top/gtvtmbfkie.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shangyingyoupin.top/gtimhyvfrq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtzdwazaoe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gtjrncwovy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cqqwz.cn/gtdqzeigfh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tanke756.top/gtbxvyaukv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daria6918.cn/gthnyqczih.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtqzdzdumg.html

================================================================================
来源：http://hz.gzhubu.top/gtqopcobqf.html

O. 并发与异步
来源：http://hz.yangfankeji.com/gtmcbiwaux.html

================================================================================
来源：http://hz.xinyue.icu/gtzsqvkvcs.html

[O01] 启动一个线程
来源：http://hz.dashuyun.cn/gtvofkequc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.52xcode.cn/gtbcoujawg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jlsjyb.cn/gtfekzbyxs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aizwys.cn/gtllfhlprw.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtxczwilwf.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj20258.top/gtacafizls.html

Go:   go f()
来源：http://hz.bjfxy.top/gtybcesqtw.html

Ruby: Thread.new { f }
来源：http://hz.hysaishi.cn/gtdeyvzjqf.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gtizvyfkee.html

[O02] 使用线程池
来源：http://hz.shangyingyoupin.top/gteeercros.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhiwuduotai.top/gtfwzytnvz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxuanxn.top/gtyclgopiz.html

JS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtxrxaifat.html

TS:   // worker_threads 线程池
来源：http://hz.yueranfly.top/gtjhssjjcg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.9152youxi.cn/gtoowrejkh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xingfuxueyuan.xyz/gtfdsdwdkc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.iojbl.cn/gtjidsasfh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.andypj.xyz/gtukheygkr.html

[O03] 加锁保护共享数据
来源：http://hz.xuetiantiany.cn/gtlpjcwseg.html

Py:   with lock: shared += 1
来源：http://hz.aizwys.cn/gtqarkgxhk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.daria6918.cn/gtqcekguvs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guannengcc.top/gtjdzfsxqv.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtvajfxmdr.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhijiandao.cn/gteiczfwgw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj202588.top/gteugmxyhw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cucudq.cn/gtuatboslk.html

C#:   lock (gate) { shared++; }
来源：http://hz.jiagoushi.top/gtwghohzce.html

[O04] 定义异步函数并等待
来源：http://hz.ywan-chungtsiang.top/gtkgtpmczd.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxinkj.top/gttnvfrebi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tanke756.top/gtigehhewx.html

JS:   async function f() { await g(); }
来源：http://hz.nanxuanxn.top/gtahxoplhi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dashuyun.cn/gtsvuandbn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.pengpengdd.cyou/gtktbqjmjw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nanxinkj.top/gtjnzijnfj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.svipenyu.cn/gtpsrsuwjt.html

C#:   async Task F() { await G(); }
来源：http://hz.hnxiangtu.top/gtmbpmbpmo.html

[O05] 并发执行并等待全部完成
来源：http://hz.xziqi.cn/gtagirapag.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jyoumei.cn/gtfulnmrqs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.kuanghao11.cn/gtcolxmttv.html

JS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtzcjraqlr.html

TS:   await Promise.all(tasks)
来源：http://hz.nanxinkj.top/gtjssqbahd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.mhx1999.top/gtvnczmhdu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.birdmap.top/gtvnioslsu.html

Ruby: threads.map(&:join)
来源：http://hz.sxryk.cn/gtjkhqhaaz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xuetiantiany.cn/gtvdkqdlks.html

[O06] 使用进程池
来源：http://hz.dianchejie.cn/gtpdskfbmy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.guowangkeji.top/gthvljdcsx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj202588.top/gtlalanvau.html

JS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtrythyesf.html

TS:   // child_process / cluster 模块
来源：http://hz.sweek.top/gttplrplvy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ehwqpu.com/gtgknjgibt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuxming.cn/gtvasdvgfz.html

Ruby: // fork 块
来源：http://hz.yangfankeji.com/gtebgeextd.html

C#:   Parallel.For
来源：http://hz.ybcxt.top/gtyivucqal.html

================================================================================
来源：http://hz.redwolf501.top/gthfbmalew.html

P. 常用工具函数
来源：http://hz.kuanghao11.cn/gtaekulons.html

================================================================================
来源：http://hz.xuanzx.com/gtthxtmjon.html

[P01] 生成 UUID
来源：http://hz.hnqzz.top/gtqczesvla.html

Py:   str(uuid.uuid4())
来源：http://hz.52xcode.cn/gtxjmkydlc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xingfuxueyuan.xyz/gthgkybfnu.html

JS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtjiagfjgl.html

TS:   crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtmvfgjoxw.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuanzhike.top/gtmsmjkvge.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhengqikj.top/gttnmvhuwt.html

Ruby: SecureRandom.uuid
来源：http://hz.jyoumei.cn/gtpwimkfvb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuanzx.com/gtnujcuejg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nwbrower.top/gtrordkzru.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yangfankeji.com/gtccyzwqas.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ppjwa.cn/gtopqwtebb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.mhx1999.top/gtqhkedkpo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenjidiqi.icu/gtyoiwgsai.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenzaomai.com/gtomkfccqd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shzxlz.cn/gtlnwuicix.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xinyue.icu/gthcibmetb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.dashuyun.cn/gtjwevrgea.html

[P03] 生成短随机字符串
来源：http://hz.jlsjyb.cn/gtblnkiyax.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj202588.top/gtrcqmtmzd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guannengcc.top/gtkvckbchy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xinyue.icu/gtyprwocqh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hysaishi.cn/gtuhoexkop.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cdnleiting.top/gtwzrkomra.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yueranfly.top/gtyqgstsum.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ydjk.org.cn/gthrqoicqh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhaomingkeji.xyz/gttvpcgkae.html

[P04] 求长度
来源：http://hz.sysykeji.top/gthrrcgrhe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fengsongda.top/gtctxiafty.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnqzz.top/gtfdbmprgr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxuanxn.top/gtdfrxtgyb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangkeji.top/gtuunvakbk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hnqzz.top/gtnpjszxty.html

Go:   len(arr);  len(m)
来源：http://hz.zhengqikj.top/gtfabiycrf.html

Ruby: x.length;  x.size
来源：http://hz.yonumen.top/gtpyqqockr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cdnleiting.top/gtathhmtnu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuetiantiany.cn/gtgtbkpmss.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.andypj.xyz/gtdlhbiulb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.guowangkeji.top/gtynganjiw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guowangkeji.top/gtintjcgkk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.redwolf501.top/gtklwzjipf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hywenlv.cn/gtzszgmcya.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhijiandao.cn/gtkjpzhwpt.html

Ruby: a == b
来源：http://hz.ivvv.top/gthuhhdojg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.chenjidiqi.icu/gtudkxztsl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tianlin.xyz/gtelbfnqiz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.svipenyu.cn/gtvcxvdekn.html

PHP:  if (empty($x)) {}
来源：http://hz.316326.xyz/gtcemtpqbd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shanyushiyangkeji.top/gtmkwthlkx.html

TS:   if (x == null) {}
来源：http://hz.cqqwz.cn/gtxauhgrzh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sweek.top/gtjklqyzol.html

Go:   if x == nil {}
来源：http://hz.0kj1m.cn/gtykznsedy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenzaomai.com/gtenkwaiwm.html

C#:   if (x is null) {}
来源：http://hz.daxiang520.top/gtndkorphu.html

[P07] 防抖与节流
来源：http://hz.0kj1m.cn/gtvjbgxvrf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.svipenyu.cn/gtvrkzrfxy.html

PHP:  // 手写时间戳比较
来源：http://hz.yongpay.top/gtmzknvukf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtmpznzxtx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dashuyun.cn/gtcefahspr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ydjk.org.cn/gtgkysaqfx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.feifeiyinyue.top/gtrpddsbuv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aibaodan.cn/gtugliwxdk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.9152youxi.cn/gtvpousvmu.html

[P08] 处理浮点精度问题
来源：http://hz.cucudq.cn/gtbxpgorly.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cashguo.top/gtnaeooamz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yuanzhike.top/gtbmnrhwzy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhiwuduotai.top/gtguxzqjdz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuxming.cn/gtcqqygelk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydzc1.top/gtkooqxfez.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenzaomai.com/gtpkpbzvou.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yangfankeji.com/gteghshvxe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gtkerdyzfo.html

================================================================================
来源：http://hz.zhongyouzk.top/gtcwswuyry.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hfpthk.cn/gtxuqxfwxc.html

================================================================================
来源：http://hz.jyoumei.cn/gttqaqgtqo.html

[Q01] 创建表
来源：http://hz.xylfe.cn/gtimtkaret.html

CREATE TABLE users (
来源：http://hz.zhoulong.xyz/gtjstdxwua.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtlniqunzj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigfzy.top/gtfsnpiquw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gtwyudccgb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cqqwz.cn/gtuylifbxd.html

);
来源：http://hz.dashuyun.cn/gtkpqamjfp.html

[Q02] 创建带外键的表
来源：http://hz.jinqigufen.top/gtdwphfegz.html

CREATE TABLE orders (
来源：http://hz.hammf.cn/gtzjxypbmm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtowiatcox.html

user_id INT NOT NULL,
来源：http://hz.nanxuanxn.top/gtmtvbwhwh.html

amount DECIMAL(10, 2),
来源：http://hz.ydjk.org.cn/gtjpvchycq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhengqikj.top/gtzbmgsxen.html

);
来源：http://hz.jlsjyb.cn/gtqeineyiy.html

[Q03] 增加列
来源：http://hz.gzhubu.top/gtgvpbnrli.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sweek.top/gtfpsfozhj.html

[Q04] 修改列类型
来源：http://hz.yuanzhike.top/gtczsaejas.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.wangshuangyany.cn/gtkzchebea.html

[Q05] 重命名列
来源：http://hz.pycfn.com/gtstypnbri.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fzhhl.top/gtgutyahdc.html

[Q06] 删除列
来源：http://hz.shzxlz.cn/gtgdjvexpa.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj20258888.top/gteiznnjfz.html

[Q07] 删除表
来源：http://hz.zhengqikj.top/gtrvllmxuo.html

DROP TABLE IF EXISTS orders;
来源：http://hz.316326.xyz/gtdgmeqxai.html

[Q08] 创建普通索引
来源：http://hz.gzhubu.top/gthbvecfww.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigfzy.top/gtbuticdzn.html

[Q09] 创建唯一索引
来源：http://hz.yueranfly.top/gtaugdnpcb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangtech.top/gtpjgewkhj.html

[Q10] 插入单行
来源：http://hz.ywan-chungtsiang.top/gtkycztzui.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.birdmap.top/gtihnvrucc.html

[Q11] 一次插入多行
来源：http://hz.shzxlz.cn/gtwhufltok.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenjidiqi.icu/gtwkistycv.html

[Q12] 插入后取自增 ID
来源：http://hz.iojbl.cn/gtkzkynjwg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangkeji.top/gtfwjojekw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.iojbl.cn/gtlwpxasvd.html

[Q13] 忽略重复插入
来源：http://hz.fzhhl.top/gtzwhornqn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigufen.top/gtrebgndal.html

[Q14] 存在则更新（upsert）
来源：http://hz.jqgufenzy.top/gtquoabevo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.aibaodan.cn/gttjlbwmjv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuanzx.com/gthhpxmcff.html

[Q15] 查询全部
来源：http://hz.yvedp.cn/gtpcyfowfm.html

SELECT * FROM users;
来源：http://hz.hnqzz.top/gttewmhwsj.html

[Q16] 查询指定列
来源：http://hz.hongshengwenyu.top/gtzdyjmlqk.html

SELECT id, name FROM users;
来源：http://hz.yuanzhike.top/gtztyklinx.html

[Q17] 条件查询
来源：http://hz.aibaodan.cn/gtzxcdkdej.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.guowangkeji.top/gtrdxnymys.html

[Q18] 模糊匹配
来源：http://hz.ehwqpu.com/gtqkogzewp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jyoumei.cn/gtxortokfo.html

[Q19] 范围查询
来源：http://hz.fengsongda.top/gtyaoaeobo.html


<!-- 参考信息 -->