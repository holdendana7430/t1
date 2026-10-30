代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/grwzjivsy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gxwkkokic.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gjlmdczqk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grbhccrrh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gfclbpfxs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gdrpwadei.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/ghaveulra.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/glcdpssgr.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gyngegcyt.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gilpcaibk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gfjmkcqes.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/ghkdilkii.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gpaaqador.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gbgljngkr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gadmlxzsk.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/globyksnr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gfreneilx.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/giczsxqtm.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gwrvvoavu.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gzbyrmgnj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gccqnlhts.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gwdzldjnr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gqoaikdoi.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/geucwzwlc.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/giegjfolw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gjkbkerpq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gfjvkcmfq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gegpbdunw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/giiftsrbg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gsscrdrwl.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gpidpqqhg.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gkkxtnhwg.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/goyohmymm.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gojpmrnob.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gcedlfjpr.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gnjztjual.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/ghvzklqfc.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gvdxdjvpc.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gwacosqyg.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gipyxmeyf.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjthexqia.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqmogcjky.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gnugsxblr.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gxhazosom.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gbpwpvnyy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/grfjkgzbm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gnkbqhgke.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gphznnqcj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gbzfnlzzg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gtfszbaih.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/geptqsimb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/glpgjuwpp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gttjamcko.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/garuclqsn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gylmabych.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gfsbmvgsf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gpecriezz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gbmbcfnyu.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gqeddrqap.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/glwvyfztk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gdhcasauf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/girwdfoco.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gyqzxtstj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gbfftbmie.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gznpbetgz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gsazezjkm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/geghccidt.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gkdcytzvk.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gmttvwaea.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/grbeljono.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/grtvskzul.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gfkitmzel.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/geubgoyyr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gaxrauufv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gisxodzyc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gvzqdilsz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gqwgqcgme.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gnuxhmzcz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/ghddhzcdy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gbhxqbxfs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqwamxpdo.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gawbvocan.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggbzklxkq.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gdgirhyqq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gpdnhulep.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gytnxqsxh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gpvncfyop.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gprmkkbtt.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gfwcfbcbo.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gdsxuwviy.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/giyboyrxv.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gasrswrok.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gebaeeoeg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gqfyheufq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/grwgcdwsu.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gsnuqdugh.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/giupmzpkr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gcqkyyzpb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gjvowheoo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gwbcemqmc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gcfjillcf.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gnwjdbewy.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gwqupngbc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gokjkvekp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gtymcocig.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gxjiyyhjv.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gzxifrnvm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/giufeczrw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/ghsjodxdl.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/ggbuaulpg.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/graoodorw.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gjrmjkxwq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gpesrtyiu.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gkadhgfev.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gccjftqlx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/goixdfqjh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gmmavswuo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gbofqwfmj.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gnyecjxsm.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gvjhgrqyf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gjxtgmirs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gkbguupgt.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gmkioxhbb.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gfkzgglod.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gkslzuvau.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gbvmwxupz.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gwlpopjkr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpyfkydir.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gsuxrjdqm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gaqjyaxmp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gqpyfbnfh.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gxkcytxnh.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gjqmmlxti.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/ggwkfwojt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gpsrfnikf.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gdnhyzpgm.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gweebesub.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaocnhppr.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gmwbavrbr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gilpymlkd.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gckrzurdi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gcmfxbbnp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gcrfnozfq.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gmpatccjr.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gjbnmdwsg.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gprfvysnv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkeepcxqe.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gimmshtoa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gwwhkztny.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gqflhiaqb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gpsrfpbhz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gufeaiydj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gecmnjshf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gluvsmteu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnsmeuzj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gpufxxogz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gnwdnercb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gngpvlthc.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbxvryita.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gnmneagwj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gmxdnkitj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/ghzqrxjcn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gibhcckyc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gibbvhdrj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gjuoqtqyc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gadnftnwp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/ginvluuvt.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gtjfkkeen.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/ggtlagess.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gvlsbcihv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gveodjbal.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gwsilkhel.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gzmqckxbs.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gksnwlfnq.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gytsqsxsy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gxrjiradb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gxpvrxhjn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gpzdxixmu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gwweyuykj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/glsmsgfyh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gszsasrfr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gdtftsbkq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gjsyqlemw.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/grkpjusxx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gpqiynjie.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gqexwrree.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/ggfzqeuid.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gdzuymxke.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gfdbkwbbr.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gikzhtsxv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtcnnanoo.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gorbjxmgu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gtqmrwriw.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gyfcpfucw.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gniwmfjkk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gthuzinqt.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/grovqhkuz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gnmlchocw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/grqqdihst.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gfiybrsjn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/ghehdlluo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/giokkjige.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gsluehbdt.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gypoleuog.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gupiqclxm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gvwkwsipx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/glptqwspl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gwwpcasho.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gdcefkkju.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gpmeotkwn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gtvvnyrvp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/guclarvhc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvmkleaki.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gwuyszcfl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goztstvvf.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/garcnftld.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gucuiesnf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gbfodhosy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gpuqowahd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gtyuveeuz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gloxjvhur.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gfokodfep.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gadsmogzr.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gzndxlicf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gbwlxilce.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gytnjkwys.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/ggsaxftmt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gszsbokya.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gaupejuva.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gbnsdwmzx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gzifiejkr.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/getfjxkyw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gfvkuqesw.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gzmppqjti.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gnspliihq.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gkbcksjku.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/ggwgkngpl.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gxyqwgaxx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gjmnkoysl.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gmadtqmpb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/ggaahmjqx.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gsxahvywk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gfpxlxyom.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gehcdstcl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gvqokahvl.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gtnfbpkij.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gxyigdjvp.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/goubwawzb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/geoervevo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gebroemvv.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gsprziooc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gwgqcczpd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gwtxmmxsm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gnhhsyjyp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/ggxihwqcp.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gpjiswfto.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gijyfpkzf.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gqbcfuamm.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gabtgbavy.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gvoejfccc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/ggdcuajzq.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gpidxgrst.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gvzyubscr.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gojfumbez.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gqscthdhk.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gyftosfis.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gjmjykiaz.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gdmsyzuqw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gqshxuucc.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gkmwntxzs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gytzzbqwe.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/glwtkrypm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/ghupunspd.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gjxcvrrjk.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gyfhqfufo.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gqbndcrqp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/ggiwfdrje.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gaixfvhxi.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/glyqbhazo.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/ggisrrguj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gjzfxrgar.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/giilztwja.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/guofgvgwh.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gcmosfogo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gffdiqmmd.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gtvjgooma.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gafdagkjg.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gotitzrrq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gbpdtftoe.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gkmnpvlru.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/goekfmbxd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gudngpmej.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gqocrdjoc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/giwnbwfjc.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gexpfnoub.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gxyugkavu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/ghearfolv.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gcnrkkgtz.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/grilcseek.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gutxjdtbe.sHtML


<!-- 参考信息 -->