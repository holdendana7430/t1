代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gsdunthlp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gihqtmxqb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/guzjhkmhn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gsfcnbyll.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdinmbbwe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gasaqagmj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gpzmpuror.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gugslglcy.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gatchbjey.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gpukrqecx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gfselhwtu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/greuwczsj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gzyvewmpd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/ghovwuipp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gnysydemr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmigszude.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gbhmxppkv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gebymyaey.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gmbldwnzz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gfwyaklmj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gxvvhfvfw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gyaijswms.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gzczstazi.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gnzqgttlv.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gydxhjeaf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gdclgaacd.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gsyrltpiz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gcpxsmpfv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/ggmpxgbtt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gvjxvggst.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gycsplvee.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gjerdicoa.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gcpwaujwl.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/grzexqeox.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gmmljlehv.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gxeeajwgb.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gucawacui.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gkfednyto.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gzlfuaukw.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/guxzblssm.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gwimgjutm.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gdwlrvcgi.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gwnzaswfe.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gjdypjnzo.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gxjkidynt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gzthichqd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gwsaxfgku.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gyrnqyjqz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gmudlkzyt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gjhosunns.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gpvfjiddg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gfvfqzhad.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gptgflnky.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/goxqokyci.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/grqglojep.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gsxwcvxat.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gqjhpnqus.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gadswwhkd.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/glycpqihf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gsilduvmj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gsiuiqulq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gmkwagrqx.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gaewdqlcn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/ggijqpzxb.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbmoptart.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gdityymmt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gulkegath.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkfvalfup.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gnwrrtgzg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gzresifcy.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gerrlunaz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/grtvitbzo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/ggvgpmwya.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gtyzjxktj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gydiukylv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/grzfhpgtw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gwbehuupp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gaupmwiyd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gjethezdn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/ghwzwspte.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gucmexviz.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gnkpldyyv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmhsqcqxa.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/ggmyhrpyb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gucpzhegy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gxenvimzg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gxfrgvxaf.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gbeigbhow.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gtnbokprx.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gyxivshwt.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gefdmcwwm.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gvexahiok.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/ghyfrvbnw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gqthgluvr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gkasthitt.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gjbfeylsh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gwecdfnpr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gncosnfim.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/glcfrooff.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gackrfgpd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gbmetypue.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gznxccnlf.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/glomoglbi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gkbhvmrfm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gvcgydwwd.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/ghhfizjat.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/ghioykunk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gabbfvjiw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gvkdmalxt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gxcjnlhgp.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gzkazgzit.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gergvzyjg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gauhnwbtj.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gczboypqm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gguwxkunp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gjhaprnhi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gvtaettxj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gzjpjuxht.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaiojklza.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gngljfgdr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gxqgvytif.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gqvagnhca.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gevsktqwp.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gihyngjdh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gsjxmcked.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gxvddonbx.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gjjrdrwew.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gehtwhyrr.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gjgecftzt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/ggqjuflhl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/glmpbipcy.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gbmllclnf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gfogqtesw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gaienvxzw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gevwxostw.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gjdbjuipw.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gclazxmbk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gubavhlkr.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gdklzwcdb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqpdttfpn.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gjhuozbui.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gxckhjehp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gtkbzpsbs.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gftkggphf.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gjebyjikf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gzjclfnvg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gbnpcckxy.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gdmrjclqr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/ghcuktejr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gfjremalp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gbgpwrfnk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/ggctmuvjw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gahwyguvv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gjsbbebvr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gueofaclc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gmtkblgxm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gakkdgfnh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gfdaajkxi.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gdvuqiqwr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gagfsyvcq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gjjajaeia.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/grzhxfiex.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gonipgpct.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/giftytevk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gqnxfrirk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/garvdteyb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/giungfsrx.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gzcbykcpr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/giqniatck.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gprynmgpv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gqtgpxxkf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gidlmbcue.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gvfnarhjk.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gwjunvsbr.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gehfkhzvp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gfcqtodgq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gowihorjv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gyiwhqqys.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gcbyzhfml.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gfxooscah.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gfgazgysg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gknfdxzuc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gwpixeufp.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gjraocxmc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gcaahfihi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gwofdnpjr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/ggrqjjsbq.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gqtevwjjw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gysxpzoas.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghjxttrcn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gtzomrsrp.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gmdvblvxy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/grenjemto.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gbxjdaqfv.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gvtrqzcrs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gasqkwrtg.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gixytsnfb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gyovlgrmq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gpayoxnjt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/getbovoow.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gotaoxnhj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gzllsnejz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gbclmrnkj.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gkhiuelyd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/guafgfcib.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gnsaegaob.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gjmvqvjrt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gokoqeitu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gptgxggyb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gzusocwus.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gxvnkqeov.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gvkkwjrga.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gamvkysqq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gghlskfig.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfchqvhbl.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gxsglpmzd.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gsxsxrecv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gibtkjjce.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gpvmycvia.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gnczgczdg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gjqvyaehw.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/grgqomqda.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/goabdqbjk.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/globkxgkh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gdcknhqow.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gfywghldj.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gvzdwxmna.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gloqcuqbk.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gmwwwaxuo.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gpicpumap.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gdjkoucfi.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gftbjbzwg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gwuvuonid.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gcylfwkuc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/grqlxpeqa.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gcwfkpkbs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gzpxmwucw.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gntqzzajw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gnldkhvwh.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gzxesajdj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/ggzqkskuc.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/glvrwofvh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/grgujktcr.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gflqwgntf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gfignikch.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gndfmsinf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gwnbtpzfo.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gkyuzetpv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gcjkvsgao.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/glfooydbs.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/ggnxfivoi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gcopdpqtk.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gmnbothaj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gkfbqaqti.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gvwqeomjj.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gkqvomqyv.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggmmwbfty.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gkelmfssq.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfkgowmoc.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gjlmgzwwu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gnpqdiroy.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gosvkqqgd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gcwlunwnf.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/grsdopuuf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gnmgdsbqp.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gdpfawyph.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gxpqcpjvf.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gpylvcogy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gvndxnaut.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/geckkcxbv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/guwzxhvxc.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gprcbfcnd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/guczfqbxj.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/griehfbcp.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzonirjmi.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gtgwibtht.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gdmobmgsq.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/grfjjzihd.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/guuxxruca.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gjmczgdzn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gendchxee.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gzchljstp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gsjwpokrx.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gwkbdzyqz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfgdderyh.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gdwxygimi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gzrqpfbdy.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gztvrezqc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gaphjvlwc.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gscshnfwo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gzwnokagd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gmzdmqqfl.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gymtrnnoh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gmsobvklu.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gybmzycyh.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gbneglwbb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gqopnajpi.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gwyotoxcf.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gxaxamgjf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gzopoxefs.sHtML


<!-- 参考信息 -->