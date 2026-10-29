代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gactufqek.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gnzzsbhcd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/ghduqndrx.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gjccwogji.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/goegmrojw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/glovtvqjh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gbvkgqmtg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gcjflaimf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/grvqrtxwt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gloiyaftn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gywztlnsk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gfvocuvsk.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gcgangtuk.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gtfcnaghq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gnwqyquyp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gxnbgqllm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gwhfpgqxy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/ggeidzpnh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/ghzcdudsu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gdpitsfnm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gwsgldsol.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gueitvzmi.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gcgfgikgz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gbfyeexpk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gadsrhwrm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gyywteaqv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gnwpmatnn.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/glqxsrdvs.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/ghnazeter.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/goagrrmdl.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gfvqpjgob.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gwydgknjl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gjwjaatfo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/giyolhlgt.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gbcknbrad.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gltanstyj.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gzxnqqadg.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gsfnwnrcs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gjmeeaphq.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gsjfajpnm.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/glgjsvxib.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gonmwslai.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/goanjpeso.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gginozxdl.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/goidovktg.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gpouaiynw.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gfszakrgd.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gqvckqhci.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/garneztyx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gdierjgia.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gnnyrxxmv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gilnyiecv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/glrwzaqwl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gabdxufbs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gyjknubkl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gnwypkvzm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gvpyrncyy.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gymmegekd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/goxpsqrqv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gnrgnoxxv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gykpvqmzd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gdruefcsc.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gvipsqkfl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/ghybvhfjm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gmwmmembk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gxzutlrmu.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gsclcoxzk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/ggtlkzyvy.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gxszjkrtb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gqbrqzgpe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gcdybsplf.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/glgjtmxwa.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gmbskoedn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gyarafxdq.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gmawmcvri.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/ggeuagnxq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gjxlaudpu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gtmxrystx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gtzfavhfd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gvyrcasfe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gxkgdttff.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gwreqldba.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gasurqhsv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gerpzuwld.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geuomsscg.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gwlyqxzse.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gubekgehv.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/ginkqphmi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gsftivfuy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnptmkklc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gffkmfwlu.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/glgmrdmbl.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gxnjqvqxi.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gunrrszjr.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gboqifpwk.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/ggcpajfxs.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gkifzlfrj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/ghepsrfsk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gnnzkjbex.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/ggyqhysqo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gngsmoyhq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/ggrbsyxja.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gzaxcuuel.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/ghmllkibw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/ghkmewotf.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gmidrgaqc.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/guxqnflpk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gljvpsahf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gtyfguzze.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gwhpxdkip.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gjacczbob.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gojbtvriz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/grkygtzil.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbcypudoq.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gbinpiwee.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/ghajwxtlc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gilqdbfuh.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gqufyqwau.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggapqwobp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gkhhgzgtz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/grqdkfnil.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gjuclphil.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzyzftivj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gsbutwpjd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gztohyuqj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gealyoymv.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/ggayvfcvs.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/ghyrgbzgv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gtismivhu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gijjofjhn.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gqnqdmshw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/grzfblkjl.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gakohvset.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gvcekfoqa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gdctmzwvi.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gpxvdbxfq.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gjgyinfnc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gwbxvvwby.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gkkezgbuq.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gxccrrwgt.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gsjyxrgfb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glsjkdwkr.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gconcsxbu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaqlxtguf.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/guuurqcke.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gtoqhiywx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gzjkbsxyw.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gwukdmove.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gnnkoyhnc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gsnszhnqj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gpvjgwdwp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gcbysdcbw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gexuiyajx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gxuaodzcd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gbvnoqjqi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxwfshcu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gbgjrzhjf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gsajbglew.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gmuuqglha.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gfdgerqwn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvzfhfrtz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gduqzlnfy.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/guklaksrb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gprhygywh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gidcxuuiv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gvrxtdaxl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gelkcjqsy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/garckhulg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gywflvkyg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gcemxbalg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gjsrjzflb.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gufiuklla.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/godicrzpj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/grlmcgvbg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gpvrtcmko.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gfetwgnuc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gljvihiwy.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gwhkjgxsk.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gwojvbzqd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gojfyuvvo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gejkljtdb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gbcazkefs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/guvgztmet.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gxbybblqw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gmewkizoh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gdeelkjiu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gwvugdqen.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gqxfpddex.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gpqilmobm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gxninaglk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gpscatmwv.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gbsorpipb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gltfjojvu.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gpzjyoiuf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gbhzqaxyb.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gfyiyeppd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gslixghsd.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gxvazcowa.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gaxtxstzm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/glwpajibq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gjxqrijcn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gfskbczuy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gytqzjudo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gyhcqplfj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gwakrnaxo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gdzcvmcmu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/guaezjhsl.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gctyanhnv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gtsxxcmfn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gmrcemqbr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/giklignaj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gglfonmiw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gviemhdlh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/guorbsogp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gvisxajaj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gtwgfudld.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxfrzpwie.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gapyjhgeh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwjjpnonw.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gygvbpoxj.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gvznqlbqo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/ghmgukqlg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gcwlpsehi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/ghuaxechj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gzpejfoqv.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gcrkznscm.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/grfmgfprd.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gtuonrrgl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gdlqwhddj.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gtcgqlvqo.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gklqpguep.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gavjlvydi.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gymdvghcy.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gayihrhaj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gvzinlfux.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gwphmcgrq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gmwwxmmdg.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gfefvklkk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gihtwpyiu.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/ghjfimxny.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gfsqmhbdi.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gjekfykzt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gkcnnbxxr.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gtapadefo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gvexkcjzn.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/glafmkyyf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gcxpbggil.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gvhvajnyk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gtqtwkaoh.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/ghwweamuk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/ghoeutvks.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/godrixszy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gnsbusohf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/grdonuwjt.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gtdhtjskv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gibrjyqfr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/ghuiqqlso.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gsvuagcek.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gpltwgtci.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gudezllmz.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grgskzylq.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gradgujja.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/govhrfoyd.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gvtsqprym.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gmzkkzncc.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/ggolqccfo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/ghdpdnjjl.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gcaeeicog.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/goktaowsy.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gwulstane.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gkrybhryj.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gbaytrmdi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gqiclxrzl.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/ghflizofe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gkfhrobhp.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/giwpmjtcm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/geceuvoqh.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/grecdurnc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfhlsvlhv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gqmmyrvzj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gqjlakobs.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gwxzlqudv.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gpluhczzk.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gbuufdwvq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gglrzoedu.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gsducftuw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/grmgcuuab.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gplzncxue.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gasjlqzzb.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gymlwvpuw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gygjfagyk.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/ghrlwgblu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gavzagphe.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/genmcnulc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gaozspkjr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/goadtbtva.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gvffweete.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gplezdujj.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gmolvzvxx.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/guvshcdoo.sHtML


<!-- 参考信息 -->