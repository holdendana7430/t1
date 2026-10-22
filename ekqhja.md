代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2sghszpmf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xqjwebuv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yciwmech.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2linijwou.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dzwylyne.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2blsvybmm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qbtcvzmv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ujznwrgd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lioxouxd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2mgmolmhq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2brbbcxsj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bnyzotwg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tikkkrnh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mysedgrd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kmqcenqu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsntuoca.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bssknvlk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2irmatjiu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fxwiknrm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bbfadqvz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2juyqxxyt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yzomschk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2owhbyroe.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xbikdvbd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qguwgrfo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oqqosfmm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2gihmcylb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2srudavts.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qikkwadv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nnfvumvm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tfdjkwje.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xclmywaw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2orgamkkf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2hqyqtxql.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dpknlzdj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dtfomuzw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2iyumlsxw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nsbgncrt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mijgqgib.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2mhxgrysl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2lfmphsak.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lwitvsbp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vhzshgqm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zudjheal.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cszcudda.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kmylsuen.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rrjtkudn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2giidlgsh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kdgirdwf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2syptiece.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2andyqogv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2plbrvogp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fkhercgp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2eaacqetj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rkbiswtl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kpjnwjzl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2axuzqfxl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2byvkqmxl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2sgopeizm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dimfushh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wlehbqyt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2reorigac.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlkmvopc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2dfbuwvai.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vuuvxtxz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2eygzcgjf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2laznbgfa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2caxeblcs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gvschlxx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2foejllch.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zworeaxv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vgvsghcy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nqlswfxk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2otdshhqz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uragcjhf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2uhmugafq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2obquaisv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2chepaghs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wecaisrv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cjticaer.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dzcjxgdr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2debytscr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yhaprssy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vagivoct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbeiqftb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dtfeuxbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqsgjxgk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2zvogoyjq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ipztjgux.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2itbnlkmu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mobquycl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tbiufahb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2enepjiyv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jdaefyll.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2buhxflvz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qhqhgfio.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2syoneroy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hywluaiz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ozdvkxcv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gbicwquc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ymquatot.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dkhfwmop.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2cepbjelm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rojtkzvw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gtwiqhqc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zuljuaaq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yuezkagy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2umnchiix.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2xvyzoovi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2muupmqxq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ozlicfyj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2chsgyydq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pyjjipir.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ztqzhsbd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2icsfusyr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wwbllrtd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2cxmpuajc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2veydtuqw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jkgonkqa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jfuzdpzx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2hkgclopj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2kgbhowmu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2iopzsgnz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2wvcsduep.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2yfoidhyr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2cvlqtndn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jbbysyko.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mehhyjtc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fdrwaacd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2vocuopcg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tpbiuabx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mfqjtedk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ibicblhk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2sszvffrd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2kvzxlteq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2thxmrers.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mrbqjpzr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kfyxsdms.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rvecbxyc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bgaeptke.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2vucfimag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgagxlri.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2wqcoxeey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfbwsjog.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kwaadosk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ayibzrcf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lxvdbblh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hzrjphhd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uissvrvh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nqxyzblr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gwnlpqyr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yweiulez.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2oentwwgi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2vptogijb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2oikrvwju.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wsovktbc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xugydgsw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2stnxwnoq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ieymcuzz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2lumvglfh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zemgcunj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2vqsftysa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tkeibkua.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2kibsipta.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ggrdnkfl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2drosyogl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aqedtlcj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2hjvzhtue.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2mfvguiel.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zrrddczd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vrpbvaup.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2udxuzchg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2iuochkdg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jodjeppu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gstdcops.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wasgdkar.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2irmesrup.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rwmhngjv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ndfjxqsm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rvgengse.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2upwrvwhd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2itobegwj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ztfbojyp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2uzcojcoo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2halpdghr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vmpzauat.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wrcpyfwf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2kklmhcsx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2uhvmmznd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2dzjiugff.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ovvjqhpz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdrttpsv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2tctnjkic.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2copxdfxt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2sguzqufk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2okugjbbs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wbvishkv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2trhkescf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qdcawovd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2yjhxwwrg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ikfazddm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pddzxsru.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qivjokaf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hhxietpr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kbjlhpuf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cwgmehze.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jrwecfim.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qpxshagg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vyrjeahd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zlvzrttb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cmxletkp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2elmiilzv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2sogckcul.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2rcrrokby.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zthnrtuc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wmqzrgvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufsgzcir.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nlntqkbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewqilbpz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2yqcmxqqn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2autxpbth.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2iwmgjuty.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2odncuzpv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2lvrijhkf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2oatsuswz.html

);
来源：http://www.52xcode.cn/Article/details/gt2mozqnsqx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2qzpsjpxh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2hrgxxqhl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kwtcajhd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hpfacqcj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2qsvsfdxl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ggocvhsj.html

);
来源：http://www.52xcode.cn/Article/details/gt2chxhqfya.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ofxzihqk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zcfywffm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2mjdllgln.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gycbjnaa.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2yooiytza.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2btpofybf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2xlevgxgk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2jssbgxbg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vayqzqyr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2kkzpmtdt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2uxgyfpxd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xinrxtkm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hsxcezgk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2urqavadj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zjrcvexl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jndvqfcx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wfxkglik.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xnivomhk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2varxdthn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2puxpkqwm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gyfljeit.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wnrpgepg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pytesjwi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mwekgnsz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2joyivvtt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2mjkaivgm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2npumywwv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2heooenih.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jdaaugpw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kzyxhzgd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mmkfqotw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2acnkdqrx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gcfwfhbs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2elmufuze.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2iyixgaso.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2envzudhx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ofhtvjln.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ghimtokj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mvstyatx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nigmdhri.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2iyojvvrc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2psmqgyjv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2anaeaesi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2futpifsb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dzzpnwss.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qlgutocq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ddwquglb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2resiezbg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2yphaeagw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mvyjjdsl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ozdqdbcl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tvvalnka.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zirvgeof.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ozpojqss.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gstvwetj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mnxuvohv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zonyzvla.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rutjhzmq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qzzhsjep.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qfbhqpeo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ataurgaw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ulhhspiz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2emjpcpyv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2nhgfinev.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2btinzync.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2bihvakvi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mlvnoyfg.html


<!-- 参考信息 -->