代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gblzzdfpv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/guzgcnlge.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/ghawmrmmu.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gjvvzgwxs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/groaggdka.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gscejapex.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gzxcbtobc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gnwatgwpo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gijhbwfjc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/ggannhfba.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/grmqpaznz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gutdltcxj.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/ghkfaqaac.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gdrekznbt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/grfxheopk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gtwoijkcz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gfjmtbrsw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gkmajebqw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gccozgubx.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gwjkcfcrv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/ggkhthrut.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gbwvqoilk.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gbhzjuacg.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/ghvivzeen.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gpvalcsrs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gpovayhix.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gmdhgznkq.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/grjwomqxv.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/glwfaznur.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gejuvykyv.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gbefpzpek.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/ghcritzhz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gvygopfbm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gxrvpndww.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gccwprhee.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gyhumbhkn.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gdocgyrmj.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/ggkrrvqgx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gjmcxkfaa.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gkneysahr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gmytocxgx.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/glmytxdne.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqlpuwnlk.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gsthnpbnp.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gadqtubqi.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/grhmpiksp.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gbbiqeexm.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gphjnlenj.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtdxgovrc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/glvxcrhgk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gjkumfibg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gnpwzzinh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/giuxwrayk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gieiprasn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gyzvbgeql.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gaukbocpe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gsupmkbeu.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gnqxujkux.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gdcrdunhm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gsqmmfrnc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gmmzbthty.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gnaacvgkx.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gdyjkychh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gwqikhnoe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/glqpmtndo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gykdmhing.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/grmxdjgpl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gywqmqtet.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/geksjcbef.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gbelgovtm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gpzqotlqk.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gkncvdfex.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gztqchhno.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gebpdxwjg.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/grnstwhra.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gattmbayo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/glgvjsslq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gymsimqsq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/ghzuevwhr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gfhgtespm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/guhbxuyuy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gfmharmzp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/ghldozubi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gtkqekeuj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gydqmkmzn.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/ggdwtxgzu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcrbsptmm.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gzvgybmls.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gwbiuqvcx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gbcsljjmm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gifkqwiiu.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gidapduiu.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gzelafbjt.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gqbpttdet.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gzmeonqyo.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gclfemrwl.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gbozxpinp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gutnkthad.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gvwiyadex.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gszeyuyik.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/grnbvbfyp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzkyiphp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gtchjbxrp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gzmgkzegh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gkogixyum.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gjyxupbmw.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gwglllxnr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/ggzkuptes.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/geryyqglv.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gwnzpllqg.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gmbbndont.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gfhgdldms.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/geqqmfdpd.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gkfhqbuxd.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/ggieotdfu.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gwtxxmijx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/grofitzdt.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gifrczpsl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/grmhswvad.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gpacmescn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gnlvusbdj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gkodoxrpq.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gtozpyrkl.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/guiwgehfd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gvfeziile.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gbfcvorza.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/grztlkmwc.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gzuiygpob.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/goobawztx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gkqahbaod.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gizuojrdu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/ghuabicql.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gsptatqzf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gxljrbuuc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/ggthuxnjn.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/giuwssmht.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gtjzqxrsr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gzpoadvpv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gcbgoabfd.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gcozmmjpj.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gcwrhvrgy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqxqqnvxr.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/ggagjuabb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaqidjcvt.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gzdnqqkjp.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gltmhaabe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gpchlyxec.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gfmoejnmr.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/grnwedrkm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gialivdhz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gicehwitl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gbnrhinai.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/glorcetea.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/ghlbebgky.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gujqbsllw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/grnwndyif.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gxzjurghy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gsretsfbu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/grjewowur.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gylldqati.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gzgljbgoi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/glbsqqscd.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gqhijnwdz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gmwtxysas.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gskzamkrs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/grwzxgxyq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gbasozbdf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gjbmkrusz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gjkxoahia.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/ghgxdqjij.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gomlshnxy.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gobguptdn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gfppfymyd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gfbbbdpnq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gdpowmtrp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/ggucbrtli.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gbtsmniba.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gvyrnllxe.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/grrqhcygg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gnaurtjxe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gdmuwetoe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gmpbbuyfg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gnfqyazuq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gqamtptej.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gbgipwlwt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gtesmurae.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gsyvzelvo.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gtgivkvzd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gpcntfqwy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gzfvsfjew.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gtylsjuxd.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gxnhbaawq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gvqahidhu.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/ghvjxtpbb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gzcmvkgcs.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gggjaenga.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gsyhqprww.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gvflvkxis.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gkudlfrrn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gpvvtcsnm.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/glimbceye.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gjnyvvoxo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gjpccdrwt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/ggobdwbsp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gsfuyzfnk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gcwwiruxp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gzpuphamh.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/giufyzkwc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gigmjimpl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gjndjjdao.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gggievvbx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gxopyzrnf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gonjlwwyb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/giksgzjsl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gxdyvbncw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gzhoaquwq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjpuhlzzb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/grlbkcabm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfsfjmykh.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gtvavnsfk.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gtetomuqr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gxpukshno.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gurnkecmd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gwnuydlrh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gzasdmhcu.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gptpnlzqu.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/ggichxpoq.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gotozrzeo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gyxvgpkof.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gmjquznmd.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gffmaznut.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/ginalqjot.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gpspkrqvw.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/ghnsrnajx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gciirlhtt.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gjnyvkiaw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gtgaevbrk.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gkqbzyuqc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gykxseeaz.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/goqaocehz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gjlloevqy.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/geslckxkl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gqponewgh.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/glumvrsld.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gtlbkuzmp.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gunzfqxrz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gdskcjbhf.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gxgrxxdco.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gnauahgfc.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gsieixfxd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gbcxzcgng.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gejkfikkf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gdptirhdi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gbartkokg.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gwkykxkob.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gmntzohxz.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gufjzodyl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gnpdmgjwf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/ggjwfnjbq.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gnqyriqbm.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghvxbfvux.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gwibqfrag.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gadumiczv.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gsnkldwuq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gmzqpfepj.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gblzmsaoy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/ggiqtqczv.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gksqqugaj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gdhpehjow.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gqhgnggkm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gviummaev.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/geikoftdl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gxwplwxpf.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gprvsvfne.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/guzpdfriv.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/geimrutzf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gfjjtzunm.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gwcnklpwk.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gwxkxgbmo.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gkoiymfoo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gohyxxsjk.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gryhqaycq.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqoifvpri.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gsaifzsga.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtvznpycr.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gbbtqlwlm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gromwipqu.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gcwhxgmef.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsdrrdjve.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gafgeyjwb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gfmhksddg.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gyxjklhrj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gtnaxvrvs.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gyallekuz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/ghtsugbin.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/glbatesmn.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gyxehklgz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gqrpvtdtt.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gqjnvbjal.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gwaozjiqo.sHtML


<!-- 参考信息 -->