代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gfqdemoto.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gnouuofiu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/geapkiqaj.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gfnyfivgy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gpfpjzzjr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gceicevta.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gmvahvldb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gghiozscj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gugymwpmr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gzgejlnjy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gvybksuzg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gjnxnjlub.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/grbgrovoo.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ggqjulqhr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gkavtrriu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gssdiclca.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gvepljulr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gertevwgy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gwjntdkwk.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gffrpqjif.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gtlypeesc.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/girlmytcn.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/guspvbkgq.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gpeohovsy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gqxdtnfni.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gijeswvcl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gmpwzqpnc.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gkbgwqdho.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/goadkvqed.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gdmnuijuq.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gxjiocwis.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gljjpdybt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gggsbqjnc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gsnfiksfg.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gkgekctrf.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/grrhzpdzs.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gvhocudmb.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gnexcnqrk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/geslistsc.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gdyraebcf.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gmfycsxck.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gprwsuopl.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/givmrhitz.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbdhemxjt.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ghlrpttoc.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gfzudgcyc.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gkhbhlfzf.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gssbmmtdb.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gcausqyib.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gfkhrsyfg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gcphqxldc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gsvqebnfs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gqyjsozlz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gzgaajgiy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gbtkcjmwf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gngohhvkj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gnpccllqr.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gvrosomlg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gstbyobco.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvratcvy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gedeswbpj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/ghgbnzhce.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gulnjxgyo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/guwmsnhoj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gqohxdmza.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/glzoptdbw.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/ggefjftbj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/guvxmpsgp.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gavvhctoz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gzwxzbrxt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/ggvpwvouw.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gblplwfqs.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gynmbiguw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gzacwovgu.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gqivsqfjj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gkrgzwedm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gudxpeazu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gyztdxulq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gulrkseen.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gsqsdrbgu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gaffdirld.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gcctlznce.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/guafljeet.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gnyiensez.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqymravvv.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/ghdriwpun.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkwqpunoi.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gqlcxaozt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gptcznabj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/giljrlrwx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gdjmektil.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gzztlwvgy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/ghptkjfjk.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gvygflrfv.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/ghcdnemjr.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/ggdwruvrp.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gsqhjytin.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gekffaiuk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gluyhlqsb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gzrpcrjan.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gckfjtker.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gstwcsvsg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/grlktcmqp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/grjwjdbiu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gilqztgrc.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gyarvssvo.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gyusuujhd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/goxdprnkq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gjimzxnth.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/glapjtsmy.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/goyuezwff.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/goorvmekm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gowyrvwrr.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/ggrixtemu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gkqexbugi.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/ggntfukqc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gsuwxkojg.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gueoxwxyk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gijddlvgq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gppehywkx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gagjisqav.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gguwdoafo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxzqtdsf.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gatavmpmt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gzxvegefb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gjgtruego.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gqcnhnimi.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/guasqtjrh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/geaxbajhk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gjhibebob.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gzcgiizqa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gndixvldb.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gcessftmq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gyzmzssls.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gmksictsd.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/ghudykywv.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gcxanircj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gheffwubi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gkadfqpyb.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gijsthuaj.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gevphbwqb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkvawsvjd.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gdxbqmlqr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsegjhydm.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gsmysuerh.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gwpyuvzcl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gespcdnkr.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/giujroooa.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/glhjczopo.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gaaqbhtdf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gemqhijfu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/geprbfith.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gotedpqis.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdwibnh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/ggnimhhec.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/guzcweoan.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gkrtnpezs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gjxnlstjy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/grenbisej.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gnsbrgohh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gsjuuewxd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/giyxbkvky.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/ggylurjbw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/ghjrfggul.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/ggjhrkwlo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gctbxatvp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gurnzboud.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gpcereryu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gzjvwjbwf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gojohsnzp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gsbekzoeq.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gapqxxplb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/ggcdvbxss.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gowvkaqca.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gqzhjuctj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gmtmakfjs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/guffcefle.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gsdwijhuf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gnorvtfhh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gzfnsfyyu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gggarpevo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gzwjahomi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gwkjbgkvz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gxxjyxkqd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gryuhccrq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/ggznthxlo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gntaejyst.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gluclleej.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gqmglfhys.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/glgzvhoyh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gsluuvvir.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/geguyppus.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gcbgmsfjb.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gazaeauau.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gswbxhjlh.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gfxficcpk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gpjvdlsvd.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gmldfxlrj.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gfzgcppob.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gclveoldn.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gsqbympog.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gtwaejiql.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ggvepxnai.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpdlavsgn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gfctjkcrm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gkybhblli.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gezilvivi.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gsualnwiz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gypiclyyv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gilofcrie.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gdakvhmcu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gtzekwcxr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gtptxyiaq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gamcxssoi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gbmkfngck.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gnfozhoyv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkgmgffop.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gsicdabzr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcdycwzak.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gaoumiaqh.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/glpbjpqll.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gzdhscdri.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gjhegxowl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gfmumeqvk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gfyugktnx.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gentpjbjf.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gxgkmkyjz.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gedensbqa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gmclihuav.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gmrkdcqpc.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gnbplgxmd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gusuiqxnp.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gfbpmrvba.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gbkpyiacw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gggaimive.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gstlwxpeq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/guavglygg.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gfidqefzs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gkgbksqbf.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/goycxwygj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gqasasqdn.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gjtnxydye.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gvzzvgyyh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/giggmopuh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gljljzumn.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gzovwvewz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gyiqwikbi.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gccdniayy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gbqgyxslc.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gpzzmxpyi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/giwzzguru.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gdjvafybd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gucqmoaok.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gzitkggug.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gzaaiznxg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gnqdehavg.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gyaqjhbko.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gtshocpts.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gwbpkpzqn.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/grszifjrq.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gprurfehb.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gyeahkceh.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmvucpwmn.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gxfoofiaf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gbiexdewj.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gxcvpfzdn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gpozwlblh.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gibxsobkf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gflbdzbgk.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/glbiopeel.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gghypxmyz.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gwvdmphfo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gnztvmsqg.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gmwijrkrt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gnezfimdy.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gaatcilwf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gvoolfrxi.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gmestrsyj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gsyzwasph.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/guubrgkqr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gzchfjnaf.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gxtknxgcp.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmmumkwno.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gyusygwpr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcgtrahuo.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gfolcrelo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gizujwlvy.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gdfnvifct.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvcxqadfk.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gzgyltsrv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gdhcydtym.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gttpvzofg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gizeiosoi.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gxtxqblsn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gzgbnrzrc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gmxmaxupj.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gnjnfzebq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/geuqmzlqc.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/ggleqijyf.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/guckquhxl.sHtML


<!-- 参考信息 -->