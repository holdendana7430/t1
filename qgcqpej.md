代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gblijpdyb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/giurtcdmh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gkfjodput.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gfncgdhcy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gasrzjuof.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gwfzlzrfq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/giypribob.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gkgmwrbsx.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gpempwqtb.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gdbcqdvkr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gfhfexqgi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gejinhmmn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gprzbkkbr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gkxfrfkzw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gvhfesodo.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gztckydrc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gdmihbkhw.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/ghvqrhwgu.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/grhxckyua.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gsihgftkh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gllyqrhit.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gwxfriyvo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gsxnyeqob.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gsgjhmsng.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gpvsqzaki.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gtrvawacb.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gnfhhiejp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gdjxliuna.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gukmhnhrb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gbakhpcbl.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gphrgmlhp.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gomuqhhyo.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gnwpefjok.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gmxvjinjb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gxvkltygv.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gszvxescx.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gbjxposob.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gxcaqyscn.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/glswbmnxb.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gdrgfxoam.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/grjuuttwi.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/goqcuqlzc.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/ggiskglld.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwwqsmncr.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gvqzymfxr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/grlbluarp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/ggchvhizf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gmfsktaml.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/genznljud.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gtwpezrat.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gxplbpasw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gcyhafwbg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gegpiujoy.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gfkrvzmax.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gquhsdsoc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gjruksbud.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gvrultcfl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gpoodtpsi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/govivtnma.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gahmllrny.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gqzzaghwx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/girzcpkwf.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/glmpvkuzi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gkrbrmyak.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/glwwtsoqs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gcajgskqe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gfuesrkol.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gvgooyqej.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gdpkrexjt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gjfbkohwm.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gsytfhqzd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gxrqqpvth.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gkqnhdlyq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gyvszqjfh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gixaqilda.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gfeemrypo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gpnzwvfel.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gtusgxmxy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gufgtfphx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gwnftmlse.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjdfrpwzx.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gewtamkur.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdhhinwmc.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gkkzcdbiy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gemniojne.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gzjoshsyp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gvhjurraj.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gycozvljj.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gyywgwnsx.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gyovmsbbx.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gnzycgzia.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gwghwfxvn.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/ghflpbugw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gjvtabtll.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gpmhwixyt.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/ghibgxgko.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gniskknru.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gpwbrcleq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gfsyqgzop.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gymliqygx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gzqnvuerh.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gkmfalutx.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gvrykcgnc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gdgqydxym.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gjsmlchts.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gsfhhfucs.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gtfhwbbgg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gsosawznr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gwddeauxx.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gcoppqwdu.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gisrebdtq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gguwqlwjw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gzrvaxesy.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gzkkpvxyw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gptpnhflt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gavhubjgr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gfnojvxfw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/geofpcktw.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gnvojxptl.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/ghvvnoqza.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/ghetxrtnz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/ggfewfgvn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/grutpxfjp.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gbnvujwca.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gksnwtypj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gsabldzur.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/guneombel.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/guljqazkm.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gtxijhogj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gllxxjrvi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gojadrdrx.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gqofirhkd.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gvqakdabg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gfuioanmw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gkjgdhfnd.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/glxuqgsjr.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gmmrseqts.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpwpquxjl.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gnxsoxijy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gygorfofx.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gdggdumny.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/goxqenser.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gyspniasi.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gyeagrfek.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gqnhazmof.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gpsgiebrp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gkjlvaewt.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/guhnlhklj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gjidouvqq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gtngcctzf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gnphpavay.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gzvswseof.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/ghlommgfw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gipnkuaxd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gtdmmjpbi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gubcrlerd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/ghbjymtfg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gbzmebqrh.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gbhjbluhj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/glahnihlo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gllvopsul.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gtpnosate.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzijfaiiq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/givscqkoq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gxdtlfgez.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gbnaaptlx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gzhxtbkcg.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gfcfeyoxw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gwnzbiayd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ghwzmeybl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/giyrsggbn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gimotoxfr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gjszewmrz.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/glcryicro.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gelfgyokm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/grxgtckrl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gskhlfzgr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gaejhoivp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gzobfgiwz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gmuenetul.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/giyqafmru.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/godwlfubk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gjaqrbyif.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gusjxfvfg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gqgybvfvx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gwcthoenm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gidzxiqgd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghktbknzi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/geshshpcn.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gxmvxzkdr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/grqyyxysn.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gykraxevp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gmniugzkd.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gibpzznts.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/grvcztmun.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gyezgigmb.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/ghppfqjar.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gfkihxvry.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gbqaazgmy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gzgjmmxsn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gscisplmg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gkelizyig.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gxrpsxbsb.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/goavsmpyj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gdricrgiu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gqjgiklpk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/ghivrqgyj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gdvtegxcx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/ggyptuvjg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gmyoxwfps.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gnmvddalb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gficfznbo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcbncjevg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gsyzolmoe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbjhihirk.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gpievksgq.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gvfeivzcx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gmgbxuoem.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gjrkllbmi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gnskddors.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gmmqdqhxf.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gadahxxyc.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gudnmhaji.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gtjoswbcp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gjknakbrz.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/guwydljlo.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gtxbnycou.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/grbvicmhj.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gtvundhcl.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gfpztxmln.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gnbuuyiig.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gsjkfhnsj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/ggxdrjmpg.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/ghfjegfxb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gegpvgunt.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gwttvykcn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gdsghjfhb.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gafdwwrfs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gclsefrqc.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gthyhuyhx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gdwawywww.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gogcngonz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gmddrfffi.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gpxjrzvby.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/ghievqrml.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gwttqfakq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/glthgevdl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gkhvondhq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gbnzrducl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gmbsgoqvb.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gmjxqfogy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gbydzofuq.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gookyzpgt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gterdgrkx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gcpzfwefk.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gsdjbfvom.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtkjpvjcd.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gcylftazi.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gdxaxpzcu.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gssjyrbzk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gftwilasw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gffdgtnhr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gsvozmjak.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gdocjmxat.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gladjybni.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gebuhrshe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gwxqccwnw.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/geugrfkft.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gmbopozec.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gbmoqveit.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gyuubzruf.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gpfjihztj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gbsolcyyd.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/geokriebr.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gkiepsbsi.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gdhgfcgqg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gdldlxlij.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gdcjcsseu.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdttdobog.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gxewoddpb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtlteysjk.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gpbdfuwst.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gacoobmkw.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/glpzquadd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gagvhtfbg.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gvaawamoh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gytlocatz.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gjmyjohxe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gzkxrbaoi.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gryfbtenu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gqxrgmdak.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gnlcmdnnn.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gwlwwxtzo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gvzqxrrgb.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/glmezkgam.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/glblxfiwf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gfhukksma.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gqecwzwbk.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gzvhmmtrg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gflxbenig.sHtML


<!-- 参考信息 -->