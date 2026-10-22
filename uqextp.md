代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2pszmurzr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ukqlozmw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2aepsshdk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2viokexzu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xstptytb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ponwuiuk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tadosmam.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2xgkzhpod.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ernogolq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkkzyqdm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rvhzyphi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pupzbhqz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kisoivdh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2kvtcxtdp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cmmjmzfb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ibxgdavk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vkhfncgv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2niqrjddt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgnfozma.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdzgprua.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fnatzevj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wczjorjj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jpaaobge.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cluzrcyx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2itsoyqpd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cjhndxat.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xyaosyal.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ajzuyzby.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ymqukrej.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lvykpnka.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lnfakyxy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mftlauns.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2drqwdwod.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qbdrpjaz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2frhpaeaq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wwurgibi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xuoczrwf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wbwendir.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2jixtehes.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cqltbpse.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2tneasybh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ruevtxiq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wykewgzv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ioauashq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2mtckrbpa.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lhcmdszr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bprhoysv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kplmnzcc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vbmbcsln.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qqwjvvjv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2xffksnvd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ulobkhkf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2urrnepkq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fudqjwyt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zfpczzli.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qirncrhw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hzkuvvpn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2czxggapf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xgvgudls.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wjqmonko.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dasvtegu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2tzzfsatj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ttdluxbm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvrkyklv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2tirqiqtu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gxirdbty.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndahzvma.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zmngyhbd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ujpzhavy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2djdvyepi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qbvbofkp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ybpbnsti.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xskdgpqu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bfsolkck.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2puhbbnvn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2btznlibn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ldfspkbl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2wxdtficd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2awevchqb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2rowmjcij.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2yjsahhlo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2orchrlty.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pvapsfip.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2clrkpauz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uqipvcci.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2eyihzauo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tqbymjzz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vidyumpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spmzbnra.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ksxgvqke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lufueazp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2dqsuscbn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2izfaznzr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qyrimsup.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2veckhfxv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2akszzgwl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tgzchypj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ztogorjp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mqhvzbpr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ztdjkogr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2srqkzrno.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dbcwjyrd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2zdjlfcoi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ubhlhfvy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vjzylxpw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jaegyfgs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2uibnsqpv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rfsercla.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2adascttf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ofjppnvy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2auxbwemb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lrofjcip.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2panaspws.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ftgyjhxh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bqsomvnd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cbepsllm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mdplhonu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2aadytygv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2orawoyne.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2rbhlqhen.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2gdutovme.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tptbdycy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mutgrtuy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2iinpdtfr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jytqignm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ldzlqrpp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmoawket.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kzggxnxl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vhpqwhic.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2evtbsung.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pygxsxty.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fnjxflfv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mecysuos.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ygpsxkmv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbeeqen.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2hfbsnaqe.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2nqllfrpz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2unkitknn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2gfptmeej.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jwbpwnpm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pyhookpr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sdotcggs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gunjotnb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2iigztuno.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ursuuazh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujyaibrq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2lpkkkhdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzsejgar.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vbvmyrdh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2kfdqccfj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ieskihnw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mjzofveh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ncdvuhtq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kaofpzkv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tliftvlo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dkysgwvq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2rqqcdygz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2wmoqpifh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dsddfwfb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2hgiqxhiz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pmdnpmwj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2hyipelol.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lvhxziqo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2sspdxrpy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aimgykle.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2woplrtcm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hofxuitg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2dxdyrgup.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2svlsctat.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jdjgutyc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kpnfcnic.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wyarbtfl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2iifpsmgd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wweopyyw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2divkdmdv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2eawqjlaf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2zyqknddo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2muogaveb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nwjfadhi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vlzeyqna.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2taiwgyoc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2bsokcofy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2psptdrpq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2oinvjuvl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rmagwgdu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2lobffwir.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2iejnbxov.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2apdelbkv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hcvofgoo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2awumolub.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2orzafcne.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2bogimkih.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2dkvcoqms.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hfctoucf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zjevodya.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2abyjsrna.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2coxtjggs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aryqulsy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nprejmbc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ceqdebjg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zuaghsux.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kiomstgn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rrfslwzo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xlckvcec.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jocwuobq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2knhpwjka.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pyrvmhgf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hpphacoh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2dilwnsim.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2wcawiquy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2obgopvml.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2chenqeff.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rexbrxok.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wovjhqnx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tcjiqorp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jljrhlld.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hpkxxrka.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wwphmpog.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2gknjupel.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2umthwpjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojxbwlok.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ydaxenyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sykqnosc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vnhsobtn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2icsifabn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2txiwkghe.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2cnggmxme.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2cwmmvjja.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2eklmhbfb.html

);
来源：http://www.52xcode.cn/Article/details/gt2kvkumbpt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bxxgfnmu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2hokngtct.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dlitbmjt.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mvicqdnd.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2qbunxfjg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2uqtleywu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2chexgnyz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2dyppmcat.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fwpqqdrl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gkadvtao.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2vmoyotrr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2bknuojsv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wfozpdgi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ymxjwmng.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2vtfyyfjn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ktnbrpxf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2nxazrnnk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yziqvqgg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gpgwbtqt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2wrydquar.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qdxwddbo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2uioranju.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fpygycdi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2xvfqtqka.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ystpaodo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2upvjegrt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2mwbdfehh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2suknhbax.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xzxuxmfq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fvlfralr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ycwoqryk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ckrrzuma.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2gbfbdsmg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2cosfrydw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qddigzbe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mofauyfz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lfyanpfy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lvzbsrtq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cqokkppg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2bfwuraog.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2fvudeawk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vserayvk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2tjitzuqo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fmmwhcrz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2njwowwzn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2syeaamnr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ibdgyfee.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ttfevpty.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wvlsumel.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2evsheost.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2nfeucwmy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sxkrrpbh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fkqfswhh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ghingcqa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2farvecac.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2oahupngk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvcekvxx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fetntrim.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zonncewl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qrmmpink.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2izoaszgc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fbgvntlf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lyrfqeaw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ynbzqxbm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wzqmujfs.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vpegmfmz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wlzoeemd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2sqmnhifh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2phalcfor.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2hhhixmty.html


<!-- 参考信息 -->