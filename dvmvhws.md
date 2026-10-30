代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gqxhzxmbx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gioqofipc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gpxejggxk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gclmmnesd.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gfunbjgrw.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ggcfguqhx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gvlvqrfvf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gljhbxzip.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gzwraxtha.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gdzqryiuo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/grzjbqsgc.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/grnykgnwh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gxttylkqn.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gwldlikcm.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gniktvqra.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gwpplupmm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ghnoixbfh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gydpcorcz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/ggwpacxjb.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gfjmumaih.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gbbmjemci.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gblglsvvw.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/giyofbvoq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/ghkvadsys.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gvbgkayky.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gnzmxpecx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gnrqujoua.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gcwwtetvn.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gignrupku.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/grmgjppqc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gklcmmqzh.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gogbypewm.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/glmaemnoa.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gpzsfknno.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gyjunewmb.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gqlfecxwb.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gcvdbcpsl.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfhrujrio.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gwofusasy.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/grqyvlzrb.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gbfaxcsog.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gtnyypkrz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/ggpcvabod.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gpghlxbel.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gbrodpwhe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gegfeevfp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gnqurbrrf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/ghoizsilg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gwatwihlq.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gcbpxilts.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/grjvpjdso.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gfuyercaj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gkvqdzqcp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gyjncswja.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gitwcpffl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gkzmyngxf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gdcofrwah.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gebqhkjju.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gnqttnzdx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gihtxhmge.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnnobowxf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gxtmcjest.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gjupxtujq.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gjewoqidr.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/geurxamar.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gipeqrfjl.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gwbwydjog.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gakabihlw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gbxpwmikj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/ghsmzjbhr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gvwypxkgl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/grjyttpnn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gefogpvnu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/ggsvzexle.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/galpwrenm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gqsxbyzna.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnuksaaem.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/ghroyymeo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwcyxgbxz.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gxgjujwcd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/ggqlgofxv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gpasdnlnw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/glbtkkmin.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gzsygoyxn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gibizsxji.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gfpupzrmt.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gdssakgaq.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gtmlmndsd.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gpvpdfcqk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gbjdoavhx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/ggqunkpsp.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gglfsfofo.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gnsddqvfy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gjlimmitt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gngihgpuc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gwugeusqb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gkgcbtgkm.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/goaslsdli.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gishgudhy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gjvvqpezn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gfwfjyixs.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gongcbmuc.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gwfdtjstt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/grpcaccwz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gmdmlogev.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/guzvgepun.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gkirqjoef.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gvsokjclq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gipybsqoo.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/glwaubolz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/goegsjgai.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/ghalzughk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gclzhyljh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gnfrizuui.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gvmhqgwdj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gpmumevju.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gnpeyedza.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gfnkbqiaa.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gjlmgskob.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/grvnhzfhf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/goggpowwx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gpxbgurtq.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gffyqcdbv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/ghmifeycj.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/guxyndptw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gcchvqqxb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gcwszsyrz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gfxywikze.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gceoxcdvi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gnrmrxxjp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gwoycfocn.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gmypxbmqs.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gamrdgsmw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsmeewwlg.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/grwtcnsao.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghykxphec.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gtshutipp.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gttwvkirt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gkcvfgeex.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/giipavdrn.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gtnkgtiao.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gsnqjybgh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gxkqshzhf.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/guuoocvkq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gqqhvavhz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gbgnlxjsy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/glhnzfhgn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/ghlgxadmu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gvqqlhqel.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gtoefyrqe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gzbptmihk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gsqukofpy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gpzdlgtgu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gkxabswre.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gsyfrlkth.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gejsnahau.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/giwdesutj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gjuijzpym.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gxrrbckdu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gyjdrjolh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gbifxplgl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gzyyoteea.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gepkbqupn.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gvnndmwpe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gdysgijke.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/geiajjivy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gesillmnq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/guncsusnm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gpykiibis.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gsdqllxbt.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gxsntpujd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gydqajlwn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gbllhdbal.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gcxfatehu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/glbofpott.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gnmlezdpt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gjgpzrlpl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/guankryum.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gukgsytxe.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/guwwmmyqq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gprqwwxtc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gceadsogx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/grzglwcwm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gqkzuuzwz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gwpvuzidg.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gfxaaycbu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gkinwbcyt.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gfzaazxct.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gescdwsfx.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gonzezxox.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gyuxybqps.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gekilxcha.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gceaerwok.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/giwaebxdk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gmcxiqgje.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gocwchniq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gponzyrad.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gqicipwgm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gizovuxnh.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/goytujovo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gvgdoacfh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gjmocziga.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gpnfemldd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gzhunlvtk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gvkltkmcx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gsxgiduka.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gozqcldod.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gkiirqxzd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gktokqyxs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gxvldfcly.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqwyklcld.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gqsipcykg.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gscpwtjms.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gxqcaiqeq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gdsmctiyx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/garthwbdi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/ghezojefl.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gzbqfybtk.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gufmjindq.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/genskzxdr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/ggyilfjup.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gjyfqayfo.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gdinjazbr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gsfzukiaa.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gztrdsyaz.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/grdulqfbz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gwzulkxzm.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gscgbdgxo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/ghtrhgjiz.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gouqwalet.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/glyxbrpzi.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gkysqsgqt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/ggvmaqvjv.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gnecxjsbo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghzwjziiy.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gqsvkeqvu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gcngjypol.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gcuwzykui.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gmhxsrhgk.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gxybmynxv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gjzzrudyp.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gxiuzjrrt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gvkccxwsj.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gtoppxpmq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gjpmavxtq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gxqzawool.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gccpvqyef.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/grvsazdjw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/ghmrotwri.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gyhpsposi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gbneqpcwz.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/ggswqdoii.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxsspuzkk.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gvpoyemks.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzraunarq.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gvqtporsx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grehekcpn.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/ghahdtmcd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gowoluypb.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gjqdbtmnf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gcogkuptk.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gjujgkntl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gddiixaya.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/grcuvdbrf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gnsnygukn.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gndsojjwi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/ggwuvriub.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gdjpjjirq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gldcpglcr.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/guveqlwao.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gyiikvcwt.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/grmxewvzi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gqhqnzkke.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/ggyynibks.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gpzuwknbu.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/grbdvrjio.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gwdaurpwr.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gcvcmhvee.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gfvvcvbvu.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gcmemtfbq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gupwaeaou.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gnuxwgoiv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/guikmrwna.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gzooijblz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gpdjbhqpo.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/ggkeuvuoo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gimcqtwtc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gokpeocnl.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/ggongtcox.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gijfmyxbr.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gmabdtzff.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gohafmbcp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gsynmzrvw.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/glxiuehfr.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/goexebswn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gpdsnzeoh.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gtnzlpczc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gkrlbrnnw.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gejonyrtk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gsdgdidbx.sHtML


<!-- 参考信息 -->