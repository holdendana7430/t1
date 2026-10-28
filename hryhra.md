代发 wailian999

[N01] 二分查找（有序数组）
来源：http://hz.nwbrower.top/gtxwaztcik.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.redwolf501.top/gtnybhvfws.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gogol.net.cn/gtlnwzanzo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.iojbl.cn/gtosvwksiz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.havefunace.top/gtbdsopzde.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangdashe.top/gtfqkpfdau.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.fengsongda.top/gtthwoqntz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinghuilouyu.cn/gtuvtfptjo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtdtsmgkkl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yanxiufei.cn/gtlciujlvd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gtrtxrdysf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gaohongyu789.top/gtvbiikben.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenzaomai.com/gtvpiyvftv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gtobzlgkel.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cheryme.top/gtxqjaulem.html

Go:   slices.Sort(arr)
来源：http://hz.zhengqikj.top/gtrtgqktkp.html

Ruby: arr.sort
来源：http://hz.c1oappe.top/gtrajnirgk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hammf.cn/gterkxycyb.html

[N03] 快速排序（分治示例）
来源：http://hz.fzhhl.top/gtyjacysxw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fzhhl.top/gtwnydmjkr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhiwuduotai.top/gtxruwoodn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnqzz.top/gtrsydlkhk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jianghu66.top/gtddubquad.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.9152youxi.cn/gtyjybkuke.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ywan-chungtsiang.top/gtytcuoien.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aibaodan.cn/gtfreswhuk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtkrydsyab.html

[N04] 斐波那契数列
来源：http://hz.ybcxt.top/gtlizukwst.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtyjsbrseq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shzxlz.cn/gthxkeiciu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtiuclbvaw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guannengcc.top/gtlzivxwkm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sweek.top/gtvvcyqcjw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ivvv.top/gttfhxfcng.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtyfkunouw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenlongwang.top/gtzfknaiwo.html

[N05] 最大公约数
来源：http://hz.zhaomingkeji.xyz/gtorinlgow.html

Py:   math.gcd(a, b)
来源：http://hz.redwolf501.top/gtwofwrmed.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.vqdsnc.cn/gtwjoiyauo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.mhx1999.top/gtryeclecj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gtikjesvam.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shanyushiyangkeji.top/gthykacqlq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hnxiangtu.top/gttrjnxtcw.html

Ruby: a.gcd(b)
来源：http://hz.quarkkingdee.top/gtejlccqaf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yueranfly.top/gtqiqnjvzj.html

[N06] 判断回文字符串
来源：http://hz.fengsongda.top/gtwnqjoxuj.html

Py:   s == s[::-1]
来源：http://hz.ydzc1.top/gtnhcmonxu.html

PHP:  $s === strrev($s);
来源：http://hz.yongpay.top/gtmhzqmpua.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtvaormwxg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gtdvfelsku.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgufenzy.top/gtabjtuoob.html

Go:   // 双指针从两端比较
来源：http://hz.ppjwa.cn/gteuzwirbn.html

Ruby: s == s.reverse
来源：http://hz.zycfv.cn/gttsusvtrl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gteowrtdgh.html

[N07] 两数之和（返回下标）
来源：http://hz.xylfe.cn/gtvnngcsqw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jianghu66.top/gtxalhimyq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gtvdxsrkzl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhaomingkeji.xyz/gtbchmhywe.html

TS:   // 手写 Map<string, number>
来源：http://hz.redwolf501.top/gtqcqsbriv.html

Java: // 手写 HashMap
来源：http://hz.pengpengdd.cyou/gtqngllnpg.html

Go:   // 手写 map[int]int
来源：http://hz.sweek.top/gtdrrktxxr.html

Ruby: // 手写 Hash
来源：http://hz.yvedp.cn/gtxnszrsed.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ywan-chungtsiang.top/gtqhyhtngy.html

[N08] 生成全排列
来源：http://hz.haohaochexian.top/gtkhbclmqu.html

Py:   itertools.permutations(arr)
来源：http://hz.jiagoushi.top/gtqmlzxyqg.html

PHP:  // 手写递归交换
来源：http://hz.cheryme.top/gtlljljyfj.html

JS:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtybdxjjyf.html

TS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtqpclnzxj.html

Java: // 手写回溯递归
来源：http://hz.zhixingplan.top/gtdbwiavpi.html

Go:   // 手写回溯递归
来源：http://hz.pycfn.com/gttobxmlem.html

Ruby: arr.permutation.to_a
来源：http://hz.ybcxt.top/gtnovgtdol.html

C#:   // 手写回溯递归
来源：http://hz.ivvv.top/gtyktpsqnj.html

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gtbiocdqns.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shuidangran.top/gtslshnkmf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ppjwa.cn/gtodwyrafz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ybcxt.top/gthfqbjhue.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhaomingkeji.xyz/gtvkxfozeq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.svipenyu.cn/gtzmbgnhbs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jlsjyb.cn/gtelieeqqc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.birdmap.top/gtwtzvkkpm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gogol.net.cn/gtwvivgzac.html

[N10] 链表节点定义
来源：http://hz.ydzc1.top/gtmcxrmzjg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.redwolf501.top/gteccmaevy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nanxuanxn.top/gtkywtkbqb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xylfe.cn/gtirzpuvzw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pycfn.com/gthjjmissn.html

Java: class Node { int v; Node next; }
来源：http://hz.hnqzz.top/gtujtngtbm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.fengsongda.top/gtxjmtbdme.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shuidangran.top/gttumxvkjj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.meibo888.top/gtclhexedn.html

[N11] 二叉树中序遍历
来源：http://hz.xuanzx.com/gtedyhmrne.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yangfankeji.com/gtmxjdmvra.html

PHP:  // 手写递归函数
来源：http://hz.yangfankeji.com/gtgdeyyhob.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtoymaftxr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtmqfnnbme.html

Java: // 手写递归
来源：http://hz.xinyue.icu/gtwonybpjz.html

Go:   // 手写递归
来源：http://hz.zhixingplan.top/gtkpshksdx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yangfankeji.com/gtwetpmvoi.html

C#:   // 手写递归
来源：http://hz.chenlongwang.top/gtxwchrepa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhixingplan.top/gtqusvtmga.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.birdmap.top/gtvwgpqtzu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cqqwz.cn/gthveokdtc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cheryme.top/gtwgaftwzm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtlqjacsqb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtssfovhvb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.meibo888.top/gtqzvlnbug.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenlongwang.top/gtbudcrdgm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtzvxhxiud.html

================================================================================
来源：http://hz.hnxiangtu.top/gtojaqxzrd.html

O. 并发与异步
来源：http://hz.xuanzx.com/gtxfdarswh.html

================================================================================
来源：http://hz.ehwqpu.com/gtlnfgvpel.html

[O01] 启动一个线程
来源：http://hz.ppjwa.cn/gtjrufwzwo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.haohaochexian.top/gtlyamwamb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yj20258888.top/gtnzftrmmx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gotoacloud.top/gtawcpovpi.html

TS:   // 同 JS
来源：http://hz.zhongyouzk.top/gtujgreoqc.html

Java: new Thread(() -> f()).start()
来源：http://hz.jqgufenzy.top/gtqtfoygxq.html

Go:   go f()
来源：http://hz.andypj.xyz/gtarhzvfef.html

Ruby: Thread.new { f }
来源：http://hz.fengsongda.top/gtehmvojpa.html

C#:   Task.Run(() => F());
来源：http://hz.zdqjudy.top/gteampmzgc.html

[O02] 使用线程池
来源：http://hz.shzxlz.cn/gtuvkmshzs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hywenlv.cn/gtsulckyqt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhijiandao.cn/gtyrwlurkr.html

JS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtyagjimjk.html

TS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtlorftvsj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenlongwang.top/gtnfxbsfnc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jqgufenzy.top/gtcjldnfiu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hammf.cn/gttjxulwvb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.aibaodan.cn/gtyvrwpljz.html

[O03] 加锁保护共享数据
来源：http://hz.xziqi.cn/gtvcnbirvu.html

Py:   with lock: shared += 1
来源：http://hz.zycfv.cn/gtaqqjmfxb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.redwolf501.top/gtdajepqzn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tanke756.top/gttmaulltv.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtunblxvlp.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuxming.cn/gtelpuchzu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gogol.net.cn/gtvesyssae.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dianchejie.cn/gtdtfqttht.html

C#:   lock (gate) { shared++; }
来源：http://hz.pengpengdd.cyou/gtqxcjghjl.html

[O04] 定义异步函数并等待
来源：http://hz.wangdashe.top/gtzbkvmpdf.html

Py:   async def f():⏎    await g()
来源：http://hz.gogol.net.cn/gtcwdwkzpk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shangyingyoupin.top/gtyhdpfldp.html

JS:   async function f() { await g(); }
来源：http://hz.sysykeji.top/gtmnyydrap.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cucudq.cn/gtqxbbbwgp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jlsjyb.cn/gtrnrxbhvw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.fengsongda.top/gtioxsiqth.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenlongwang.top/gtonqsmhzf.html

C#:   async Task F() { await G(); }
来源：http://hz.guowangkeji.top/gtgwgrpcsm.html

[O05] 并发执行并等待全部完成
来源：http://hz.mhx1999.top/gtwvnymooq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yonumen.top/gtuweahdtz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.havefunace.top/gtybahmntw.html

JS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtxtcgzfqx.html

TS:   await Promise.all(tasks)
来源：http://hz.zhiwuduotai.top/gtdkhsbmbe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tian-w.cn/gteclhrhrt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hongshengwenyu.top/gtlcwhawoe.html

Ruby: threads.map(&:join)
来源：http://hz.316326.xyz/gtotckpmsn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.daxiang520.top/gtzdawxmal.html

[O06] 使用进程池
来源：http://hz.yvedp.cn/gtgzummyog.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangshuangyany.cn/gtsereazek.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.guowangkeji.top/gtfljrqxyr.html

JS:   // child_process / cluster 模块
来源：http://hz.hfpthk.cn/gtgukcufpc.html

TS:   // child_process / cluster 模块
来源：http://hz.hysaishi.cn/gtxnytrrbk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtwwiwxnou.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shangyingyoupin.top/gtmeywfhow.html

Ruby: // fork 块
来源：http://hz.zycfv.cn/gtjzmuxmov.html

C#:   Parallel.For
来源：http://hz.andypj.xyz/gtjulfrywt.html

================================================================================
来源：http://hz.ydjk.org.cn/gtnskdjiag.html

P. 常用工具函数
来源：http://hz.ppjwa.cn/gtndzofncu.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtsrrurhqq.html

[P01] 生成 UUID
来源：http://hz.jqgfzy.top/gtoqgvlsii.html

Py:   str(uuid.uuid4())
来源：http://hz.gzhubu.top/gterwxdfzg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.birdmap.top/gtnzwsjtmq.html

JS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtuuutkgxe.html

TS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtwwxdbbdv.html

Java: UUID.randomUUID().toString()
来源：http://hz.xingfuxueyuan.xyz/gtzbdqfsjn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ywan-chungtsiang.top/gtdpvovvlr.html

Ruby: SecureRandom.uuid
来源：http://hz.meibo888.top/gtldaedsxb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dashuyun.cn/gtnnclkjsi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhixingplan.top/gtbubjmqgk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pycfn.com/gtcnohwmjw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.vqdsnc.cn/gtyrmeeijl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhijiandao.cn/gtdxelgepw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenzaomai.com/gtxotscxdo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.svipenyu.cn/gttxgxrzbd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydzc1.top/gtwnerqsxd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ppjwa.cn/gttllnjssa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sxryk.cn/gtcpdgmttk.html

[P03] 生成短随机字符串
来源：http://hz.zhoulong.xyz/gtfgmstgbd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jiagoushi.top/gtiocubnul.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuetiantiany.cn/gtiuqiyput.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sweek.top/gtfzfvpgnh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cdnleiting.top/gtojryhhpf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jiagoushi.top/gtlpucijko.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cucudq.cn/gtdgtvhepe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhoulong.xyz/gtvrzxzakv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhoulong.xyz/gtpprauqor.html

[P04] 求长度
来源：http://hz.9152youxi.cn/gthjgcafeh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daxiang520.top/gtodlmqfwd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtphvlreji.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxuanxn.top/gtustpcygi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenzaomai.com/gtyckttigi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.52xcode.cn/gtxunkcuhe.html

Go:   len(arr);  len(m)
来源：http://hz.snrcjt.cn/gtsvndhhlq.html

Ruby: x.length;  x.size
来源：http://hz.shzxlz.cn/gtqtnhibuy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yueranfly.top/gtvnfdrynb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangtech.top/gtycthzjnp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.aizwys.cn/gtsykhqkox.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ppjwa.cn/gtsofvpvqn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.quarkkingdee.top/gtpbdxmnap.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pycfn.com/gtcayhztkz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.snrcjt.cn/gtrpnsrlpl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.redwolf501.top/gtxvurohwi.html

Ruby: a == b
来源：http://hz.xingfuxueyuan.xyz/gtfujafmon.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhixingplan.top/gtlknqeuhz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tianlin.xyz/gtjmmcmsoy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.dashuyun.cn/gtqakzmpha.html

PHP:  if (empty($x)) {}
来源：http://hz.ydzc1.top/gtonbqiibz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zdqjudy.top/gtlqrxztwr.html

TS:   if (x == null) {}
来源：http://hz.smart0.xyz/gtapywvhxi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hfpthk.cn/gtthjfimey.html

Go:   if x == nil {}
来源：http://hz.nanxinkj.top/gtouxgfohv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.feifeiyinyue.top/gtvkesidey.html

C#:   if (x is null) {}
来源：http://hz.ybcxt.top/gtllgspphj.html

[P07] 防抖与节流
来源：http://hz.kuanghao11.cn/gtbyjwsyeb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fengsongda.top/gtblutcuws.html

PHP:  // 手写时间戳比较
来源：http://hz.birdmap.top/gtblddhtsp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gthcvjrwrt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtcgitpdol.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sxryk.cn/gtawbujopw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ydzc1.top/gtmrxjopyp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hysaishi.cn/gtbejpcuzj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xziqi.cn/gtitzlsxxm.html

[P08] 处理浮点精度问题
来源：http://hz.gaohongyu789.top/gtwumoxotz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ivvv.top/gthufdmheo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yongpay.top/gtercvuepd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.redwolf501.top/gtuplpcyno.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.mhx1999.top/gtbugdixsk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tianlin.xyz/gtdlbxkxhs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shzxlz.cn/gtinmoserh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gtzabpeojq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shuidangran.top/gtcrkxrzay.html

================================================================================
来源：http://hz.ydzc1.top/gtfwqnphmz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.smart0.xyz/gtwfvtxwsx.html

================================================================================
来源：http://hz.cashguo.top/gtvfgmhqfv.html

[Q01] 创建表
来源：http://hz.haohaochexian.top/gtetmcheoq.html

CREATE TABLE users (
来源：http://hz.gogol.net.cn/gtlwjhwsfo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenzaomai.com/gtyolqzlwq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.andypj.xyz/gtiamxtmmd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gaohongyu789.top/gtxetdokhi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.9152youxi.cn/gtoeeczbyr.html

);
来源：http://hz.andypj.xyz/gtomzvsejy.html

[Q02] 创建带外键的表
来源：http://hz.jlsjyb.cn/gtttqmzlcq.html

CREATE TABLE orders (
来源：http://hz.ydzc1.top/gtrhqkxroy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hammf.cn/gtjxgzlzpr.html

user_id INT NOT NULL,
来源：http://hz.chenzaomai.com/gthbskimyb.html

amount DECIMAL(10, 2),
来源：http://hz.yuxming.cn/gtvldtrqof.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hywenlv.cn/gtlujhjhox.html

);
来源：http://hz.zhixingplan.top/gtutejgekb.html

[Q03] 增加列
来源：http://hz.hnxiangtu.top/gtruguggqr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tanke756.top/gtvsxcupba.html

[Q04] 修改列类型
来源：http://hz.c1oappe.top/gtlldhifyt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yongpay.top/gtnikcqcgm.html

[Q05] 重命名列
来源：http://hz.tianlin.xyz/gtztnpqrdd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gotoacloud.top/gtziiizcir.html

[Q06] 删除列
来源：http://hz.shanyushiyangtech.top/gtxgvpaidz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.iojbl.cn/gthtbcazoj.html

[Q07] 删除表
来源：http://hz.ivvv.top/gtcnmvrohr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.kuanghao11.cn/gtocwahgnk.html

[Q08] 创建普通索引
来源：http://hz.shanyushiyangtech.top/gttssuxdqg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtwptggthx.html

[Q09] 创建唯一索引
来源：http://hz.ppjwa.cn/gtzelyrpkh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ehwqpu.com/gtokfdszuk.html

[Q10] 插入单行
来源：http://hz.daria6918.cn/gtjwiqijgj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhiwuduotai.top/gtddezgste.html

[Q11] 一次插入多行
来源：http://hz.yuxming.cn/gtjndwumro.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tianlin.xyz/gtucihmunp.html

[Q12] 插入后取自增 ID
来源：http://hz.zhengqikj.top/gtgzpsrjpv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.vqdsnc.cn/gttlrzwhyg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daria6918.cn/gtmkstxclt.html

[Q13] 忽略重复插入
来源：http://hz.zhongyouzk.top/gtwurjtsog.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinyuanbaomall.cn/gtdjqiajzx.html

[Q14] 存在则更新（upsert）
来源：http://hz.52xcode.cn/gtukpxiarr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258888.top/gtimcheqxu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuanzx.com/gtmczhtrev.html

[Q15] 查询全部
来源：http://hz.tian-w.cn/gtuvwrgfef.html

SELECT * FROM users;
来源：http://hz.jinqigfzy.top/gtqmhfydmy.html

[Q16] 查询指定列
来源：http://hz.sufxvd.cn/gttuyjyiph.html

SELECT id, name FROM users;
来源：http://hz.zhijiandao.cn/gtezpgnpjq.html

[Q17] 条件查询
来源：http://hz.vqdsnc.cn/gtmrieooje.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hfpthk.cn/gtheexptov.html

[Q18] 模糊匹配
来源：http://hz.jiagoushi.top/gtluqqkvyl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hfpthk.cn/gtvkjpbdga.html

[Q19] 范围查询
来源：http://hz.nanxinkj.top/gtehnbztmz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yonumen.top/gtarluprkz.html

[Q20] IN 列表
来源：http://hz.ydjk.org.cn/gtuqjwztre.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yongpay.top/gttvhbbopr.html

[Q21] 空值判断
来源：http://hz.sxryk.cn/gtyvgilcnl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenjidiqi.icu/gtpuieiwit.html

[Q22] 排序
来源：http://hz.hammf.cn/gtlosywdoq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cqqwz.cn/gtrqecijux.html

[Q23] 分页
来源：http://hz.shuidangran.top/gtzezajfek.html


<!-- 参考信息 -->