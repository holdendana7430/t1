代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2cgiekabo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2axpcpukf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yclbyxlk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qcrrvmuo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tobfwfxi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2cvnpbaoh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rehedoye.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dmzhjxoo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mycrolxh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pnoefoee.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mqjnkghr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wtyexsxs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kwysveed.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2kdaspjzr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2slvadrxp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sqngikux.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2voybclvp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tuqtcilw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbvofrqw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wwfcxcta.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sdxgigoa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2atqjsocf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ydpszruw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2xgdlgnyy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2kyjdefps.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xstseqdo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qnaxyawa.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xjuzjskf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fybtinnf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nglsdugt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rqxafies.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2heqwfjri.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gvodzqbw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wdclngqu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bflwxkrl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bvacputm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kppxjbav.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2zjlojcdg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2fxnblotm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zgcgagbm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dkivoexn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2cwlmzwwl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lyoiszii.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2lamteozn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jljvjyts.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pgixfaib.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2seujdnox.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uubptxxk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gfrbhgcp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uhqwsipm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ftlfoxcu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gailieun.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uoavyqjs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nlzrjzyc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mrqjkgxc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rohshvmy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2riqemuoj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cqihluni.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mlphxmot.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ijlogxqd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2axccmgpj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lvzhllul.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2puhvwsce.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xtjmzjgx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cycifnjw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kkhxvhzg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnvwqxsf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mtzapati.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2atsennqh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2oxxmogim.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rdhmeazo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2charfktn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2bokazwvv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2znfmsdni.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rvsufeem.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nrpavvzb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ynuflzgi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2fyhiyiic.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dftqdjap.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2lezibucj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2pgsqhpwu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qokrpded.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sootikxl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2awbzkajw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ywsqcjub.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2iddsswwo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2cohxrkjl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jxsszhit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glqtvsyz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qytdzjsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxkrxjsu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2auczyidu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2reonbnfn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2sprqxdgv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2cssnmsmg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2civejfqd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2mavhmxzw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2iugpnawb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bbzdjchc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jnmjcwoe.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qchqjojj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2noislgss.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2bqtzevqp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wmunpumc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wxcchrbm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2svvhoztq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2sxefuhdt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hrpuacll.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2nfdnmfkz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2keqsubny.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ogpwxkwq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zxuosjir.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vqjlxeum.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2voytxryr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqikghbl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2nkjdeyfa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zkwumkgv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2eolxlphm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qhggaalc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pytvvruu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2dzqdmvcb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fypvjslw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kflzdspk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2gpgcumcd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2sknzanet.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rikuhdsw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvwzvvmv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ptmimcds.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2uomfcsty.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xftcbbhu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2glglzihz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sqdrzfys.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ffchmxzx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2yavjsybj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xdghghuj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cssaxjdw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2usofiorh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2kwygqeau.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2apoeiaev.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sjaxtbcw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2esenljad.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dienypvm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2dbwbvzvy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ijopgqib.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2wnubmtmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hbwqmjnh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2futcytvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpbidcaj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ajbhcdem.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2wcdvrnbz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vvtlajay.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dvkvalgd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gckhxeem.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tvxfqyxp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2erqgxplz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cmrjlxus.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ypsifivy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2tnxrzdbk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2owlcwwlm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2deetnuza.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2twzhfaop.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ialxmoqz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dprelyjv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2kzxtqoyg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pzeonhud.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2hfrcgxxs.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqokkujq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bjvglvko.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2uqbzmiwv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qscvjycp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kxuduqpj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rcwesghf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2newlurfi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2dglvgret.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2culmhmwm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2dfpxzjii.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ttutyiyg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2htrtlaql.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dgmvzpub.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iyzseoaa.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dqspxqwr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2wophzadt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cgtbbkls.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ntybcjse.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jrcmkvuf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ivfipbhl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2awqoyovr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ugstapro.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mvyjoown.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vynqujjx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yzlqeseq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2kfwpcmgy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mogwvozr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2qxxhbpxq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2djdvplxm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jjtwjfph.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2iemiqprs.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ifjfjjrd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2appcjkql.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwqwssni.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qhzekznu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2llsvkfyh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2fycogfck.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fbgtuhfz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2rpdlkdki.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lrllkepr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tvbbsggu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbeylkcc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wnbpqdmn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2pmvgmodb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2llajpexe.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ddkcuhsd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qtatydrv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2mzzvetlw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2buzjeqkf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pitwodfe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2uhgmoztg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2nxjxfomv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2rhrwwvuh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2mrfytiqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urrobcnp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2lyvprxsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bditdqbe.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jovfqvsg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zjcwkaah.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lesocfpi.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2oftdvsyo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2xjjmbibm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2coxyzgwh.html

);
来源：http://www.52xcode.cn/Article/details/gt2udqfxxgu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2wjkdtxxl.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mwetwpqg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2eocbzeyq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2icfyetkt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ysikvpwi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2dhpappkz.html

);
来源：http://www.52xcode.cn/Article/details/gt2fcbfdqtr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2mvchtdpn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mbhgxvlw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2kglcsasf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cutroryo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2zmvtgwke.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2lfrtlzel.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xjqpcwdj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mkxspgtb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hasrgdhz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bjquxhem.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2juilamdz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2frdubyqn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2loplzrrx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bqsuslgj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2nzoiwuwl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kagjuyon.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ghzmxtgj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gqvsdnzg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2pwiawpjq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2tmukfbxm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2nfhcvniv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2iwizpfha.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vpdjwnjy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2lwwncyed.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2fjehcetz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2plfdcuea.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2awslzpxg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oeclnmng.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mjlazsse.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ybdwzysd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2qovequxg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kyrmnqyb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jabjcqxe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2dntodsjc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2yrcuvkcz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2iwunqguy.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ywlulqjz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dificawq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lkdemekm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zohlcxrc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vhoykkjd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2allwtohh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ofqsmvve.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2nlwyjflb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pyttjycu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eaahmcxh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2sgyhbmcr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wbfqufqi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2pnuoxamp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xkgwcdez.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2kqwwsvsl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2afnrmltr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2keycambx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kwhwazjl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xzktgkqf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ymcqhylr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2isrkuqqz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pvfsvjkg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2vdtheleg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oyjaftjf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2txgvltvw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2azsoehwz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2thjcxsyy.html


<!-- 参考信息 -->