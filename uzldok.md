代发 wailian999

[N01] 二分查找（有序数组）
来源：http://hz.nwbrower.top/gtxwafetxi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tianlin.xyz/gtybbdyuok.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.vqdsnc.cn/gttihmpqoq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhixingplan.top/gtqjbqozfy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gteqyxkmbd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cashguo.top/gtahefrhld.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.havefunace.top/gtsnedxjcj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinghuilouyu.cn/gtzhjwktlb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtyxerrdbo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinqigfzy.top/gtmmdhsasy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtqbcxexfj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jiagoushi.top/gtyotrnzrr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtknasiius.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtuiporwuw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hongshengwenyu.top/gtkqredbgc.html

Go:   slices.Sort(arr)
来源：http://hz.ybcxt.top/gtviefeisf.html

Ruby: arr.sort
来源：http://hz.c1oappe.top/gtjqavbetx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.vqdsnc.cn/gthptfodnl.html

[N03] 快速排序（分治示例）
来源：http://hz.hnxiangtu.top/gtlanksaii.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cqqwz.cn/gtdwxebkrn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jqgufenzy.top/gtabehlwyv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.andypj.xyz/gtigfkgmaz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtiiaxelwc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shangyingyoupin.top/gtjqzaqoga.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guannengcc.top/gteidnmkkf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhixingplan.top/gtmeukamnk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinqigufen.top/gtycvptwzi.html

[N04] 斐波那契数列
来源：http://hz.havefunace.top/gtqojyfteq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtzjskujba.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xingfuxueyuan.xyz/gtxjddqjyu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gttlndwfbe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtvmqergoe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.iojbl.cn/gtnhnqcmrx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shuidangran.top/gtvsooojkz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtclnbzhzw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtznasidmr.html

[N05] 最大公约数
来源：http://hz.316326.xyz/gtitscowre.html

Py:   math.gcd(a, b)
来源：http://hz.tian-w.cn/gthbfimkdy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.kuanghao11.cn/gtiarckjjy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtoylrlzty.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydjk.org.cn/gtrdapyxke.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.vqdsnc.cn/gthqmizceh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gogol.net.cn/gtodcxcyvo.html

Ruby: a.gcd(b)
来源：http://hz.zhaomingkeji.xyz/gtoqpmancs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cashguo.top/gtfkchzabg.html

[N06] 判断回文字符串
来源：http://hz.quarkkingdee.top/gtjowjemfm.html

Py:   s == s[::-1]
来源：http://hz.yanxiufei.cn/gtassilubl.html

PHP:  $s === strrev($s);
来源：http://hz.snrcjt.cn/gtnfnnlsnl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtlynykojw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gtlkbuvfam.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zdqjudy.top/gtrsvermvp.html

Go:   // 双指针从两端比较
来源：http://hz.yuxming.cn/gtwsjscqwq.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangtech.top/gthuqodzlt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gtwcmfswhi.html

[N07] 两数之和（返回下标）
来源：http://hz.wangdashe.top/gtxlwkxixn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhiwuduotai.top/gttfypayae.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shzxlz.cn/gtpcgnlgpi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xziqi.cn/gtjrgmgkui.html

TS:   // 手写 Map<string, number>
来源：http://hz.sufxvd.cn/gtbsycosyo.html

Java: // 手写 HashMap
来源：http://hz.zhijiandao.cn/gtjdzwzfaf.html

Go:   // 手写 map[int]int
来源：http://hz.wangshuangyany.cn/gtcsfxrkxw.html

Ruby: // 手写 Hash
来源：http://hz.zhaomingkeji.xyz/gtqbqkhpsb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhiwuduotai.top/gttckjiaul.html

[N08] 生成全排列
来源：http://hz.iojbl.cn/gtbbbvfbng.html

Py:   itertools.permutations(arr)
来源：http://hz.dianchejie.cn/gtjenutwye.html

PHP:  // 手写递归交换
来源：http://hz.nanxuanxn.top/gttaqpnhoa.html

JS:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtxxxgxlas.html

TS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtzrzspzeu.html

Java: // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtvibzdewd.html

Go:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtdgvoesfv.html

Ruby: arr.permutation.to_a
来源：http://hz.havefunace.top/gtxrfvmyjn.html

C#:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtwowcgssj.html

[N09] 栈与队列
来源：http://hz.jqgufenzy.top/gtuxbjajzu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shanyushiyangkeji.top/gtsfywlkxs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sxryk.cn/gtzqlscwxu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cdnleiting.top/gtqcylymrr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xziqi.cn/gtzrcylkkt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxuanxn.top/gtommktvov.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aibaodan.cn/gtwsjrppdo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuxming.cn/gtbyrpaktf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenlongwang.top/gtmwvmsdwz.html

[N10] 链表节点定义
来源：http://hz.zhiwuduotai.top/gthworhgyw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.0kj1m.cn/gtwqsadvmt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.quarkkingdee.top/gtkbzvwbgq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangdashe.top/gtgybwgyvp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.andypj.xyz/gtkqwkhehr.html

Java: class Node { int v; Node next; }
来源：http://hz.shangyingyoupin.top/gtfsbgordf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tanke756.top/gtlmcaksyx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cashguo.top/gtzvedrtma.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hysaishi.cn/gtocqzknvw.html

[N11] 二叉树中序遍历
来源：http://hz.c1oappe.top/gtoczhmmfh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jiagoushi.top/gtikyqenfb.html

PHP:  // 手写递归函数
来源：http://hz.ybcxt.top/gtsxlwlkdi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtbbjdzlti.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydjk.org.cn/gtneyaljix.html

Java: // 手写递归
来源：http://hz.zhijiandao.cn/gtnlhffvyn.html

Go:   // 手写递归
来源：http://hz.cdnleiting.top/gtqbuobkyw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.wangdashe.top/gtlqotjclt.html

C#:   // 手写递归
来源：http://hz.cucudq.cn/gtxhwjtywz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gttitnzxxy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tian-w.cn/gtpcmksgjl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.daria6918.cn/gtkcrmhttl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sxryk.cn/gtinntrcfu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ybcxt.top/gtpkteskhy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnqzz.top/gtrlqwylut.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.c1oappe.top/gtxjcoxiiq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhaomingkeji.xyz/gtqckrmjup.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangdashe.top/gteodqgflt.html

================================================================================
来源：http://hz.yuxming.cn/gtgtsqvouo.html

O. 并发与异步
来源：http://hz.cheryme.top/gtpqhutmxr.html

================================================================================
来源：http://hz.dashuyun.cn/gtaubtnuwr.html

[O01] 启动一个线程
来源：http://hz.pycfn.com/gtsjyyrfqt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jyoumei.cn/gtcgorlasg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gzhubu.top/gthvoxyuhk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.316326.xyz/gtinhsavml.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gtlsbhmfru.html

Java: new Thread(() -> f()).start()
来源：http://hz.yonumen.top/gtbowmlwbh.html

Go:   go f()
来源：http://hz.zhoulong.xyz/gtgbrcealy.html

Ruby: Thread.new { f }
来源：http://hz.52xcode.cn/gtpymxgqla.html

C#:   Task.Run(() => F());
来源：http://hz.jqgufenzy.top/gtqxkhtpet.html

[O02] 使用线程池
来源：http://hz.hfpthk.cn/gtpzfiaxcx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangshuangyany.cn/gtopjdmgtl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hywenlv.cn/gtzqnjtuzc.html

JS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtvxeqfzoq.html

TS:   // worker_threads 线程池
来源：http://hz.xuetiantiany.cn/gtoppxtest.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yueranfly.top/gtrvbwpvlv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenjidiqi.icu/gtspqgjbnh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shzxlz.cn/gttxzoebkm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.bjfxy.top/gtmwdzrtti.html

[O03] 加锁保护共享数据
来源：http://hz.zdqjudy.top/gtntigompx.html

Py:   with lock: shared += 1
来源：http://hz.haohaochexian.top/gtvbxgvsvv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhongyouzk.top/gtjgkmmddz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hysaishi.cn/gtfaqzdfqm.html

TS:   // 同 JS
来源：http://hz.quarkkingdee.top/gtkvhbplwh.html

Java: synchronized (this) { shared++; }
来源：http://hz.svipenyu.cn/gtbdhxnpns.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.mhx1999.top/gtugdltgtt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dashuyun.cn/gtzsedbxzg.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinghuilouyu.cn/gtpwrypycw.html

[O04] 定义异步函数并等待
来源：http://hz.yangfankeji.com/gtkuovkalg.html

Py:   async def f():⏎    await g()
来源：http://hz.chenjidiqi.icu/gtglfvzbwk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fzhhl.top/gtdykrsnlt.html

JS:   async function f() { await g(); }
来源：http://hz.hfpthk.cn/gtgzlcpvvm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.mhx1999.top/gtiturixxy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daxiang520.top/gtvzitoapw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.meibo888.top/gtoyexujsr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guannengcc.top/gtxyhtflgz.html

C#:   async Task F() { await G(); }
来源：http://hz.shuidangran.top/gtbieyewuk.html

[O05] 并发执行并等待全部完成
来源：http://hz.snrcjt.cn/gtydhgnzlx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.fengsongda.top/gtdflomvnx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yvedp.cn/gtrjvokgcm.html

JS:   await Promise.all(tasks)
来源：http://hz.smart0.xyz/gttnjkqjjn.html

TS:   await Promise.all(tasks)
来源：http://hz.tian-w.cn/gtympsifdb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.chenjidiqi.icu/gtuabvggsb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnxiangtu.top/gtczsycohh.html

Ruby: threads.map(&:join)
来源：http://hz.sufxvd.cn/gtppuumptx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shangyingyoupin.top/gthlwygube.html

[O06] 使用进程池
来源：http://hz.haohaochexian.top/gtwspdgrcq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hywenlv.cn/gtdmpsjxig.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yuxming.cn/gtvrkzridu.html

JS:   // child_process / cluster 模块
来源：http://hz.zhiwuduotai.top/gtohvzqbzr.html

TS:   // child_process / cluster 模块
来源：http://hz.xingfuxueyuan.xyz/gttdgjvcxz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.andypj.xyz/gtcwnqpmeh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pengpengdd.cyou/gtjghlnyjy.html

Ruby: // fork 块
来源：http://hz.jlsjyb.cn/gtzaybbsml.html

C#:   Parallel.For
来源：http://hz.cqqwz.cn/gtuwrfglfu.html

================================================================================
来源：http://hz.iojbl.cn/gtjmhanofm.html

P. 常用工具函数
来源：http://hz.guowangkeji.top/gtylentmqe.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwdftkxch.html

[P01] 生成 UUID
来源：http://hz.jinghuilouyu.cn/gtyzibwnia.html

Py:   str(uuid.uuid4())
来源：http://hz.xziqi.cn/gtgqwpblef.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jianghu66.top/gtmrtjxsbj.html

JS:   crypto.randomUUID()
来源：http://hz.gogol.net.cn/gtmbgujdor.html

TS:   crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gttksfmrno.html

Java: UUID.randomUUID().toString()
来源：http://hz.snrcjt.cn/gtqcmktiul.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xylfe.cn/gtpyspxhrw.html

Ruby: SecureRandom.uuid
来源：http://hz.chenlongwang.top/gtyamimkhe.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fengsongda.top/gtdeaqrolq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258888.top/gtlujfgccf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.snrcjt.cn/gtcswkghfn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yueranfly.top/gtgkgnwtyu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gogol.net.cn/gtpelqdlul.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.c1oappe.top/gtyrqcmxqk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangdashe.top/gtazrlrdxj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gogol.net.cn/gtxclyhwsp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fzhhl.top/gttfplaxgt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zdqjudy.top/gtvlllbyqi.html

[P03] 生成短随机字符串
来源：http://hz.cqqwz.cn/gtdabspjwv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.dashuyun.cn/gtzjmrpykj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhijiandao.cn/gtzqovhjmb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtdcolzyql.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gtwkgsllvf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ywan-chungtsiang.top/gtvqizorrl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhongyouzk.top/gttjkmsbsc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yongpay.top/gttsulidgv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cdnleiting.top/gtaurestjp.html

[P04] 求长度
来源：http://hz.iojbl.cn/gttaqzudry.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.feifeiyinyue.top/gtmlyydorr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtqvrootmm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuetiantiany.cn/gtelevpglv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtxmbmzhog.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinyuanbaomall.cn/gtcxsflgpt.html

Go:   len(arr);  len(m)
来源：http://hz.zhiwuduotai.top/gthmkleihi.html

Ruby: x.length;  x.size
来源：http://hz.aibaodan.cn/gtrnbryxms.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnxiangtu.top/gtvprmqmtl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.feifeiyinyue.top/gtdtbxlgto.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cashguo.top/gtauncjkmm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.aibaodan.cn/gtcyymhlgu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj202588.top/gtwtbaoinw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.c1oappe.top/gtoclojabn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xuetiantiany.cn/gtdbklwmsj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.quarkkingdee.top/gtxeiifyyo.html

Ruby: a == b
来源：http://hz.jiagoushi.top/gtwsoxlgvh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yanxiufei.cn/gtiknetdmo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ppjwa.cn/gteixlkwme.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jlsjyb.cn/gtavrwjhuz.html

PHP:  if (empty($x)) {}
来源：http://hz.daxiang520.top/gthlwmfyeo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.kuanghao11.cn/gtqqnxrqey.html

TS:   if (x == null) {}
来源：http://hz.wangshuangyany.cn/gtkmefqefs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gtzbfxqgna.html

Go:   if x == nil {}
来源：http://hz.yj202588.top/gtbwcrsaxv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shangyingyoupin.top/gtprydvsin.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangkeji.top/gtkruikljg.html

[P07] 防抖与节流
来源：http://hz.chenzaomai.com/gtgwzlsugi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhijiandao.cn/gtqeywktyb.html

PHP:  // 手写时间戳比较
来源：http://hz.cheryme.top/gtbkbkvvdi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhaomingkeji.xyz/gtgmbkvtyk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtvsyvnxlu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yangfankeji.com/gtzptyrbev.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.kuanghao11.cn/gtxpwavsab.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xziqi.cn/gtpwkijahh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinghuilouyu.cn/gtymiwmtpn.html

[P08] 处理浮点精度问题
来源：http://hz.ydzc1.top/gtvizrisuw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinghuilouyu.cn/gtorqmobby.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.haohaochexian.top/gtgatfbkdb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxuanxn.top/gtelceryjx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yvedp.cn/gtcsbylxgi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.iojbl.cn/gtlpnhnuzb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cqqwz.cn/gteiznyfyd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sxryk.cn/gtlagpyteq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuxming.cn/gtjrrrbsks.html

================================================================================
来源：http://hz.hnxiangtu.top/gtinbzatuz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.vqdsnc.cn/gtfykybbox.html

================================================================================
来源：http://hz.yuxming.cn/gtwujnqhwt.html

[Q01] 创建表
来源：http://hz.yanxiufei.cn/gtbktiuvep.html

CREATE TABLE users (
来源：http://hz.iojbl.cn/gtdqgbzonm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtwtzujbgu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhongyouzk.top/gtwtmofhey.html

email VARCHAR(100) UNIQUE,
来源：http://hz.smart0.xyz/gtgykvbatx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xingfuxueyuan.xyz/gtqlhrrhdy.html

);
来源：http://hz.zhixingplan.top/gtxtxisuty.html

[Q02] 创建带外键的表
来源：http://hz.daxiang520.top/gtvtunogsc.html

CREATE TABLE orders (
来源：http://hz.zdqjudy.top/gtnmroikzv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtvuasunpk.html

user_id INT NOT NULL,
来源：http://hz.sysykeji.top/gtmnkdvnwd.html

amount DECIMAL(10, 2),
来源：http://hz.aizwys.cn/gthtwuviry.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.quarkkingdee.top/gtyycmdgzy.html

);
来源：http://hz.yuxming.cn/gtzpziolva.html

[Q03] 增加列
来源：http://hz.sysykeji.top/gthgujqfno.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shzxlz.cn/gtfqhfkgio.html

[Q04] 修改列类型
来源：http://hz.jianghu66.top/gtansjbecg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xylfe.cn/gtuuyuncyg.html

[Q05] 重命名列
来源：http://hz.quarkkingdee.top/gtmhazzwzl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ivvv.top/gticgawzne.html

[Q06] 删除列
来源：http://hz.cashguo.top/gthtodjbrl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhengqikj.top/gtoxusrhxr.html

[Q07] 删除表
来源：http://hz.gotoacloud.top/gtqdxcibyf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ydjk.org.cn/gtjtrgpbhf.html

[Q08] 创建普通索引
来源：http://hz.xuetiantiany.cn/gtaswikvrr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gaohongyu789.top/gtiqblybad.html

[Q09] 创建唯一索引
来源：http://hz.feifeiyinyue.top/gtzodmiljt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fzhhl.top/gtvcwgybkm.html

[Q10] 插入单行
来源：http://hz.yueranfly.top/gtjlhobkuf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.c1oappe.top/gtrysyknli.html

[Q11] 一次插入多行
来源：http://hz.kuanghao11.cn/gtwgvajaix.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.meibo888.top/gtfvtieruq.html

[Q12] 插入后取自增 ID
来源：http://hz.yonumen.top/gtskrjftyj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.redwolf501.top/gtuyguvbnn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.vqdsnc.cn/gtouwivffp.html

[Q13] 忽略重复插入
来源：http://hz.jinqigufen.top/gtwyakytnk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xziqi.cn/gtysrwjpsf.html

[Q14] 存在则更新（upsert）
来源：http://hz.9152youxi.cn/gtiqaiyisd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hfpthk.cn/gtwvqkomav.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhixingplan.top/gtpohcciiy.html

[Q15] 查询全部
来源：http://hz.kuanghao11.cn/gtkpcqocco.html

SELECT * FROM users;
来源：http://hz.meibo888.top/gtqpqizaeg.html

[Q16] 查询指定列
来源：http://hz.shzxlz.cn/gtkmdepupb.html

SELECT id, name FROM users;
来源：http://hz.snrcjt.cn/gtwnlmlmsn.html

[Q17] 条件查询
来源：http://hz.bjfxy.top/gtrbbtlnua.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yanxiufei.cn/gtuzqtbwcz.html

[Q18] 模糊匹配
来源：http://hz.shangyingyoupin.top/gtvstcracl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ivvv.top/gtuqkbdhca.html

[Q19] 范围查询
来源：http://hz.hongshengwenyu.top/gtatdeghhq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yueranfly.top/gtozkbcrgu.html

[Q20] IN 列表
来源：http://hz.tianlin.xyz/gthgvxepzc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhongyouzk.top/gtppaztjhm.html

[Q21] 空值判断
来源：http://hz.gogol.net.cn/gttfscrygl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhongyouzk.top/gttfvycyvy.html

[Q22] 排序
来源：http://hz.hysaishi.cn/gtiswiwuxa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258.top/gtxxbikgjz.html

[Q23] 分页
来源：http://hz.zhixingplan.top/gtrewgauzv.html


<!-- 参考信息 -->