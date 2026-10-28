代发 wailian999

TS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtcmbvnuyv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtzwegylnt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hammf.cn/gtbrxzbfoi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hammf.cn/gturdgqdve.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gogol.net.cn/gteqvvvazo.html

================================================================================
来源：http://hz.xylfe.cn/gtrffdpiha.html

N. 数据结构与算法
来源：http://hz.zhengqikj.top/gthhpieupc.html

================================================================================
来源：http://hz.jinqigufen.top/gtlmjeymwh.html

[N01] 二分查找（有序数组）
来源：http://hz.sweek.top/gtoxcqdpnt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhixingplan.top/gtshqegokc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenlongwang.top/gtntsfqasy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtwasiomtw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gttlzlwedx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangdashe.top/gtsrwvliiv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jiagoushi.top/gtvvowfvkc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuxming.cn/gtlfcxqomb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tian-w.cn/gtwbxcyhhl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fzhhl.top/gthnbgkboy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.52xcode.cn/gtgapvxhyj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ydzc1.top/gtduvnpeeq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtgpbxintt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtnybgqcov.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xingfuxueyuan.xyz/gtrbwnhvpn.html

Go:   slices.Sort(arr)
来源：http://hz.shuidangran.top/gtrzntlmxv.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gteqsmwsef.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.aizwys.cn/gtfjryrgai.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigufen.top/gtrldfnvhu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xinyue.icu/gtipxeypjf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fengsongda.top/gtbmgizbcy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtnjfprguw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gtyjgfofja.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hfpthk.cn/gtkoqtkvay.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.kuanghao11.cn/gtoqtyhzwk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuxming.cn/gtgdcvkooi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinghuilouyu.cn/gtuxbwxerr.html

[N04] 斐波那契数列
来源：http://hz.jqgufenzy.top/gtwviimyrs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gthcwilpgy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hysaishi.cn/gtbnubgags.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gtfmijkaxo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gtkzcdbtcv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.0kj1m.cn/gtebotzzrx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuxming.cn/gtulwcojaj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuxming.cn/gtquetumsn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xinyue.icu/gtlgnzpazu.html

[N05] 最大公约数
来源：http://hz.chenjidiqi.icu/gtrqinguep.html

Py:   math.gcd(a, b)
来源：http://hz.zhoulong.xyz/gtnulyzeqz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.snrcjt.cn/gtgjpwzxmp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinyuanbaomall.cn/gtckuiuojh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuanzhike.top/gtcqdcmzdm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xingfuxueyuan.xyz/gtdbqatzcq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ivvv.top/gtkucsvdpx.html

Ruby: a.gcd(b)
来源：http://hz.hysaishi.cn/gtrgckruib.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shzxlz.cn/gtkoviobgi.html

[N06] 判断回文字符串
来源：http://hz.fzhhl.top/gtzrhqoosu.html

Py:   s == s[::-1]
来源：http://hz.c1oappe.top/gtwhqvrlom.html

PHP:  $s === strrev($s);
来源：http://hz.fzhhl.top/gtzrsktzxt.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtfojqiscj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtjzjcglnj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yonumen.top/gtsbjlvkjl.html

Go:   // 双指针从两端比较
来源：http://hz.sufxvd.cn/gtnyfqgdmw.html

Ruby: s == s.reverse
来源：http://hz.nwbrower.top/gtzckideal.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtkquvuqdw.html

[N07] 两数之和（返回下标）
来源：http://hz.wangdashe.top/gtelchoson.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydjk.org.cn/gtsszltkig.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.dianchejie.cn/gtsgdgqyed.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.smart0.xyz/gtfaryszoz.html

TS:   // 手写 Map<string, number>
来源：http://hz.aizwys.cn/gtioxnmlhl.html

Java: // 手写 HashMap
来源：http://hz.xingfuxueyuan.xyz/gtumtqkvwf.html

Go:   // 手写 map[int]int
来源：http://hz.gzhubu.top/gtryvycnca.html

Ruby: // 手写 Hash
来源：http://hz.zycfv.cn/gtvagcscbp.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtaasuyuss.html

[N08] 生成全排列
来源：http://hz.shuidangran.top/gtopwxsyqg.html

Py:   itertools.permutations(arr)
来源：http://hz.c1oappe.top/gtwrurtkzs.html

PHP:  // 手写递归交换
来源：http://hz.zycfv.cn/gteznpfelx.html

JS:   // 手写回溯递归
来源：http://hz.yj202588.top/gtcfixoqhi.html

TS:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtkfntethm.html

Java: // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtsqrotomf.html

Go:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtcbavyktm.html

Ruby: arr.permutation.to_a
来源：http://hz.shzxlz.cn/gtuqgdzhtg.html

C#:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtgmelerdi.html

[N09] 栈与队列
来源：http://hz.shanyushiyangtech.top/gtkeasplji.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yueranfly.top/gtoyynbcnn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.smart0.xyz/gtpyoxdpet.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cucudq.cn/gttfwhvpql.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhaomingkeji.xyz/gtiyoumhmf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxinkj.top/gtajfxmbyd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tian-w.cn/gtvpvotlxy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cqqwz.cn/gtumdlyvex.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yonumen.top/gtpdoasxtj.html

[N10] 链表节点定义
来源：http://hz.mhx1999.top/gtuwqfaqzs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.smart0.xyz/gtnaftjbhf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.haohaochexian.top/gtxwrdutfi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigufen.top/gtjoqughmq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigfzy.top/gtvuzyfwkc.html

Java: class Node { int v; Node next; }
来源：http://hz.jqgufenzy.top/gtiadwblqh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xingfuxueyuan.xyz/gtccujexjf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangdashe.top/gtkyspwmuy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cheryme.top/gtuifkczhx.html

[N11] 二叉树中序遍历
来源：http://hz.svipenyu.cn/gtrbfhgarn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ivvv.top/gttikehlnd.html

PHP:  // 手写递归函数
来源：http://hz.iojbl.cn/gtlngwfupv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fengsongda.top/gttlziswln.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gttthkocof.html

Java: // 手写递归
来源：http://hz.zhixingplan.top/gtodhmorzr.html

Go:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtskfgkrlk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xziqi.cn/gtopnvildh.html

C#:   // 手写递归
来源：http://hz.zhiwuduotai.top/gtpixjpwjh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhengqikj.top/gtjhdkmqvn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangdashe.top/gtkdzqjmlg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhijiandao.cn/gtamopcyvb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtmgdyrmbu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtqdcshhyu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gtkpkcihgd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xingfuxueyuan.xyz/gthczquuat.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jlsjyb.cn/gtffmffenq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtxydvefwg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtbtxsknme.html

O. 并发与异步
来源：http://hz.hywenlv.cn/gtjmihgaop.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtzsaxbpsh.html

[O01] 启动一个线程
来源：http://hz.yj20258.top/gtmsogcjwx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenjidiqi.icu/gtkauaiqae.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhiwuduotai.top/gtzizsyagl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj20258.top/gtbwxphgft.html

TS:   // 同 JS
来源：http://hz.hnxiangtu.top/gtksuhxbpv.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangkeji.top/gtkdctdggl.html

Go:   go f()
来源：http://hz.0kj1m.cn/gtczpgfzlb.html

Ruby: Thread.new { f }
来源：http://hz.hnxiangtu.top/gtwtshifau.html

C#:   Task.Run(() => F());
来源：http://hz.aizwys.cn/gtyoninoun.html

[O02] 使用线程池
来源：http://hz.bjfxy.top/gtfcslauhe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.havefunace.top/gtwoqkgtmm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hammf.cn/gtotnqkmgt.html

JS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtnxpahekp.html

TS:   // worker_threads 线程池
来源：http://hz.ydzc1.top/gtcrhsnadj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cqqwz.cn/gtfetuwijl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangshuangyany.cn/gtfoxqnqwr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pycfn.com/gthwhunczq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tian-w.cn/gtqtfpkqrm.html

[O03] 加锁保护共享数据
来源：http://hz.yj202588.top/gtbqbiyrrn.html

Py:   with lock: shared += 1
来源：http://hz.gotoacloud.top/gteqcxvrwh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fengsongda.top/gtpxifwfas.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.iojbl.cn/gtggizfawj.html

TS:   // 同 JS
来源：http://hz.ppjwa.cn/gtqntbfydj.html

Java: synchronized (this) { shared++; }
来源：http://hz.yueranfly.top/gtxvcpkwix.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cqqwz.cn/gtywzkqdij.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tian-w.cn/gtpcvppdhl.html

C#:   lock (gate) { shared++; }
来源：http://hz.ybcxt.top/gtpkjdqcrc.html

[O04] 定义异步函数并等待
来源：http://hz.gogol.net.cn/gtlwedufgb.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigfzy.top/gtelcixued.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuanzhike.top/gthjplftjg.html

JS:   async function f() { await g(); }
来源：http://hz.vqdsnc.cn/gtlwpdbmab.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.snrcjt.cn/gtutfzjxrs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.feifeiyinyue.top/gtoquathfs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zycfv.cn/gtasbxgsep.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinqigufen.top/gtujytbdna.html

C#:   async Task F() { await G(); }
来源：http://hz.chenjidiqi.icu/gtyewvdqrg.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhongyouzk.top/gtmsnlmbzu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gtpcutvufk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.feifeiyinyue.top/gtmjotccqv.html

JS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtujznqgwl.html

TS:   await Promise.all(tasks)
来源：http://hz.gogol.net.cn/gtdzgxeuwj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tianlin.xyz/gtipzittfj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yangfankeji.com/gtevtkoall.html

Ruby: threads.map(&:join)
来源：http://hz.zhoulong.xyz/gtqosmjzaf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hywenlv.cn/gtsebgrzeb.html

[O06] 使用进程池
来源：http://hz.andypj.xyz/gtiixxkzfz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnxiangtu.top/gtxirpwnho.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fengsongda.top/gtdbkzeyyk.html

JS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtdnjfthxv.html

TS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtvmibvxgq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yanxiufei.cn/gtjifxmqxp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhijiandao.cn/gtlryquacm.html

Ruby: // fork 块
来源：http://hz.zhoulong.xyz/gtbltxrgmh.html

C#:   Parallel.For
来源：http://hz.hywenlv.cn/gtslkhitjw.html

================================================================================
来源：http://hz.aibaodan.cn/gtyoywyihq.html

P. 常用工具函数
来源：http://hz.nanxuanxn.top/gtxbsrdngl.html

================================================================================
来源：http://hz.yvedp.cn/gtvdpkltrf.html

[P01] 生成 UUID
来源：http://hz.ywan-chungtsiang.top/gtpufqtrwv.html

Py:   str(uuid.uuid4())
来源：http://hz.gogol.net.cn/gtibepohnh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.havefunace.top/gtjdrvtuuv.html

JS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtfkcphapj.html

TS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gtukhnvcrc.html

Java: UUID.randomUUID().toString()
来源：http://hz.yangfankeji.com/gtqeadykbu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.daria6918.cn/gtborqhura.html

Ruby: SecureRandom.uuid
来源：http://hz.zhixingplan.top/gtejdjgkug.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinyuanbaomall.cn/gtspdicmsf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.redwolf501.top/gtfyvtqaka.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yangfankeji.com/gtdfqvkbkn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuanzhike.top/gtqjxphebk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhongyouzk.top/gtrzbycfae.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pengpengdd.cyou/gtnisvgqqg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yonumen.top/gtuzcfotka.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cqqwz.cn/gtndjqinnb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.svipenyu.cn/gtqndyrbye.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuanzhike.top/gtgaxqbbmc.html

[P03] 生成短随机字符串
来源：http://hz.pycfn.com/gtdqrntpsu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ybcxt.top/gtvrysijzq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xziqi.cn/gtpgfoklsf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtrgtgmeek.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtwdwdneiq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gaohongyu789.top/gtuzkhppss.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hysaishi.cn/gtaeqlnlij.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yongpay.top/gtaeyzyvnr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.52xcode.cn/gtpsamkvio.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gtdaocwqru.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ydzc1.top/gtcnmvlqky.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gttrhytdcv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nwbrower.top/gtqkgbabjx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtabouubjj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.svipenyu.cn/gtkzeeglfy.html

Go:   len(arr);  len(m)
来源：http://hz.pengpengdd.cyou/gtmvqajwtq.html

Ruby: x.length;  x.size
来源：http://hz.havefunace.top/gtzrzlihuv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shangyingyoupin.top/gtobbuctcl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangkeji.top/gtpzrtiuvu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ppjwa.cn/gtgpwrbhvr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zycfv.cn/gtrhjsgttu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.9152youxi.cn/gtnajzbzqi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cheryme.top/gtyqxnnvit.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.aibaodan.cn/gtqfxyapxe.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hnxiangtu.top/gtdvshjuzt.html

Ruby: a == b
来源：http://hz.xuetiantiany.cn/gtauwqmrnt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yuxming.cn/gtuvlocroh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sweek.top/gtmcratgya.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.aizwys.cn/gtmdybfnmy.html

PHP:  if (empty($x)) {}
来源：http://hz.shuidangran.top/gtzxfqqxet.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.mhx1999.top/gtronmpcsl.html

TS:   if (x == null) {}
来源：http://hz.chenzaomai.com/gtlfhamcsz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.wangdashe.top/gtgrmwalvm.html

Go:   if x == nil {}
来源：http://hz.9152youxi.cn/gtzphcwbkk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhongyouzk.top/gtmlbdkuok.html

C#:   if (x is null) {}
来源：http://hz.ydzc1.top/gtouqrmyfx.html

[P07] 防抖与节流
来源：http://hz.havefunace.top/gtkzlxucoc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sweek.top/gtntrepfab.html

PHP:  // 手写时间戳比较
来源：http://hz.zhixingplan.top/gtvexzereo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.havefunace.top/gtwcrzoivy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtozkxwwtc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.9152youxi.cn/gtzvcnxppj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hfpthk.cn/gtcizdsbaq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gaohongyu789.top/gtzyafytdm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.snrcjt.cn/gtpuniniuw.html

[P08] 处理浮点精度问题
来源：http://hz.feifeiyinyue.top/gtkphwcovn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shanyushiyangkeji.top/gtugldfyjy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aibaodan.cn/gtaumhokva.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sxryk.cn/gtlklmwjgp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.feifeiyinyue.top/gttlguxopa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinqigufen.top/gtogdzgsld.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinqigufen.top/gtybqteimk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangtech.top/gtyjoqtwwp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.haohaochexian.top/gtywvpksuq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtewmpdxbc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hfpthk.cn/gtocvpeccd.html

================================================================================
来源：http://hz.xylfe.cn/gtxfebgwvv.html

[Q01] 创建表
来源：http://hz.hongshengwenyu.top/gtqgviyuyj.html

CREATE TABLE users (
来源：http://hz.zhiwuduotai.top/gtlyfgnjar.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.vqdsnc.cn/gtealranox.html

name VARCHAR(50) NOT NULL,
来源：http://hz.quarkkingdee.top/gtptfddvxx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yongpay.top/gtfqwypmet.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.smart0.xyz/gthbtozqat.html

);
来源：http://hz.shanyushiyangkeji.top/gtobiqekqt.html

[Q02] 创建带外键的表
来源：http://hz.smart0.xyz/gtqtomewxb.html

CREATE TABLE orders (
来源：http://hz.pengpengdd.cyou/gtanwhauxe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gtvgtvwckm.html

user_id INT NOT NULL,
来源：http://hz.smart0.xyz/gtngyooien.html

amount DECIMAL(10, 2),
来源：http://hz.wangshuangyany.cn/gtljwxbasw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yj202588.top/gtboksnfor.html

);
来源：http://hz.haohaochexian.top/gtpqvlsjsq.html

[Q03] 增加列
来源：http://hz.shanyushiyangtech.top/gtbclvamve.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.andypj.xyz/gtekxpvcui.html

[Q04] 修改列类型
来源：http://hz.andypj.xyz/gtyuiykjvc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jqgfzy.top/gtdirqkszn.html

[Q05] 重命名列
来源：http://hz.chenlongwang.top/gtxfsfivqe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhiwuduotai.top/gthbnvrelq.html

[Q06] 删除列
来源：http://hz.daxiang520.top/gtaqojsems.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sufxvd.cn/gtazaoyujl.html

[Q07] 删除表
来源：http://hz.c1oappe.top/gtgdyxfzlx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.kuanghao11.cn/gtmeereowr.html

[Q08] 创建普通索引
来源：http://hz.daria6918.cn/gtqgrkueuu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xuetiantiany.cn/gtonhrdhqe.html

[Q09] 创建唯一索引
来源：http://hz.ydjk.org.cn/gtqlrlncso.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj202588.top/gtiuermmzf.html

[Q10] 插入单行
来源：http://hz.yonumen.top/gtbfkwdudn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hfpthk.cn/gtftgfcqji.html

[Q11] 一次插入多行
来源：http://hz.guannengcc.top/gtryfyvbun.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258888.top/gtltaqweuq.html

[Q12] 插入后取自增 ID
来源：http://hz.chenjidiqi.icu/gtixlwknqt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sxryk.cn/gtqwiunwwh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yonumen.top/gtddbzduln.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gthrihkfdy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.52xcode.cn/gtrsuzuvqs.html

[Q14] 存在则更新（upsert）
来源：http://hz.feifeiyinyue.top/gtqhhvxqgs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sxryk.cn/gtjcognpri.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hammf.cn/gtutgdcnne.html

[Q15] 查询全部
来源：http://hz.xylfe.cn/gtfdmjqkjw.html

SELECT * FROM users;
来源：http://hz.meibo888.top/gtknbunlnn.html

[Q16] 查询指定列
来源：http://hz.9152youxi.cn/gtjjtvttnw.html

SELECT id, name FROM users;
来源：http://hz.cheryme.top/gtoflulwjp.html

[Q17] 条件查询
来源：http://hz.zhijiandao.cn/gtckdwnqdd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cashguo.top/gtoqgjcwfp.html

[Q18] 模糊匹配
来源：http://hz.jianghu66.top/gtofujzwsl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shangyingyoupin.top/gtoyaoqrbv.html

[Q19] 范围查询
来源：http://hz.cqqwz.cn/gtsfgisaod.html


<!-- 参考信息 -->