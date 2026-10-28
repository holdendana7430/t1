代发 wailian999

[N01] 二分查找（有序数组）
来源：http://hz.xingfuxueyuan.xyz/gtznsdonjk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtqlngfcnw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hywenlv.cn/gtnrkxzjvs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtmeoocxtn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangtech.top/gthdhkbgkm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnxiangtu.top/gtopuljokr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigfzy.top/gtepmgywfk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigfzy.top/gtelagzirh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.daxiang520.top/gtfwgiexxm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jyoumei.cn/gtdupguhpn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.0kj1m.cn/gtuzklwmce.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xinyue.icu/gtpgxregte.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gthqfdgpdu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtpgjllqwh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenjidiqi.icu/gtdmerkbsq.html

Go:   slices.Sort(arr)
来源：http://hz.xinyue.icu/gtwfmuxsih.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtygqkhbte.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.redwolf501.top/gtjyfpdsqo.html

[N03] 快速排序（分治示例）
来源：http://hz.zhaomingkeji.xyz/gtofszoxhv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hfpthk.cn/gtplsccoek.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhijiandao.cn/gtdsejyfhg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gtehblmjcu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sxryk.cn/gtsoaojnwz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ydjk.org.cn/gtjenzadrq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.kuanghao11.cn/gtjinjqnte.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.wangdashe.top/gtbqdawsav.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtrxpkburb.html

[N04] 斐波那契数列
来源：http://hz.yj202588.top/gtxbeidkmf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtudqezvpm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.daria6918.cn/gtqnhvgigb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.bjfxy.top/gtuxawswnl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gaohongyu789.top/gtxeqiigfi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ehwqpu.com/gtrajjuffr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tian-w.cn/gtzkapazfe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gtueiwyhog.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sufxvd.cn/gtoqpumwlm.html

[N05] 最大公约数
来源：http://hz.zhongyouzk.top/gtptrquyqv.html

Py:   math.gcd(a, b)
来源：http://hz.jinyuanbaomall.cn/gtcljdeaol.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tianlin.xyz/gtljwjcmkf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtrrszegsc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtgguuwdnw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gzhubu.top/gtcsxloeoa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ivvv.top/gtioosccpc.html

Ruby: a.gcd(b)
来源：http://hz.shanyushiyangtech.top/gtqqocuqjr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zycfv.cn/gtqcauvkat.html

[N06] 判断回文字符串
来源：http://hz.ivvv.top/gtulzatlai.html

Py:   s == s[::-1]
来源：http://hz.c1oappe.top/gtaoypakrx.html

PHP:  $s === strrev($s);
来源：http://hz.snrcjt.cn/gtjotixkbm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtrsqxxvow.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtbaemaemg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.haohaochexian.top/gtqzzimjdr.html

Go:   // 双指针从两端比较
来源：http://hz.gaohongyu789.top/gtsoherhdb.html

Ruby: s == s.reverse
来源：http://hz.aizwys.cn/gtyijrmykw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtxwzzqkhp.html

[N07] 两数之和（返回下标）
来源：http://hz.zhiwuduotai.top/gtvythdaif.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pengpengdd.cyou/gtcrpcvgjr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yanxiufei.cn/gtibcvnbcp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fzhhl.top/gtrjdbrvbk.html

TS:   // 手写 Map<string, number>
来源：http://hz.aibaodan.cn/gtehndkrfl.html

Java: // 手写 HashMap
来源：http://hz.yanxiufei.cn/gthazcdxgs.html

Go:   // 手写 map[int]int
来源：http://hz.kuanghao11.cn/gtultljhfj.html

Ruby: // 手写 Hash
来源：http://hz.zhijiandao.cn/gtwhonpnqx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnqzz.top/gtpzijxigs.html

[N08] 生成全排列
来源：http://hz.pycfn.com/gtzvcgxiuo.html

Py:   itertools.permutations(arr)
来源：http://hz.cucudq.cn/gtvxdhvync.html

PHP:  // 手写递归交换
来源：http://hz.gotoacloud.top/gtfuvnsfbq.html

JS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gthwnmyjdw.html

TS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtfaxowgeq.html

Java: // 手写回溯递归
来源：http://hz.jianghu66.top/gternpftar.html

Go:   // 手写回溯递归
来源：http://hz.sweek.top/gtshrjitwj.html

Ruby: arr.permutation.to_a
来源：http://hz.yuxming.cn/gtwbpaetvm.html

C#:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gttvdhbqxy.html

[N09] 栈与队列
来源：http://hz.yuanzhike.top/gtznaywydx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.wangshuangyany.cn/gtwfwtomyc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtjckrgezi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.iojbl.cn/gtlnhjbsnz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenzaomai.com/gtwaknyryc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj202588.top/gtrytscbdi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gogol.net.cn/gtakckrwva.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtxwgzlrhp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hnxiangtu.top/gtmmmqqtld.html

[N10] 链表节点定义
来源：http://hz.zhijiandao.cn/gtkgldvidj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xziqi.cn/gtdmknenhk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hywenlv.cn/gtkfxdtvah.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fengsongda.top/gtxzpwglwj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dashuyun.cn/gtsobuiqdz.html

Java: class Node { int v; Node next; }
来源：http://hz.shuidangran.top/gtcvdbmfoi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xinyue.icu/gttsqmdpiv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cheryme.top/gtxtjgjszt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhijiandao.cn/gtaxkyxjzo.html

[N11] 二叉树中序遍历
来源：http://hz.kuanghao11.cn/gtsbcuuxsv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ehwqpu.com/gtzqbailiv.html

PHP:  // 手写递归函数
来源：http://hz.nwbrower.top/gtdzzkxjam.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtqxgrbsiq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtuavsdyfa.html

Java: // 手写递归
来源：http://hz.sufxvd.cn/gtxhtquenc.html

Go:   // 手写递归
来源：http://hz.ybcxt.top/gthgprotcf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guowangkeji.top/gtnfltzuoi.html

C#:   // 手写递归
来源：http://hz.cucudq.cn/gttajqlnvb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yonumen.top/gtavboozzd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jyoumei.cn/gtvcpcnolx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jiagoushi.top/gtygomsbje.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yueranfly.top/gthqtxihni.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gtvlmemuhj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dianchejie.cn/gtkjexsaxo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pengpengdd.cyou/gtgsduiuxf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xylfe.cn/gtjnplowzq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtnylvuoob.html

================================================================================
来源：http://hz.xylfe.cn/gtpzqsznhl.html

O. 并发与异步
来源：http://hz.cashguo.top/gtlhhlvxjs.html

================================================================================
来源：http://hz.jqgfzy.top/gtrsgimpza.html

[O01] 启动一个线程
来源：http://hz.sweek.top/gtbsxzntec.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hnxiangtu.top/gtivurvecc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shuidangran.top/gtitlazofv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhiwuduotai.top/gtcjowmiuw.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtzrczcwxj.html

Java: new Thread(() -> f()).start()
来源：http://hz.aibaodan.cn/gtbquyepzw.html

Go:   go f()
来源：http://hz.sysykeji.top/gtrjnsiwlw.html

Ruby: Thread.new { f }
来源：http://hz.ehwqpu.com/gtgtovkrfh.html

C#:   Task.Run(() => F());
来源：http://hz.ybcxt.top/gtbxdfnven.html

[O02] 使用线程池
来源：http://hz.jlsjyb.cn/gtvcjblotd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinqigufen.top/gtpvdcqsjz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sxryk.cn/gtlgzsejby.html

JS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gthqhmhmzx.html

TS:   // worker_threads 线程池
来源：http://hz.jinghuilouyu.cn/gtkesplomx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jqgfzy.top/gtgexbgwgr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhongyouzk.top/gtmqvvhhnt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.52xcode.cn/gtpobtebts.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nwbrower.top/gtkwvjhwec.html

[O03] 加锁保护共享数据
来源：http://hz.52xcode.cn/gtimqiyiiy.html

Py:   with lock: shared += 1
来源：http://hz.ehwqpu.com/gtphfeqony.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.haohaochexian.top/gtjtbjlhva.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenzaomai.com/gtvbgicurd.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtjofxzqif.html

Java: synchronized (this) { shared++; }
来源：http://hz.yonumen.top/gtsfkhoneg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuxming.cn/gtyqfwzquj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ydjk.org.cn/gthzyklthx.html

C#:   lock (gate) { shared++; }
来源：http://hz.bjfxy.top/gtfrlnywxz.html

[O04] 定义异步函数并等待
来源：http://hz.ivvv.top/gtheknqmvg.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgfzy.top/gtrqiwglvu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xylfe.cn/gtsytkbgyd.html

JS:   async function f() { await g(); }
来源：http://hz.hongshengwenyu.top/gtwtzeukuq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhongyouzk.top/gtgueoummc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shzxlz.cn/gtqblsuyop.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinghuilouyu.cn/gtqzfqgvwr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cucudq.cn/gtihgaknbp.html

C#:   async Task F() { await G(); }
来源：http://hz.sysykeji.top/gtluydkpad.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigfzy.top/gtxuuybnal.html

Py:   asyncio.gather(*tasks)
来源：http://hz.havefunace.top/gtfqjpkmek.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shuidangran.top/gtdszlglzn.html

JS:   await Promise.all(tasks)
来源：http://hz.snrcjt.cn/gtlgjtbgwr.html

TS:   await Promise.all(tasks)
来源：http://hz.vqdsnc.cn/gtagsaemhw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.smart0.xyz/gtflimsbcn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jiagoushi.top/gtlyuiivva.html

Ruby: threads.map(&:join)
来源：http://hz.daxiang520.top/gtlaycvsat.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fengsongda.top/gtyawatfqr.html

[O06] 使用进程池
来源：http://hz.zycfv.cn/gtermsxgwr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ybcxt.top/gtpnlsjgwn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinqigfzy.top/gtqbbcdewa.html

JS:   // child_process / cluster 模块
来源：http://hz.jqgufenzy.top/gtzggrxuue.html

TS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gtbmsgrury.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhongyouzk.top/gthybtavsv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.c1oappe.top/gtujbaavus.html

Ruby: // fork 块
来源：http://hz.shanyushiyangtech.top/gtbdjexnyf.html

C#:   Parallel.For
来源：http://hz.tanke756.top/gtsoaqxqsp.html

================================================================================
来源：http://hz.hfpthk.cn/gtaxksseyc.html

P. 常用工具函数
来源：http://hz.jinghuilouyu.cn/gtokilgzzp.html

================================================================================
来源：http://hz.sweek.top/gtdfafwgnj.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtnuybtfcz.html

Py:   str(uuid.uuid4())
来源：http://hz.jiagoushi.top/gtorenxkre.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hammf.cn/gtiejxyfkc.html

JS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtyuwqdchb.html

TS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtlibxmaql.html

Java: UUID.randomUUID().toString()
来源：http://hz.jyoumei.cn/gtsgysnuny.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pengpengdd.cyou/gtmawxkfsc.html

Ruby: SecureRandom.uuid
来源：http://hz.fzhhl.top/gtomytwmel.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.316326.xyz/gtydpuqiyx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jyoumei.cn/gtlxpjfguj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hfpthk.cn/gtvdtirmmu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jqgufenzy.top/gtboxmzyfh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hongshengwenyu.top/gttkkhweai.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxinkj.top/gtsciyqwct.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sxryk.cn/gtmyvmukex.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yvedp.cn/gtymjuskrq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sweek.top/gtlvlltzsz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenjidiqi.icu/gtsmvvawyw.html

[P03] 生成短随机字符串
来源：http://hz.zhengqikj.top/gtccujczse.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.kuanghao11.cn/gtdbeslvqf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ehwqpu.com/gtfozovshr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yvedp.cn/gtkobobfhi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gtgabveron.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ybcxt.top/gtupdsadru.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hnqzz.top/gthkwmegxq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yvedp.cn/gtwmvmqmcz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dianchejie.cn/gtqybauuoo.html

[P04] 求长度
来源：http://hz.316326.xyz/gtlmgfnnmf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yongpay.top/gtokuveqgp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ivvv.top/gtaourhiac.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.vqdsnc.cn/gtnqetiube.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.bjfxy.top/gtzhtoagmo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zdqjudy.top/gtysdimhvd.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gtslhvrayc.html

Ruby: x.length;  x.size
来源：http://hz.aibaodan.cn/gtgwgvecie.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zdqjudy.top/gthwfssaox.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gthswcnxlo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.fengsongda.top/gthmcghjjp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.andypj.xyz/gtsrbdwrbo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgfzy.top/gtooiomnli.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258888.top/gtmltbywgf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.guowangkeji.top/gtclkyvhhj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxuanxn.top/gtltrhpqow.html

Ruby: a == b
来源：http://hz.birdmap.top/gtslahxeoe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.fzhhl.top/gtuiadzmei.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dianchejie.cn/gtvknskypm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yvedp.cn/gtiusedxux.html

PHP:  if (empty($x)) {}
来源：http://hz.gaohongyu789.top/gtywudgtsk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tian-w.cn/gtnbskxueu.html

TS:   if (x == null) {}
来源：http://hz.zhoulong.xyz/gtdexprqip.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jyoumei.cn/gtwhmeocde.html

Go:   if x == nil {}
来源：http://hz.jianghu66.top/gtekwpwzqd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.dianchejie.cn/gtqxtcmttc.html

C#:   if (x is null) {}
来源：http://hz.xuetiantiany.cn/gthkqkwgsc.html

[P07] 防抖与节流
来源：http://hz.hongshengwenyu.top/gtxhubznrk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.316326.xyz/gtsdnfvqdk.html

PHP:  // 手写时间戳比较
来源：http://hz.cucudq.cn/gthtrwttra.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtmmejsduh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hammf.cn/gtaycvagcb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sxryk.cn/gtlxurkurt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xuetiantiany.cn/gtvjqaonzk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pycfn.com/gtgurpvtzl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.redwolf501.top/gtuuxeyfkm.html

[P08] 处理浮点精度问题
来源：http://hz.gaohongyu789.top/gtzghphpzn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258.top/gtwsycylkk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.quarkkingdee.top/gtqhrcelaq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cdnleiting.top/gtwwzjrbpy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ivvv.top/gtaejmuuxr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yueranfly.top/gtbgwjpwqr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.kuanghao11.cn/gtunxwjirj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ybcxt.top/gtbogoltpf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.dianchejie.cn/gtpotjqlgi.html

================================================================================
来源：http://hz.yj20258888.top/gtzysiwnfu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj202588.top/gtozzdmebb.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gttffficrt.html

[Q01] 创建表
来源：http://hz.hammf.cn/gtjhhnfado.html

CREATE TABLE users (
来源：http://hz.tanke756.top/gtjuewbvbm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhoulong.xyz/gtlinafcyj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xylfe.cn/gtytdfiwan.html

email VARCHAR(100) UNIQUE,
来源：http://hz.52xcode.cn/gtvtdepbcn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhijiandao.cn/gtezqwzgfg.html

);
来源：http://hz.xziqi.cn/gtukipolcm.html

[Q02] 创建带外键的表
来源：http://hz.nanxuanxn.top/gtgzsfwzzw.html

CREATE TABLE orders (
来源：http://hz.guannengcc.top/gtbpeauceq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.andypj.xyz/gtaapspugb.html

user_id INT NOT NULL,
来源：http://hz.dianchejie.cn/gtjqwxygwr.html

amount DECIMAL(10, 2),
来源：http://hz.jlsjyb.cn/gtzchwvexe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.snrcjt.cn/gtzvbhkztu.html

);
来源：http://hz.jianghu66.top/gtbccxzhvq.html

[Q03] 增加列
来源：http://hz.xinyue.icu/gttitkryyu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhiwuduotai.top/gtbcqwhnao.html

[Q04] 修改列类型
来源：http://hz.xylfe.cn/gtpfwxkyds.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.smart0.xyz/gtlziftqhc.html

[Q05] 重命名列
来源：http://hz.fzhhl.top/gtqxeuzuzw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhijiandao.cn/gthwjsxflz.html

[Q06] 删除列
来源：http://hz.havefunace.top/gtoeslnvsi.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.pycfn.com/gtsgahuvwl.html

[Q07] 删除表
来源：http://hz.guannengcc.top/gtvqoejhyj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhiwuduotai.top/gtsvsyyksh.html

[Q08] 创建普通索引
来源：http://hz.chenjidiqi.icu/gtfvrwnjgh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gtwrdefxsb.html

[Q09] 创建唯一索引
来源：http://hz.gogol.net.cn/gtahelsloz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daxiang520.top/gtmfeuiwhq.html

[Q10] 插入单行
来源：http://hz.dianchejie.cn/gtyxpdgiil.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shuidangran.top/gtyyaqegkn.html

[Q11] 一次插入多行
来源：http://hz.shzxlz.cn/gtynsghivb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shangyingyoupin.top/gteprvzxiy.html

[Q12] 插入后取自增 ID
来源：http://hz.yuanzhike.top/gtuosbeugl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ehwqpu.com/gtdwkupdcu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenlongwang.top/gtnpcyuozc.html

[Q13] 忽略重复插入
来源：http://hz.52xcode.cn/gtddlwhaoe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangkeji.top/gtcqmwzrwc.html

[Q14] 存在则更新（upsert）
来源：http://hz.0kj1m.cn/gtpobauhij.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnxiangtu.top/gtuwynxebf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hfpthk.cn/gtndmipiyd.html

[Q15] 查询全部
来源：http://hz.hnqzz.top/gtedshgnvx.html

SELECT * FROM users;
来源：http://hz.hnxiangtu.top/gtjcrdtfqx.html

[Q16] 查询指定列
来源：http://hz.xylfe.cn/gtgvqlzyhn.html

SELECT id, name FROM users;
来源：http://hz.ydzc1.top/gtkpkitagc.html

[Q17] 条件查询
来源：http://hz.sysykeji.top/gtlcsaykqe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.aibaodan.cn/gtjmvkhgse.html

[Q18] 模糊匹配
来源：http://hz.zdqjudy.top/gtseyvocyx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.kuanghao11.cn/gtctsqpctd.html

[Q19] 范围查询
来源：http://hz.nanxinkj.top/gtohetqdjz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhixingplan.top/gtjudsfwux.html

[Q20] IN 列表
来源：http://hz.cqqwz.cn/gtmdvutgxi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nwbrower.top/gtjubjgfrm.html

[Q21] 空值判断
来源：http://hz.daria6918.cn/gtglhgetcq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shangyingyoupin.top/gtjdrunvxm.html

[Q22] 排序
来源：http://hz.ydjk.org.cn/gtheinoral.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhongyouzk.top/gtsjpbplgj.html

[Q23] 分页
来源：http://hz.yj202588.top/gtvuwtxuat.html


<!-- 参考信息 -->