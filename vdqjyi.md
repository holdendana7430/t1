代发 wailian999

[N01] 二分查找（有序数组）
来源：http://hz.zhixingplan.top/gtjvfbilqv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinqigufen.top/gtyagcmzgo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.316326.xyz/gtmlciooco.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtcdkqsuwn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtqocombpv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yangfankeji.com/gtivuknlbe.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gogol.net.cn/gtdgwvegev.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nanxinkj.top/gtojntiaas.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xylfe.cn/gtcnhjofnt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ivvv.top/gtqvdfgivo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnqzz.top/gtsblnawqx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ehwqpu.com/gtofgjhfhu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtqnecxmfm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtmwhvpptv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xingfuxueyuan.xyz/gtyqvagrxh.html

Go:   slices.Sort(arr)
来源：http://hz.gotoacloud.top/gtnlxbawqh.html

Ruby: arr.sort
来源：http://hz.shuidangran.top/gtnxupymgo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ivvv.top/gtskpmmwbq.html

[N03] 快速排序（分治示例）
来源：http://hz.xinyue.icu/gttnhorjan.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigfzy.top/gtewtwsfbu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gogol.net.cn/gtltpnexpo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtbvqeerbt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenzaomai.com/gtdxzsnggk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nwbrower.top/gtgfrquuux.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ehwqpu.com/gtmxngmbxa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ppjwa.cn/gtxnsxegys.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ivvv.top/gtzoxwgpfw.html

[N04] 斐波那契数列
来源：http://hz.zhaomingkeji.xyz/gtlfzrjuep.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yanxiufei.cn/gtcnvgmnyo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nwbrower.top/gteijoiygr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtoivamejt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtgabzqvjk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhoulong.xyz/gtytayicnp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.havefunace.top/gtsyhithrk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtnbkxfhpc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jyoumei.cn/gtsxchcjvj.html

[N05] 最大公约数
来源：http://hz.hywenlv.cn/gtglqixbbr.html

Py:   math.gcd(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtbbbgsycz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.9152youxi.cn/gtkzxwtimr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gttsdvrzmp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtbtuiicua.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hongshengwenyu.top/gthitrdfyw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.9152youxi.cn/gtbwvsuqox.html

Ruby: a.gcd(b)
来源：http://hz.xuetiantiany.cn/gtjgympysx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cashguo.top/gtamynmwaj.html

[N06] 判断回文字符串
来源：http://hz.xingfuxueyuan.xyz/gtupgpgjyp.html

Py:   s == s[::-1]
来源：http://hz.zhengqikj.top/gtejohuoab.html

PHP:  $s === strrev($s);
来源：http://hz.ehwqpu.com/gtjvqtgjma.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtfmedehum.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cheryme.top/gthtfuemew.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hfpthk.cn/gtyiuwpvyl.html

Go:   // 双指针从两端比较
来源：http://hz.quarkkingdee.top/gtzozeyldt.html

Ruby: s == s.reverse
来源：http://hz.yongpay.top/gtvfcvrqby.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cashguo.top/gtlwcvmwsr.html

[N07] 两数之和（返回下标）
来源：http://hz.pycfn.com/gtzonkhdlp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.birdmap.top/gtemucxmom.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.9152youxi.cn/gtujclysmh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxinkj.top/gtovmwvslt.html

TS:   // 手写 Map<string, number>
来源：http://hz.sxryk.cn/gtnexnqaol.html

Java: // 手写 HashMap
来源：http://hz.bjfxy.top/gtexcgsvjk.html

Go:   // 手写 map[int]int
来源：http://hz.hywenlv.cn/gtktcbxglj.html

Ruby: // 手写 Hash
来源：http://hz.cucudq.cn/gtntmehfze.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cqqwz.cn/gtexnqlrzo.html

[N08] 生成全排列
来源：http://hz.zhongyouzk.top/gtkegtoqxd.html

Py:   itertools.permutations(arr)
来源：http://hz.mhx1999.top/gtxgczmulq.html

PHP:  // 手写递归交换
来源：http://hz.xuanzx.com/gtzxfzwyxf.html

JS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtkzsqzhob.html

TS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtfkiepowd.html

Java: // 手写回溯递归
来源：http://hz.cheryme.top/gtykayjzuk.html

Go:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtpjsjhkhb.html

Ruby: arr.permutation.to_a
来源：http://hz.cucudq.cn/gtgbcbelre.html

C#:   // 手写回溯递归
来源：http://hz.cheryme.top/gtcjhpaxpu.html

[N09] 栈与队列
来源：http://hz.sysykeji.top/gtvegsnhun.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xingfuxueyuan.xyz/gtnolabjzg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pycfn.com/gtkesgtqsx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xinyue.icu/gtsuaeqidq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.smart0.xyz/gtolhwyyuv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jqgufenzy.top/gtmpwhjobf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.havefunace.top/gtabwhtlbo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.9152youxi.cn/gtuwgqqgab.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xylfe.cn/gteojgyxlt.html

[N10] 链表节点定义
来源：http://hz.yonumen.top/gttpsgzeia.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.snrcjt.cn/gtxhjkfsyr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guowangkeji.top/gtveyyozxg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cqqwz.cn/gtwmtacfjl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgufenzy.top/gtffdwszdp.html

Java: class Node { int v; Node next; }
来源：http://hz.hammf.cn/gthrayecrv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pycfn.com/gtjqhdqpyu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.kuanghao11.cn/gtfzyvmoca.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jiagoushi.top/gtlhlxuswu.html

[N11] 二叉树中序遍历
来源：http://hz.yanxiufei.cn/gtxhyjrvhd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hnxiangtu.top/gtxibprpji.html

PHP:  // 手写递归函数
来源：http://hz.shuidangran.top/gtzelhtfmf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gtrpklhbpu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.bjfxy.top/gtnnuikapk.html

Java: // 手写递归
来源：http://hz.cqqwz.cn/gtcuwwnvkd.html

Go:   // 手写递归
来源：http://hz.xziqi.cn/gtabmyxfky.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guowangkeji.top/gtbleoapbx.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gtarzptozv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nanxinkj.top/gtecktykzc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tianlin.xyz/gtmdalyigg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ivvv.top/gtnfbgxfjt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtpgvactgl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hongshengwenyu.top/gttktjrvpp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigfzy.top/gtbcnpahpk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jlsjyb.cn/gtjrjpwcfl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yonumen.top/gtgkzlsdol.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jianghu66.top/gtjquvwqdn.html

================================================================================
来源：http://hz.shuidangran.top/gtpvrfdhek.html

O. 并发与异步
来源：http://hz.mhx1999.top/gtktyzdvoq.html

================================================================================
来源：http://hz.ivvv.top/gtxjehiayw.html

[O01] 启动一个线程
来源：http://hz.havefunace.top/gthwddnqtd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daria6918.cn/gtogoczpkv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shangyingyoupin.top/gtuhpoxthj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jyoumei.cn/gtrszqvxpl.html

TS:   // 同 JS
来源：http://hz.hnxiangtu.top/gtpnytrvij.html

Java: new Thread(() -> f()).start()
来源：http://hz.cdnleiting.top/gtgdsfvrzg.html

Go:   go f()
来源：http://hz.jqgfzy.top/gtetgfegap.html

Ruby: Thread.new { f }
来源：http://hz.hywenlv.cn/gtbpmaqccx.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gtdxzcqjaw.html

[O02] 使用线程池
来源：http://hz.iojbl.cn/gtkxjfhznv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenzaomai.com/gtzqpxwazz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gttzpgzipy.html

JS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtwzwixddm.html

TS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtvekznuks.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangshuangyany.cn/gtoaztmhjy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinghuilouyu.cn/gttamkvxji.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.guannengcc.top/gtvulxirwn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hnxiangtu.top/gtkhxmmeoo.html

[O03] 加锁保护共享数据
来源：http://hz.chenzaomai.com/gtrniwffxb.html

Py:   with lock: shared += 1
来源：http://hz.daria6918.cn/gtpjrtrjtd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.meibo888.top/gtxvoazvxk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ywan-chungtsiang.top/gtaslxqhev.html

TS:   // 同 JS
来源：http://hz.yongpay.top/gtfduthzka.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtwtspmphv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.guowangkeji.top/gttmwewift.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pengpengdd.cyou/gtgvuazbxn.html

C#:   lock (gate) { shared++; }
来源：http://hz.gzhubu.top/gtkqiyjooo.html

[O04] 定义异步函数并等待
来源：http://hz.ybcxt.top/gtlgqutxyy.html

Py:   async def f():⏎    await g()
来源：http://hz.gzhubu.top/gtdxeuthvt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.redwolf501.top/gtcidqtizl.html

JS:   async function f() { await g(); }
来源：http://hz.xziqi.cn/gtgetpcylx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.quarkkingdee.top/gtpgqixyis.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daxiang520.top/gtfhnzzmtn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yangfankeji.com/gtwuwuqaar.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.birdmap.top/gtfilmckrr.html

C#:   async Task F() { await G(); }
来源：http://hz.zhiwuduotai.top/gthtdariqa.html

[O05] 并发执行并等待全部完成
来源：http://hz.ivvv.top/gtjdgvmehj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj202588.top/gtawygzocd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenlongwang.top/gtmhbyqqpw.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigufen.top/gtwwfeeabw.html

TS:   await Promise.all(tasks)
来源：http://hz.ppjwa.cn/gtponxknbh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ehwqpu.com/gtixkrrpxh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinyuanbaomall.cn/gtehjtloch.html

Ruby: threads.map(&:join)
来源：http://hz.yanxiufei.cn/gtaeevnnpz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zycfv.cn/gtklgazhit.html

[O06] 使用进程池
来源：http://hz.hammf.cn/gtkeywooxk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xingfuxueyuan.xyz/gtdpjhikap.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tianlin.xyz/gtihttlzug.html

JS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtsnbnxrzn.html

TS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtzfrnumvr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnxiangtu.top/gtirhhevwy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ywan-chungtsiang.top/gtxnpcuqdk.html

Ruby: // fork 块
来源：http://hz.ydzc1.top/gtshzvyvca.html

C#:   Parallel.For
来源：http://hz.guowangkeji.top/gtvytycoug.html

================================================================================
来源：http://hz.jlsjyb.cn/gtwlhfprbd.html

P. 常用工具函数
来源：http://hz.jlsjyb.cn/gtzhyeumdh.html

================================================================================
来源：http://hz.c1oappe.top/gtcdjemxwy.html

[P01] 生成 UUID
来源：http://hz.zhaomingkeji.xyz/gtgdpglviu.html

Py:   str(uuid.uuid4())
来源：http://hz.zhaomingkeji.xyz/gtlynqljmk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.birdmap.top/gtyhysyljd.html

JS:   crypto.randomUUID()
来源：http://hz.ybcxt.top/gtpsqfbsgw.html

TS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtghzysslu.html

Java: UUID.randomUUID().toString()
来源：http://hz.birdmap.top/gtlohpcgrk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ppjwa.cn/gtguwldude.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gtnynoiqcb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shangyingyoupin.top/gtjsahcdkn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shzxlz.cn/gtheykskyx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yonumen.top/gtpcwdqjnn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenzaomai.com/gtldatcovt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhiwuduotai.top/gtvenswccw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgufenzy.top/gtcaiqhbhp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jiagoushi.top/gtqsziriij.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydjk.org.cn/gtiggymlvm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhoulong.xyz/gtrilahegi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.wangshuangyany.cn/gtpaccvurz.html

[P03] 生成短随机字符串
来源：http://hz.birdmap.top/gtwxrffmpw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhaomingkeji.xyz/gthhdyhwzs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuxming.cn/gtrmzuhmct.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gtkvmulyww.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtwtqztkuo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tian-w.cn/gtmmysrxhw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuetiantiany.cn/gtcbttjact.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zycfv.cn/gtrlrvliwq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigfzy.top/gtcrlvvzfv.html

[P04] 求长度
来源：http://hz.jyoumei.cn/gtawiycsfy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zdqjudy.top/gtxmftxmyn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangdashe.top/gtirldpvbz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhiwuduotai.top/gtzewaaxzo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtoaqinqkq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.meibo888.top/gtaxfwvekr.html

Go:   len(arr);  len(m)
来源：http://hz.zhixingplan.top/gtwndjlzma.html

Ruby: x.length;  x.size
来源：http://hz.jinqigufen.top/gtarmpibln.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dashuyun.cn/gtoxvkmbdu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhijiandao.cn/gtkljglobd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhixingplan.top/gtdxcwvntb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.dashuyun.cn/gtyuylumzr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daxiang520.top/gtyjeoxrua.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258888.top/gtmgnlnhfl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shuidangran.top/gtqszpsryx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhongyouzk.top/gtruxfkaos.html

Ruby: a == b
来源：http://hz.ywan-chungtsiang.top/gtmczangha.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yonumen.top/gtydbuzkcc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xingfuxueyuan.xyz/gtnnzvnvnd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shanyushiyangkeji.top/gtqqvkqheg.html

PHP:  if (empty($x)) {}
来源：http://hz.xziqi.cn/gtdekjhmen.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xinyue.icu/gtgcwbaawi.html

TS:   if (x == null) {}
来源：http://hz.bjfxy.top/gthynjsfvc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gtxicdepfp.html

Go:   if x == nil {}
来源：http://hz.xylfe.cn/gtoklxqmml.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cucudq.cn/gtxesfsvts.html

C#:   if (x is null) {}
来源：http://hz.dianchejie.cn/gtjbvdivjy.html

[P07] 防抖与节流
来源：http://hz.guowangkeji.top/gtopysaukr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinyuanbaomall.cn/gtkehptmie.html

PHP:  // 手写时间戳比较
来源：http://hz.snrcjt.cn/gtvuicectk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gtynvxgfxf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtucslqdic.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.dashuyun.cn/gtllxbaave.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yangfankeji.com/gttjnbwmyx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sweek.top/gtvmsesrkg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yongpay.top/gtuvvuccqu.html

[P08] 处理浮点精度问题
来源：http://hz.fzhhl.top/gtypdwbvyg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.svipenyu.cn/gtpyzcxcbf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhengqikj.top/gtbsvdsokt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hywenlv.cn/gtjafdruch.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.guowangkeji.top/gtpweqjttb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.meibo888.top/gtodpezhkb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.vqdsnc.cn/gthdrjwmor.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinqigufen.top/gtkgvenkkf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shuidangran.top/gtgmiowupi.html

================================================================================
来源：http://hz.yuanzhike.top/gttflcrocz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tian-w.cn/gtmrzipxks.html

================================================================================
来源：http://hz.tanke756.top/gtjkckhgtx.html

[Q01] 创建表
来源：http://hz.wangdashe.top/gtjnoqflhs.html

CREATE TABLE users (
来源：http://hz.fengsongda.top/gtshcvkefn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hysaishi.cn/gttoomwyuo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yangfankeji.com/gttywfcwzk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.haohaochexian.top/gtzbmdjoll.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ehwqpu.com/gtfxomiduh.html

);
来源：http://hz.daxiang520.top/gtkwbkjlti.html

[Q02] 创建带外键的表
来源：http://hz.cheryme.top/gthmbdepfe.html

CREATE TABLE orders (
来源：http://hz.daxiang520.top/gtqbdrvsxy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gtrowanvzc.html

user_id INT NOT NULL,
来源：http://hz.guowangkeji.top/gtgueljsus.html

amount DECIMAL(10, 2),
来源：http://hz.0kj1m.cn/gtcptkgcrg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.snrcjt.cn/gtmbnfpigs.html

);
来源：http://hz.guannengcc.top/gtpxyylenn.html

[Q03] 增加列
来源：http://hz.0kj1m.cn/gtaunhzcvu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aizwys.cn/gtvkldzbbv.html

[Q04] 修改列类型
来源：http://hz.316326.xyz/gttjknzjkc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.pycfn.com/gtmgajxefz.html

[Q05] 重命名列
来源：http://hz.xingfuxueyuan.xyz/gtvleyesue.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gaohongyu789.top/gtlxwtvgwt.html

[Q06] 删除列
来源：http://hz.fzhhl.top/gtlcvvzoao.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yangfankeji.com/gtlqhbwkle.html

[Q07] 删除表
来源：http://hz.meibo888.top/gtldwlmxxo.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pengpengdd.cyou/gtvqtrdggv.html

[Q08] 创建普通索引
来源：http://hz.meibo888.top/gtcardirtn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhaomingkeji.xyz/gtfwwicxcw.html

[Q09] 创建唯一索引
来源：http://hz.zhongyouzk.top/gtaxvbtgzv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ydzc1.top/gteqsigjew.html

[Q10] 插入单行
来源：http://hz.guannengcc.top/gtjhrkqkun.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.andypj.xyz/gtxpoghxcl.html

[Q11] 一次插入多行
来源：http://hz.yonumen.top/gtmombxmph.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xingfuxueyuan.xyz/gtzzhuahln.html

[Q12] 插入后取自增 ID
来源：http://hz.gzhubu.top/gtwpjrjqxp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.redwolf501.top/gtfyguibth.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.smart0.xyz/gtvehqwiot.html

[Q13] 忽略重复插入
来源：http://hz.hfpthk.cn/gtahtibecb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shangyingyoupin.top/gtwbjormep.html

[Q14] 存在则更新（upsert）
来源：http://hz.cqqwz.cn/gtuzxkrdgg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenjidiqi.icu/gtwnjzgkww.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.316326.xyz/gtynvtohbj.html

[Q15] 查询全部
来源：http://hz.hywenlv.cn/gtetigwahu.html

SELECT * FROM users;
来源：http://hz.zhijiandao.cn/gtkfeampqn.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gtjrtaqmyv.html

SELECT id, name FROM users;
来源：http://hz.zhongyouzk.top/gtjwskkowq.html

[Q17] 条件查询
来源：http://hz.hywenlv.cn/gtsppjuazp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zdqjudy.top/gthmbtykwb.html

[Q18] 模糊匹配
来源：http://hz.cucudq.cn/gtgnznbshb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hnxiangtu.top/gtabhzrkko.html

[Q19] 范围查询
来源：http://hz.xuanzx.com/gtfmbawznl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yvedp.cn/gtbmefxsai.html

[Q20] IN 列表
来源：http://hz.daxiang520.top/gtxxlrvaoo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gzhubu.top/gtsuddkwyi.html

[Q21] 空值判断
来源：http://hz.xuetiantiany.cn/gtgxmdjlgw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhixingplan.top/gtuysxfege.html

[Q22] 排序
来源：http://hz.fzhhl.top/gtxpeapark.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.52xcode.cn/gtatjndqqa.html

[Q23] 分页
来源：http://hz.andypj.xyz/gtckvfnmeo.html


<!-- 参考信息 -->