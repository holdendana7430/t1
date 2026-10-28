代发 wailian999

[N01] 二分查找（有序数组）
来源：http://hz.xuetiantiany.cn/gtbblwziam.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.guowangkeji.top/gtkkexnlic.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinyuanbaomall.cn/gtuqlbvxrh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtyhsjkfkr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtfzrbhqyi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gtxerbdfao.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xziqi.cn/gtdkhuqwqc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tianlin.xyz/gtzaivmvcy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtsyosaebd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinqigufen.top/gtywuyfgkm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnqzz.top/gtbfiarkrt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tian-w.cn/gtvktmcnzx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtbwrqpegr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtpryeevyg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hammf.cn/gtwqidrdwq.html

Go:   slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtzluccxug.html

Ruby: arr.sort
来源：http://hz.meibo888.top/gthbvckfwi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.bjfxy.top/gtavmwwsmi.html

[N03] 快速排序（分治示例）
来源：http://hz.ydjk.org.cn/gtbawcfpaz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sweek.top/gtnirpfhcj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhixingplan.top/gtmdygmzwa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gterglgplm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtdpqwlnjx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ywan-chungtsiang.top/gtdvxipxcx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hfpthk.cn/gtotpirrfy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cheryme.top/gtegqmqapq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgufenzy.top/gtbzengjtj.html

[N04] 斐波那契数列
来源：http://hz.xuetiantiany.cn/gtckabheja.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jiagoushi.top/gticknrykb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangtech.top/gtcmkvriwa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtupavzceh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangdashe.top/gtxbjwichh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gtdkqmmwyx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.dashuyun.cn/gttjsnahbc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtkbcinxte.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dianchejie.cn/gtqnitegcb.html

[N05] 最大公约数
来源：http://hz.yanxiufei.cn/gtskfgpoxi.html

Py:   math.gcd(a, b)
来源：http://hz.xuanzx.com/gtwbpzlzex.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnqzz.top/gtrnvlwpqi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guowangkeji.top/gtjvtgwyox.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnxiangtu.top/gtlxgmexua.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinqigfzy.top/gtsjeobmto.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.0kj1m.cn/gtwtikoyhr.html

Ruby: a.gcd(b)
来源：http://hz.jinyuanbaomall.cn/gthgtehxki.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhixingplan.top/gtulxvrsbx.html

[N06] 判断回文字符串
来源：http://hz.chenlongwang.top/gtfbbpnvky.html

Py:   s == s[::-1]
来源：http://hz.xuanzx.com/gtyuqfvdfx.html

PHP:  $s === strrev($s);
来源：http://hz.xylfe.cn/gtkxyqhmgr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.316326.xyz/gtpdjnbezb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtuwmbfvgq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nwbrower.top/gtfsuoenif.html

Go:   // 双指针从两端比较
来源：http://hz.kuanghao11.cn/gtfswsurwd.html

Ruby: s == s.reverse
来源：http://hz.cdnleiting.top/gtoowbmolh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtjhixlrpv.html

[N07] 两数之和（返回下标）
来源：http://hz.yuanzhike.top/gtbvabopaq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenzaomai.com/gtzwhxsjis.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.daria6918.cn/gtmxpsemhx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydzc1.top/gtdmqhvlwf.html

TS:   // 手写 Map<string, number>
来源：http://hz.hywenlv.cn/gtuyonzhyz.html

Java: // 手写 HashMap
来源：http://hz.xylfe.cn/gtiqjmhtiy.html

Go:   // 手写 map[int]int
来源：http://hz.jyoumei.cn/gtouuvzita.html

Ruby: // 手写 Hash
来源：http://hz.52xcode.cn/gtxlhybdmy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxuanxn.top/gtvuejokgy.html

[N08] 生成全排列
来源：http://hz.redwolf501.top/gtzzcxokde.html

Py:   itertools.permutations(arr)
来源：http://hz.jyoumei.cn/gtawmdjuct.html

PHP:  // 手写递归交换
来源：http://hz.jianghu66.top/gtanuubcvy.html

JS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtidkmdbrc.html

TS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtvpwashio.html

Java: // 手写回溯递归
来源：http://hz.chenzaomai.com/gtkgdjjrey.html

Go:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtvddpebka.html

Ruby: arr.permutation.to_a
来源：http://hz.52xcode.cn/gtmlqegies.html

C#:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtooenavbt.html

[N09] 栈与队列
来源：http://hz.hammf.cn/gtmbsawfbq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cdnleiting.top/gtlxbzjnlt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.meibo888.top/gtcoeatwfn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xylfe.cn/gtmehyphed.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangtech.top/gtmugulcvq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yangfankeji.com/gtjhbzgvmm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ppjwa.cn/gtovgtkqhi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangkeji.top/gtbhyndowt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gaohongyu789.top/gtldplqdzl.html

[N10] 链表节点定义
来源：http://hz.ydjk.org.cn/gtzawfuinu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydjk.org.cn/gtigkanehz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.bjfxy.top/gtcdevgaph.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yuanzhike.top/gtxedzzidn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xuetiantiany.cn/gtbbefgnus.html

Java: class Node { int v; Node next; }
来源：http://hz.nanxuanxn.top/gtkjgqeqdw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.mhx1999.top/gtixgvogsh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnqzz.top/gtvukcfipn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ydzc1.top/gtwhdopvwe.html

[N11] 二叉树中序遍历
来源：http://hz.havefunace.top/gtcfcdculw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nanxinkj.top/gtclenxpnv.html

PHP:  // 手写递归函数
来源：http://hz.guannengcc.top/gtntcpavjj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigfzy.top/gtegowsmku.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigufen.top/gtbfceqlkv.html

Java: // 手写递归
来源：http://hz.jyoumei.cn/gtterkeuxm.html

Go:   // 手写递归
来源：http://hz.hfpthk.cn/gtdbvpitir.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daxiang520.top/gtrtokcfsj.html

C#:   // 手写递归
来源：http://hz.jlsjyb.cn/gtdrraxvin.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnqzz.top/gtjujuzukk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.mhx1999.top/gtqpqmevao.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yongpay.top/gtcdvzltzb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gtymfkdyil.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtppkdqkqi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dashuyun.cn/gttydkaqjf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenjidiqi.icu/gtvmpfvdkz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ywan-chungtsiang.top/gtkyhelevk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gtikxblrdu.html

================================================================================
来源：http://hz.jinqigufen.top/gttzbfbiek.html

O. 并发与异步
来源：http://hz.zhoulong.xyz/gtamxhlnor.html

================================================================================
来源：http://hz.sysykeji.top/gtyoofnvzf.html

[O01] 启动一个线程
来源：http://hz.feifeiyinyue.top/gtypjqiobp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tian-w.cn/gtylrwydvs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jiagoushi.top/gtcfojvrlw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jlsjyb.cn/gtvrbafbkd.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtknbifcsm.html

Java: new Thread(() -> f()).start()
来源：http://hz.nwbrower.top/gtszgzetyy.html

Go:   go f()
来源：http://hz.shzxlz.cn/gtfptuyjea.html

Ruby: Thread.new { f }
来源：http://hz.vqdsnc.cn/gtntnwpvcn.html

C#:   Task.Run(() => F());
来源：http://hz.vqdsnc.cn/gtisscznmz.html

[O02] 使用线程池
来源：http://hz.gzhubu.top/gtaztyhbet.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xylfe.cn/gtcpwdmime.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhengqikj.top/gtrqindqve.html

JS:   // worker_threads 线程池
来源：http://hz.nwbrower.top/gtxaqvgmmi.html

TS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtbbmqmxpo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.52xcode.cn/gtjujsdemy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zycfv.cn/gtvlgcktvo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.redwolf501.top/gtkzcsogxa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.52xcode.cn/gtarrguxtj.html

[O03] 加锁保护共享数据
来源：http://hz.zhongyouzk.top/gtysjheywy.html

Py:   with lock: shared += 1
来源：http://hz.jyoumei.cn/gthrfejztf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ppjwa.cn/gtusmkphnj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuxming.cn/gtzktdmkrj.html

TS:   // 同 JS
来源：http://hz.jinyuanbaomall.cn/gtezorbsic.html

Java: synchronized (this) { shared++; }
来源：http://hz.tian-w.cn/gtfnquncda.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ivvv.top/gtbgmrloxu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cdnleiting.top/gtcggasjaj.html

C#:   lock (gate) { shared++; }
来源：http://hz.andypj.xyz/gtmtgcsrwy.html

[O04] 定义异步函数并等待
来源：http://hz.tianlin.xyz/gtuuewylru.html

Py:   async def f():⏎    await g()
来源：http://hz.andypj.xyz/gtdyvcannj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinghuilouyu.cn/gtmklffrel.html

JS:   async function f() { await g(); }
来源：http://hz.cdnleiting.top/gtkadzixka.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxuanxn.top/gttbojbnvq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ppjwa.cn/gtbijhqnnq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jyoumei.cn/gtavrhngac.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nwbrower.top/gtsyongllj.html

C#:   async Task F() { await G(); }
来源：http://hz.gogol.net.cn/gtlxdyrptm.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258.top/gtzyodhvfd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yvedp.cn/gtgrsfsmud.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinqigfzy.top/gtqlytcpbg.html

JS:   await Promise.all(tasks)
来源：http://hz.gaohongyu789.top/gtzqrjxeun.html

TS:   await Promise.all(tasks)
来源：http://hz.jqgfzy.top/gtbafeyamf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nwbrower.top/gtupuwiyav.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenzaomai.com/gtexiacovj.html

Ruby: threads.map(&:join)
来源：http://hz.tianlin.xyz/gtspvkrnnt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xuanzx.com/gtwrlrfldw.html

[O06] 使用进程池
来源：http://hz.ydzc1.top/gtbdktugwc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhijiandao.cn/gtpezlfyic.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.havefunace.top/gtrkdknfns.html

JS:   // child_process / cluster 模块
来源：http://hz.zhengqikj.top/gtvgvuzdvy.html

TS:   // child_process / cluster 模块
来源：http://hz.jinghuilouyu.cn/gtcsrgwzcp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jianghu66.top/gtxlpqojyr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtktgyzdgq.html

Ruby: // fork 块
来源：http://hz.sxryk.cn/gtuuaaibhc.html

C#:   Parallel.For
来源：http://hz.redwolf501.top/gtsjijzhke.html

================================================================================
来源：http://hz.cdnleiting.top/gtmjjzujrg.html

P. 常用工具函数
来源：http://hz.shzxlz.cn/gtfyswxsff.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtwwlxtrxw.html

[P01] 生成 UUID
来源：http://hz.bjfxy.top/gtwmmzlkiw.html

Py:   str(uuid.uuid4())
来源：http://hz.gogol.net.cn/gtttutbkkj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xylfe.cn/gtaxmxveqn.html

JS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtnrxccyhv.html

TS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtiqyissdq.html

Java: UUID.randomUUID().toString()
来源：http://hz.xinyue.icu/gtaplqbmlm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nanxinkj.top/gtelortaks.html

Ruby: SecureRandom.uuid
来源：http://hz.daria6918.cn/gtgxpjmoim.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhiwuduotai.top/gtvcjkirqc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tanke756.top/gterhkxhuv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhaomingkeji.xyz/gtutpimvnw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.0kj1m.cn/gtsvlfbalo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhongyouzk.top/gtzgrizfxh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigufen.top/gttepzakap.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tianlin.xyz/gtnmravfvz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jyoumei.cn/gtghwvgyjm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhaomingkeji.xyz/gtpxfplusi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydjk.org.cn/gteesdyhxa.html

[P03] 生成短随机字符串
来源：http://hz.hongshengwenyu.top/gtczjphoxg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pycfn.com/gtpepdudsz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.svipenyu.cn/gtefzmbxru.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtodqrkivu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenzaomai.com/gtzuisesxn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tian-w.cn/gthumikdna.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ehwqpu.com/gtjvfrqhar.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.bjfxy.top/gtwfcxjaso.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yueranfly.top/gtnvuukzyp.html

[P04] 求长度
来源：http://hz.bjfxy.top/gtipqhhmlk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangtech.top/gtyvmvjgtf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtvrokqupk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtagzbvzxv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gttwansdzu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sufxvd.cn/gtlcwicrom.html

Go:   len(arr);  len(m)
来源：http://hz.yueranfly.top/gtrdqoewxb.html

Ruby: x.length;  x.size
来源：http://hz.ydjk.org.cn/gtyykgcgfv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.bjfxy.top/gteotwjzei.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hongshengwenyu.top/gtmdsooogj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tianlin.xyz/gtgyepdnvd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jlsjyb.cn/gtyeunhrow.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cucudq.cn/gtejfacipz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtwrmsrrwr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.quarkkingdee.top/gtdnyqaorv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxuanxn.top/gtbtxeomxr.html

Ruby: a == b
来源：http://hz.yj202588.top/gtbiqnyuhc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gogol.net.cn/gtkihqgbcf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fzhhl.top/gtixeeyhma.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yvedp.cn/gtjlyhjebj.html

PHP:  if (empty($x)) {}
来源：http://hz.wangdashe.top/gtoexqqwcj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sxryk.cn/gticzgrpad.html

TS:   if (x == null) {}
来源：http://hz.andypj.xyz/gtszmooexj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.feifeiyinyue.top/gtnuomumyj.html

Go:   if x == nil {}
来源：http://hz.yongpay.top/gtqugpqjzm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gotoacloud.top/gtxctoknnu.html

C#:   if (x is null) {}
来源：http://hz.jqgfzy.top/gtcpdckkjh.html

[P07] 防抖与节流
来源：http://hz.jqgfzy.top/gtmvdfnigd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sxryk.cn/gtzyrnhpvl.html

PHP:  // 手写时间戳比较
来源：http://hz.hammf.cn/gtgcxiaxxw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtzsxjbfpn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gtsosubmke.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shzxlz.cn/gtzztgbvfb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.52xcode.cn/gtzefbkzyg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pengpengdd.cyou/gtdvikvhju.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.birdmap.top/gtiwsbunog.html

[P08] 处理浮点精度问题
来源：http://hz.meibo888.top/gtxlkfwowl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.birdmap.top/gtxyhkhepu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shanyushiyangkeji.top/gthftzmbbb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.smart0.xyz/gtewpzvjwb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenjidiqi.icu/gtjfspcgav.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhixingplan.top/gtehavmyxu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yanxiufei.cn/gtvfrtziot.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pycfn.com/gtnddhiove.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xuanzx.com/gtkkaaooks.html

================================================================================
来源：http://hz.chenlongwang.top/gtzhxmpzqm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zdqjudy.top/gtpsotwbsp.html

================================================================================
来源：http://hz.xuanzx.com/gtdxqwvrsu.html

[Q01] 创建表
来源：http://hz.tian-w.cn/gtfglhaomw.html

CREATE TABLE users (
来源：http://hz.iojbl.cn/gtletaqeva.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtxlvraxyk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.andypj.xyz/gtjxonlwpz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydzc1.top/gtbeljfhqx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gzhubu.top/gtsqekxcjv.html

);
来源：http://hz.nwbrower.top/gtkkbbunat.html

[Q02] 创建带外键的表
来源：http://hz.nanxinkj.top/gtxqjmvjob.html

CREATE TABLE orders (
来源：http://hz.zhoulong.xyz/gtfchpogid.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gzhubu.top/gtnfwuaxfh.html

user_id INT NOT NULL,
来源：http://hz.0kj1m.cn/gtvdlbnegq.html

amount DECIMAL(10, 2),
来源：http://hz.shzxlz.cn/gtnujklkdp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.smart0.xyz/gtxpyvfszs.html

);
来源：http://hz.jianghu66.top/gtbeqtuxgm.html

[Q03] 增加列
来源：http://hz.hammf.cn/gtokckeqsh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dashuyun.cn/gtzmcltwvj.html

[Q04] 修改列类型
来源：http://hz.yj202588.top/gtyfzmrqwr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinqigufen.top/gtbepzxwcz.html

[Q05] 重命名列
来源：http://hz.smart0.xyz/gtecxnjmnp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yongpay.top/gtjjqjxgxj.html

[Q06] 删除列
来源：http://hz.fengsongda.top/gtbdpklnus.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.vqdsnc.cn/gtbrnpgevw.html

[Q07] 删除表
来源：http://hz.shanyushiyangkeji.top/gtwdgiaoyl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yonumen.top/gtgqmrzxrk.html

[Q08] 创建普通索引
来源：http://hz.zhixingplan.top/gtsmcgmcts.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gtkgqjdvoi.html

[Q09] 创建唯一索引
来源：http://hz.tanke756.top/gtxejputct.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.316326.xyz/gtkvapattb.html

[Q10] 插入单行
来源：http://hz.sweek.top/gtgcerawnm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shzxlz.cn/gtsxffxydb.html

[Q11] 一次插入多行
来源：http://hz.hnxiangtu.top/gtvhvdqdwd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ybcxt.top/gtwagxxtkt.html

[Q12] 插入后取自增 ID
来源：http://hz.shangyingyoupin.top/gtfllkclnj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shangyingyoupin.top/gtjjipabth.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.fengsongda.top/gtnifplkqy.html

[Q13] 忽略重复插入
来源：http://hz.mhx1999.top/gthaxhliuw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.quarkkingdee.top/gturlymzcy.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenjidiqi.icu/gtoxmjhuco.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.daxiang520.top/gtkxqjkwdk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ehwqpu.com/gtjmztgdje.html

[Q15] 查询全部
来源：http://hz.iojbl.cn/gtphvbhfhn.html

SELECT * FROM users;
来源：http://hz.shanyushiyangtech.top/gtbfkfpong.html

[Q16] 查询指定列
来源：http://hz.ybcxt.top/gtgshabfif.html

SELECT id, name FROM users;
来源：http://hz.gaohongyu789.top/gtcezxahxk.html

[Q17] 条件查询
来源：http://hz.yueranfly.top/gtbtrenevg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hnxiangtu.top/gtpqqmbkja.html

[Q18] 模糊匹配
来源：http://hz.yj20258888.top/gtiodkjdjh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xuanzx.com/gtcmfhgtxy.html

[Q19] 范围查询
来源：http://hz.chenzaomai.com/gtmcxeiore.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj202588.top/gtczpmlgpj.html

[Q20] IN 列表
来源：http://hz.sweek.top/gtnuhwdrgi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tanke756.top/gtrrupzuxe.html

[Q21] 空值判断
来源：http://hz.xylfe.cn/gtyogkzgqs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nanxuanxn.top/gtsgrlrtke.html

[Q22] 排序
来源：http://hz.nanxuanxn.top/gtkkzhaigq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gaohongyu789.top/gtyllfrvrj.html

[Q23] 分页
来源：http://hz.chenzaomai.com/gtqgvjpcpz.html


<!-- 参考信息 -->