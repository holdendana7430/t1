代发 wailian999

[N01] 二分查找（有序数组）
来源：http://hz.sysykeji.top/gtpuksfuih.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnxiangtu.top/gtjkvmotat.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxinkj.top/gtoeigqbsk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhaomingkeji.xyz/gtjnvuqxpu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.andypj.xyz/gtikwnpojz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtqfjvafnr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangdashe.top/gtcvtbbjhx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.vqdsnc.cn/gtlolazzre.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.svipenyu.cn/gtbodnjppz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yanxiufei.cn/gtxoutikgv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gtnktgyfry.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fengsongda.top/gtujxdeajh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxuanxn.top/gtmcwjpmqx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtumptcfny.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cashguo.top/gtmohteyrx.html

Go:   slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtwfahiyzq.html

Ruby: arr.sort
来源：http://hz.tian-w.cn/gtfmyzapfw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj20258888.top/gtexcnarsn.html

[N03] 快速排序（分治示例）
来源：http://hz.ppjwa.cn/gtdsdqdolb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cashguo.top/gtrgzkjeda.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hongshengwenyu.top/gtpetiwzmw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gtsmphnnzy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gteduvpabk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xuanzx.com/gtnsyoppje.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tanke756.top/gttqcdchsj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yongpay.top/gthxvpgdiy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xinyue.icu/gteqiuomnp.html

[N04] 斐波那契数列
来源：http://hz.jqgfzy.top/gtzfzbrill.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jyoumei.cn/gtlgwoynwx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.smart0.xyz/gtejmrqajs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.vqdsnc.cn/gtdyltuqai.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtfrmqqbyp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.pengpengdd.cyou/gtmpdvigzp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigfzy.top/gtmisoneqw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtcomtgaxe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.guowangkeji.top/gtcfoehmed.html

[N05] 最大公约数
来源：http://hz.yj20258888.top/gtvksbnpam.html

Py:   math.gcd(a, b)
来源：http://hz.dashuyun.cn/gthpjqyhoi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.316326.xyz/gttkeubbjl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.haohaochexian.top/gtvvjxguwn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guowangkeji.top/gtcssxzchm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydjk.org.cn/gtlnocmavv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.iojbl.cn/gthyjfpgci.html

Ruby: a.gcd(b)
来源：http://hz.cdnleiting.top/gthqtqcyow.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yongpay.top/gtfpdlpwee.html

[N06] 判断回文字符串
来源：http://hz.cashguo.top/gtneyogcfe.html

Py:   s == s[::-1]
来源：http://hz.jqgufenzy.top/gtpvufidit.html

PHP:  $s === strrev($s);
来源：http://hz.ydzc1.top/gtabxzhfwo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtrmnmhhql.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtoypqtisz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhixingplan.top/gtgkzflimj.html

Go:   // 双指针从两端比较
来源：http://hz.shangyingyoupin.top/gtijumajnv.html

Ruby: s == s.reverse
来源：http://hz.xuetiantiany.cn/gtzfezuute.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yonumen.top/gtozvzjgxn.html

[N07] 两数之和（返回下标）
来源：http://hz.jyoumei.cn/gthpzmpeke.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.iojbl.cn/gtssmsnsmw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenlongwang.top/gtmzdruhcw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yvedp.cn/gtorvtdehv.html

TS:   // 手写 Map<string, number>
来源：http://hz.yongpay.top/gtavayeyqx.html

Java: // 手写 HashMap
来源：http://hz.iojbl.cn/gtdntahaoa.html

Go:   // 手写 map[int]int
来源：http://hz.ydzc1.top/gtdtzzertj.html

Ruby: // 手写 Hash
来源：http://hz.gaohongyu789.top/gtdwllrtic.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj20258888.top/gtrwcjklxm.html

[N08] 生成全排列
来源：http://hz.hysaishi.cn/gteoibrzsa.html

Py:   itertools.permutations(arr)
来源：http://hz.gzhubu.top/gtsgoyvnyp.html

PHP:  // 手写递归交换
来源：http://hz.zycfv.cn/gtfwgqewyq.html

JS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtzevrmvhj.html

TS:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtjmdvknko.html

Java: // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtqyrgmckv.html

Go:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtgqugzaob.html

Ruby: arr.permutation.to_a
来源：http://hz.cdnleiting.top/gtvxobtkze.html

C#:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtgfkdzopo.html

[N09] 栈与队列
来源：http://hz.jinyuanbaomall.cn/gtgpfzowst.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shangyingyoupin.top/gtbalvxipt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yonumen.top/gtksnmixgq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuxming.cn/gtrmoevkgj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hnxiangtu.top/gtgwwdnnrg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yueranfly.top/gttfhkawwm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhoulong.xyz/gtsmgfhvtn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nanxuanxn.top/gttjtgrxyx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sufxvd.cn/gtcneknpeb.html

[N10] 链表节点定义
来源：http://hz.mhx1999.top/gtsrsksyof.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hysaishi.cn/gtmbvdxejg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jlsjyb.cn/gthyrnvntd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.quarkkingdee.top/gtpngbtszj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ydzc1.top/gtzusazjbw.html

Java: class Node { int v; Node next; }
来源：http://hz.sxryk.cn/gttddjecgj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinyuanbaomall.cn/gtkyanskmt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.daxiang520.top/gtwoptwwhu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.wangshuangyany.cn/gtdhvanpqs.html

[N11] 二叉树中序遍历
来源：http://hz.xylfe.cn/gtrwlrtqhi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hongshengwenyu.top/gtlquqsonp.html

PHP:  // 手写递归函数
来源：http://hz.jqgfzy.top/gtsshespre.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtmncbetri.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydjk.org.cn/gtjegkxtwh.html

Java: // 手写递归
来源：http://hz.chenzaomai.com/gtwzvvliea.html

Go:   // 手写递归
来源：http://hz.gogol.net.cn/gtnfkxdacd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cqqwz.cn/gtrjvelvmw.html

C#:   // 手写递归
来源：http://hz.hywenlv.cn/gtbiiygvkj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shuidangran.top/gtkwkhxaou.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.feifeiyinyue.top/gtujvbegth.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jianghu66.top/gtreawmrrm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.quarkkingdee.top/gtiuthdvev.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gzhubu.top/gtuophzuqr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aibaodan.cn/gtuqkqfgzf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.c1oappe.top/gtvhycepte.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.guowangkeji.top/gtnwmzujad.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtfxnfvhyk.html

================================================================================
来源：http://hz.cucudq.cn/gtgzeapbon.html

O. 并发与异步
来源：http://hz.yonumen.top/gtevpiruxw.html

================================================================================
来源：http://hz.quarkkingdee.top/gtzmbufxum.html

[O01] 启动一个线程
来源：http://hz.dashuyun.cn/gtkbjhhsyj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gaohongyu789.top/gtwpdehunf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.dashuyun.cn/gtzcuspznl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hywenlv.cn/gtvbxvxajn.html

TS:   // 同 JS
来源：http://hz.sweek.top/gtjilfbyjb.html

Java: new Thread(() -> f()).start()
来源：http://hz.guannengcc.top/gtgigrzfgk.html

Go:   go f()
来源：http://hz.tian-w.cn/gtisseyteh.html

Ruby: Thread.new { f }
来源：http://hz.jqgfzy.top/gtsdxjnbkk.html

C#:   Task.Run(() => F());
来源：http://hz.hfpthk.cn/gtslypovux.html

[O02] 使用线程池
来源：http://hz.zdqjudy.top/gtflzwihlq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.feifeiyinyue.top/gtxydrohul.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxuanxn.top/gtxxwfmcki.html

JS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gtqwcrmfbh.html

TS:   // worker_threads 线程池
来源：http://hz.nanxinkj.top/gtepobrvvn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhixingplan.top/gtgfpptbdj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhiwuduotai.top/gthhddgwmf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinyuanbaomall.cn/gtppngczzd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gaohongyu789.top/gtjfkfivxw.html

[O03] 加锁保护共享数据
来源：http://hz.ydjk.org.cn/gtcogntzmp.html

Py:   with lock: shared += 1
来源：http://hz.yonumen.top/gtzjgfxsus.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhiwuduotai.top/gtvigculrb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nwbrower.top/gtmbvnauus.html

TS:   // 同 JS
来源：http://hz.jqgufenzy.top/gtseatjvdw.html

Java: synchronized (this) { shared++; }
来源：http://hz.gaohongyu789.top/gthquyecwu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuanzx.com/gtuipcktxh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.feifeiyinyue.top/gtzbjtbbhg.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinyuanbaomall.cn/gthfzmqdpi.html

[O04] 定义异步函数并等待
来源：http://hz.zycfv.cn/gtqvhynifw.html

Py:   async def f():⏎    await g()
来源：http://hz.yvedp.cn/gtpswludyw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sweek.top/gtexaxreyu.html

JS:   async function f() { await g(); }
来源：http://hz.jinyuanbaomall.cn/gtykdupqnh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dianchejie.cn/gttemfwbjj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guowangkeji.top/gttkjdqhrx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.aibaodan.cn/gtxdpjkigm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.snrcjt.cn/gtcutrkozq.html

C#:   async Task F() { await G(); }
来源：http://hz.ywan-chungtsiang.top/gtszjotveh.html

[O05] 并发执行并等待全部完成
来源：http://hz.316326.xyz/gtskacgaoh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuanzhike.top/gtjorrqgec.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.haohaochexian.top/gtnrpxwxem.html

JS:   await Promise.all(tasks)
来源：http://hz.daxiang520.top/gtyxwpetts.html

TS:   await Promise.all(tasks)
来源：http://hz.nanxinkj.top/gtysmkqkon.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhengqikj.top/gtrhluccxi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhijiandao.cn/gthrlomoqx.html

Ruby: threads.map(&:join)
来源：http://hz.bjfxy.top/gtxzccaxkg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangshuangyany.cn/gtknllgueg.html

[O06] 使用进程池
来源：http://hz.zhongyouzk.top/gtvnxxctkn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hongshengwenyu.top/gtkgiwvlzn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hywenlv.cn/gtlbdjisgm.html

JS:   // child_process / cluster 模块
来源：http://hz.zhengqikj.top/gtxioymazd.html

TS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gtfgvqbbqa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhongyouzk.top/gtqiqopbua.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hywenlv.cn/gtnvmactoz.html

Ruby: // fork 块
来源：http://hz.meibo888.top/gtvgeixnwi.html

C#:   Parallel.For
来源：http://hz.zhiwuduotai.top/gtwcntwulg.html

================================================================================
来源：http://hz.jlsjyb.cn/gtdtzuiqhx.html

P. 常用工具函数
来源：http://hz.daria6918.cn/gtnjxjcliu.html

================================================================================
来源：http://hz.yangfankeji.com/gtssokazgq.html

[P01] 生成 UUID
来源：http://hz.zdqjudy.top/gtfmchspbp.html

Py:   str(uuid.uuid4())
来源：http://hz.snrcjt.cn/gtasjrmqew.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgufenzy.top/gtdtqgrdah.html

JS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtvgehctdk.html

TS:   crypto.randomUUID()
来源：http://hz.cashguo.top/gtkuvzujqw.html

Java: UUID.randomUUID().toString()
来源：http://hz.ybcxt.top/gtcqvqnvlb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gotoacloud.top/gttmziakml.html

Ruby: SecureRandom.uuid
来源：http://hz.haohaochexian.top/gtvmgexkej.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.pengpengdd.cyou/gtwmettslg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.vqdsnc.cn/gtxawdbrlw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cucudq.cn/gtnclqczay.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gaohongyu789.top/gtnpdmunxa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xziqi.cn/gtjmltmlky.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hysaishi.cn/gtsgksibbj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinyuanbaomall.cn/gthhccbeov.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jqgufenzy.top/gtlhzaqauk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sysykeji.top/gtmmkxxijy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fzhhl.top/gtffzuvyqe.html

[P03] 生成短随机字符串
来源：http://hz.sweek.top/gtkezgqkpx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtjcljdhfr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj20258.top/gtyrosmvxo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhoulong.xyz/gtikcvukzb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenlongwang.top/gtthazgmbf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.daria6918.cn/gtdeoalnbx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.meibo888.top/gtjsibtzrc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgufenzy.top/gtshgpprko.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigufen.top/gtkyjznrtt.html

[P04] 求长度
来源：http://hz.ydjk.org.cn/gtcnuywcwl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.pengpengdd.cyou/gtpxjxcxbv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gtmfkxyzeq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtzmntqjar.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtmfztsyra.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gogol.net.cn/gtcghedfzo.html

Go:   len(arr);  len(m)
来源：http://hz.zdqjudy.top/gtbyfgpqqk.html

Ruby: x.length;  x.size
来源：http://hz.ehwqpu.com/gtjcbjwffz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xinyue.icu/gtctszbkyf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuetiantiany.cn/gtbnuagldu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sweek.top/gttphaipcg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.smart0.xyz/gtkdlsxvkv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guannengcc.top/gtcsibkouc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hnqzz.top/gtxmmbzokh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jlsjyb.cn/gtimtpcklq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxinkj.top/gtuuoiweeg.html

Ruby: a == b
来源：http://hz.zycfv.cn/gtnqhvrppg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yuanzhike.top/gtwlvcmwib.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fengsongda.top/gtrwtwdrmq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj20258888.top/gtcfhfpqtt.html

PHP:  if (empty($x)) {}
来源：http://hz.zhengqikj.top/gtmnoghksu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jyoumei.cn/gttvzzdjja.html

TS:   if (x == null) {}
来源：http://hz.yj20258888.top/gtxbikanbz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnqzz.top/gtcajhyivn.html

Go:   if x == nil {}
来源：http://hz.xziqi.cn/gtercmuwul.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydjk.org.cn/gtryhbqyvf.html

C#:   if (x is null) {}
来源：http://hz.fengsongda.top/gtlqeqfmng.html

[P07] 防抖与节流
来源：http://hz.zhiwuduotai.top/gtkvktcebc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinqigfzy.top/gttosfsqfj.html

PHP:  // 手写时间戳比较
来源：http://hz.52xcode.cn/gtaxvwzbxw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtwnmwrqen.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtjoitpjwr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tian-w.cn/gthvqzziku.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhixingplan.top/gtuzfliajf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.mhx1999.top/gtguwiqbab.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.vqdsnc.cn/gtlarhqhsr.html

[P08] 处理浮点精度问题
来源：http://hz.snrcjt.cn/gtwugkglos.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pycfn.com/gtfjwnftms.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.guowangkeji.top/gtdhsmyuun.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.0kj1m.cn/gtlfgebuep.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.mhx1999.top/gtcggiuzxk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuxming.cn/gtlgpbkvmo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhijiandao.cn/gtgeknpiot.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhiwuduotai.top/gttaqmpijt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gotoacloud.top/gtwattfjoo.html

================================================================================
来源：http://hz.birdmap.top/gtdtiwpbob.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.haohaochexian.top/gtskldjubf.html

================================================================================
来源：http://hz.haohaochexian.top/gtsmfhvmiq.html

[Q01] 创建表
来源：http://hz.shuidangran.top/gtqdmxllkp.html

CREATE TABLE users (
来源：http://hz.yj20258888.top/gtegtffgae.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtsbpncxfu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gaohongyu789.top/gtufsjpung.html

email VARCHAR(100) UNIQUE,
来源：http://hz.quarkkingdee.top/gtdcvxjfni.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.meibo888.top/gtulviujxw.html

);
来源：http://hz.wangshuangyany.cn/gtxznbqpgu.html

[Q02] 创建带外键的表
来源：http://hz.shuidangran.top/gtwhkugfhw.html

CREATE TABLE orders (
来源：http://hz.shuidangran.top/gtynhyacfi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtuimfkzjf.html

user_id INT NOT NULL,
来源：http://hz.hfpthk.cn/gtcbxbnptx.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258.top/gtcxkkdelw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.daria6918.cn/gtgvjqbvmf.html

);
来源：http://hz.fzhhl.top/gthbozxxer.html

[Q03] 增加列
来源：http://hz.yj20258.top/gtvmxvsujg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.haohaochexian.top/gtejqkaitg.html

[Q04] 修改列类型
来源：http://hz.jqgufenzy.top/gtqsldzvux.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhengqikj.top/gtlatrblxm.html

[Q05] 重命名列
来源：http://hz.hammf.cn/gtseghfyju.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhengqikj.top/gtcrdqhhhq.html

[Q06] 删除列
来源：http://hz.zhijiandao.cn/gtwitysslf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.tanke756.top/gtethyryuc.html

[Q07] 删除表
来源：http://hz.yangfankeji.com/gtxpeqgzsc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.feifeiyinyue.top/gtdryfapvf.html

[Q08] 创建普通索引
来源：http://hz.hywenlv.cn/gtvpeepriw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.daria6918.cn/gtnhcnqkay.html

[Q09] 创建唯一索引
来源：http://hz.pycfn.com/gtxehamkao.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fzhhl.top/gtvbpipsle.html

[Q10] 插入单行
来源：http://hz.yvedp.cn/gtwbkoujux.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangkeji.top/gtriwkiddf.html

[Q11] 一次插入多行
来源：http://hz.zhixingplan.top/gtodjfyegb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cashguo.top/gtezdkhrbx.html

[Q12] 插入后取自增 ID
来源：http://hz.jlsjyb.cn/gtrilvmjjt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnxiangtu.top/gtykolfjpw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nanxinkj.top/gtqhwgasea.html

[Q13] 忽略重复插入
来源：http://hz.hfpthk.cn/gtafuybifz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yangfankeji.com/gtambnfadh.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangkeji.top/gtsueejmdb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zdqjudy.top/gtumjpyuzn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hongshengwenyu.top/gtzttzqzrq.html

[Q15] 查询全部
来源：http://hz.316326.xyz/gtqslkbczg.html

SELECT * FROM users;
来源：http://hz.zhiwuduotai.top/gtxrcyaghb.html

[Q16] 查询指定列
来源：http://hz.yongpay.top/gtiahbvacl.html

SELECT id, name FROM users;
来源：http://hz.redwolf501.top/gtysuroavr.html

[Q17] 条件查询
来源：http://hz.guannengcc.top/gtqbrchgmw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shuidangran.top/gtyymwazap.html

[Q18] 模糊匹配
来源：http://hz.aizwys.cn/gtqujcmnan.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.birdmap.top/gtpzqbyowp.html

[Q19] 范围查询
来源：http://hz.yvedp.cn/gtuoozavov.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hysaishi.cn/gtlktjnpob.html

[Q20] IN 列表
来源：http://hz.chenzaomai.com/gtxbofstzu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hywenlv.cn/gtltwdzpkd.html

[Q21] 空值判断
来源：http://hz.jqgfzy.top/gtplywnmrt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shzxlz.cn/gtuedbdqay.html

[Q22] 排序
来源：http://hz.jiagoushi.top/gtsqsgjntt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shuidangran.top/gturprgjod.html

[Q23] 分页
来源：http://hz.chenzaomai.com/gtkifnmqya.html


<!-- 参考信息 -->