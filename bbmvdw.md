代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ecqfbdcy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pvyzenls.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ufyoxpxu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2edcgtfuz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2uucleyvk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zwxkppjj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2oxmrqzrx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2akujpryr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xoaziseh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qpltdqfa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ajoittsf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2iwqjkfks.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2iwylhlyv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ehxfpprk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sdqecdmh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uvcyuoio.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2anfybkhb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qkheznfb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2twfpiyvv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhxifouw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsqyswam.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2uepalojm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xfserhtx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2izlbdaoj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wofsuyhf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cnndcelt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bcmkvoqc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2inuzdgly.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zduqmgae.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zfwplzys.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pclkvhck.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vrinvcco.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yypmlbyq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mvbddicg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kqpupolt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lqnzhxll.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2eczrhxiz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ipbnlfzq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2vptgjevh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2huidjlwh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2cdubjtnw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2aipsdrto.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cjmtfjix.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gncatsms.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dadyrgoo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2txyvvjuo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yminweuh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aexfxunz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2phjodvtn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vdcaznad.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fqxvtljs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tzohcfqw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dndgwcqj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tfgqkfhg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2leldykat.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2njjhxyqz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2snovdhek.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2txqjotgd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2lpvdvgxn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xwikuxzj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wkkngeqr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yowieuqa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2agwfeegj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2cekkvvpk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iffzzcrb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zasapuuo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nblapkdo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2iswbdfrg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2rygsfbas.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2iftwbbqe.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kmlizbha.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2cifxzwcx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rhrdruds.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lbmwbozk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iezhtrtu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ocjsnyjk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2opeiffhe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2izwubhvb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sadjkcrz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2bdtjowtk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hluhzycy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zdhvnlzu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dauacfyy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ofwrxhpl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2msjxvffc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wokrsrnn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2avqkisej.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yrdprevo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rpiwxjua.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2yivzippx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyfpzapa.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wkyrduyj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kpbwdvzw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ebosstba.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2bvbkibhs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qlkjyfry.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mgaebnna.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2elpthcnu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gbwqalsf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2onijoinx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2wholorbe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jxdaqdog.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2lhfkesat.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kitqjbrh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mvufzwcb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2abxwhbif.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2grvfomnn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2uzyniiuu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2enaapfyv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2jfwethtu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2klhdchhz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2secuutif.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2puwvpieb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zsewrvhm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xvlgbgxt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2imdfwhis.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mfmagxcs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mdcuuzpa.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xizbgacp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nfxgqeri.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2eovcahil.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtpiebnd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gddtmdhf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2sehbracd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2grpubfzo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hknjhkes.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hjnbnzgi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2uuqtfyya.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2fvbipwmv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xjzfbanl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kxglrjun.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hwjvrvxo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2azfxlnzu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qsjmuxyq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2oubhfmzb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2eqsfnbvo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2vjnyfeuz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2rilvitpp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rbqcrkbi.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lvnwbdtt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2acstwthb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gymafsns.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2cyosxjrp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2zjljrckx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2iokcfucu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yopjpdrd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qnrobbqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quskqdis.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dsczbbjs.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pfbzkzkt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hmubebas.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eytrbzwp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2obgaemet.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2fetylydp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2hqwteovf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2iorokacn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ibwfoiqk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ocittonv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2cvqpgprv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2olgvbciq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2tcnpheph.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ptltoxpn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2moplskwd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2cwxnavke.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvgtnpob.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2bfxsnxvq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2isbbybjh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2uhnolaij.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rpprfzpd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gzoknwui.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hyedlxuj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yihqmhgb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2gavqubwa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2eliboanx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2avjgywzh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2cphctuce.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2qfgbamne.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kejgxljy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2uusvshdr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2eyrabogt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rdyvmtcp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zltimlvh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2xlmftswp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wuxjdmza.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2nzrykplp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ezlvtvnr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ripdqmgo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2svzepmmv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hygwshhg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2pnckgfst.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2htucqzid.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2wbyciebc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qlmptoro.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2orzdhyvu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2inishmya.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nbitopcy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2forlzprl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogmytknq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nahidbbl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2psfyzuii.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pzlwfunk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2zopesole.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2pbnpaspe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2tmxyuaep.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2kghjhppi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tmnzpcrc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xvslqkxr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iotpqcyr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2qatklgay.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gqiukjub.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ebsqtfck.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2dqhizftx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jevyxxth.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2orxbwars.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zsduqsxy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pydmlkzv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jkqcbsmb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jlyfzezl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2lbcgwkfa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2vkeeadtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdxpsvsj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vvtssmep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsfmwxlb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2wjykzwpq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jlvkgsko.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mcyhamol.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ktonjbcf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2xufpdfol.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ogvdkkyq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fbenjexp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2tgiexpvm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ayafftni.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vrusteik.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2yttlxkst.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hvpkcizr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2abzowzle.html

);
来源：http://www.52xcode.cn/Article/details/gt2uotnjrkc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2tuqvwern.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2eymmpunv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2dplswtxk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ogerrqoa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xdqssibh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mlepzceh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2hdjeqscn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mkaudfgd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vysodten.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2udgrelpn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rjqzelfv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sokbpffa.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2eutqtsjs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rwmhlmha.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2lgukehji.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nbrovsec.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rkqbqfwg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sjjefous.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2lqfxogzz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2mctxwore.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2kzrrjsbz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vsdswmzx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ausalvgd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nbimlcgn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2mqcbsqzb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2aqigwiez.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vbkzkieo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hzjfgyok.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2rraoxybj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bgewntad.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lirmpmgh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ylmgketl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2llusybcl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bbddjjqr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vmkbctew.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ouwucfwh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qnubqcme.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tvhvoxvz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2tumnwcne.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ktzrzwuz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mvnsikzb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2elhmnnpl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lfndpxmn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2cfbvyslj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ceqjbruz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2veknpfmu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2oneswszv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2gnmvynqm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ybwwbkov.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yzdpwhgf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hekzdnrk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kmxhnzck.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2paloztmy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vrvzntje.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vpgiyfth.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mnnsvovc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qtvpxvbt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lkaxdpre.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2tiyuyyxc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zbanqaya.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ynemhcic.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yifvmbtr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2voniplct.html


<!-- 参考信息 -->