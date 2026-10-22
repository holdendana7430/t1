代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wjjnkmah.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zopczqcx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2offjjjxn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xcfiswem.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2adtgbwzl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2swpejhqu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ebxybahq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2esqwxzqw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qefueeah.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtjjopes.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wdhaxkjj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pbsafoxd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfirwjpa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2feoxqhej.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pivxahgl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2owosucqf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2khpxtfca.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nlluagmp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbhwvfum.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zakcmjsx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qtmqcpip.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2tfwzydxc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hwzmyryc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fbueccih.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vegcepaa.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ynfyckpu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ftrlhvys.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2femnkfex.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2phmdbrjd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rjmfxrtw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pacatafz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ucjqkhjn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ggeaowdz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yoolbozs.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kogeyive.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2aqjhmqvz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mcikfelp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2pxqzjhjy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2urobthng.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2rvkjwwts.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bxspwotk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ftwthnsy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2lgukdacm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2eiayiwsq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jlwwwtjz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ypplebmw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vxhuuhvn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ixvjwayw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2utfhjnbx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hnrmsnwx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rgubnyol.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jnlmpzwq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bdfkpmij.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dfebsnvt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2efquaytn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2snkuqwpm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jnkipuky.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gtnaqpyh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mmbctxsd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hktrlsll.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2pztveuzv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2khpidbpq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2iykxwvey.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lfeobzjf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mzlruvrk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vjbtpera.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2priijgqo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qcciyfrn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2rviargwq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2uzkonjbq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2rbmdqqpb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2boatyoqj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zfuyosea.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uahooqla.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hhkoeotw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bpmfiueb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2saahuqqk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2bzgbdepc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bdxdnwpo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2lojniyty.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2lwqxofqh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2jjzlwwzh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gpnvvspt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pljpadcj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bwvhfkrj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2yvlbobhz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2owqwamtd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2saibnnmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hihclgnc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dnlgxzax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxxjvijf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2nqehaaph.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lcpghizc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2drzqnqqk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xwvomojr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rkeeqgch.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ykvafhwq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jucpxayd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2nihfkraz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jwmavsqq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yejyrcri.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2cvthbejp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cyokgynx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gezftdaf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jtwqppha.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dphhhjcx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2oppbslju.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hfafmyks.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2iinrqtib.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bqkysfum.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jdpaoqxh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ahzivugr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ttpwrhvz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ciglmsih.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmsjfczj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2xfilooak.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xviheuli.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zkwwjkbu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jxfxleqj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2bjwoagbo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2cilmkwzq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbbdgiix.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifvctkoc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xohyiuix.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2txjuwrsg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2asvmgasz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2xkscrmun.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2fwxpavmt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cvmwsjzt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2rijgrxsd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qlfullpy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dhsvsslg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mjgvrddh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tnywmbzk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2szubipiv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tecarrma.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2kqmtoflt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wphdcvih.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2onjwgelf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2juybwkwb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2iipdlgao.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mmomvkzl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2avwqalhf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2nsfsijpz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2zagvvbhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iiowcimf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2laiimebu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atmvkxxr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gozwncwr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lphlrkpk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ufmjicsx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ogznqpmo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jpzraysh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2vdwdyilm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rhquorvz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oaaeolhp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2sczomhug.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2pxsdcrns.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2gdxevnze.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dvysfbbs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2prkbymms.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2syihnneb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2spigicuh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ukstciry.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2jqrrojvx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hnmywopa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gyqzxdep.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2yanmgdab.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2usszcjfj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pprmnzcc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mdfeqvqa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hmyrdycd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2afemxsxu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ufedetxw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wqeobjle.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2uyncgprv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rlxyoozj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bfubwmsc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jlamtpns.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hyxnkfgs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jinistfp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nougvkbn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ypqiazeq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vycpdjto.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2axhxsyxa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2tsqsocin.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ftojfcvg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2njrambaa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yrnnobwi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2btzovxee.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xcoqfiog.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lbcsabdu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2cdgzkwbj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mdctjycb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2dsgkjrgv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vyzsneze.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2zjhhhrnr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2jqlfmosk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mxryvapp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2glflzgps.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wfyqvqau.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rwjytoey.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2sykxjxzd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2obqpufnr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ixqcfsqr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2msnkvurt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jqsufjdi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2smteqfdi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lvfjeaye.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lysuahue.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2keutwurk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2tursydhd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2caxdpfmq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2doiponar.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2kldoxzzz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pscvnhxg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2kxidlimf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2humnpvyw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2dsccirsg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qgguvbhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aboyxdzu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bylhrwaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kljmrsmn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2dqdxouyx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2kehnwikc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2swojzped.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qmksvxzx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2fsuauodn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2cpryuofc.html

);
来源：http://www.52xcode.cn/Article/details/gt2vspixgom.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2dwnnfqva.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2atylvawh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sykxfuic.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fuxsmqyt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2amnlfpsj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ugydwcpi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2urcwdcsg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2sqkghaod.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2qjtmkqdf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kztmhsea.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wmnlsfsx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2pfzzqzza.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2vxuqnztv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2wgdvmjmu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2aaznforl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ezsybrul.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ogyqrajw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2fytfated.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2puxrokax.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2porgiemv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kbqkvfeb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rbgjyxxu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kmujaens.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jznwszip.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tfmtwnnq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2krsgxcyd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xzhihzfw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2zchyslss.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vhesdeub.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mrfnybvv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2mvroxgqr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2kngurvvy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2czdnjmfn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2swfftynx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ipfkfqgq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2pqsathyx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2muhqdikm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rwkwmkhu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cavbvomr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gpvtmvpw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2merjkrzx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2kmjicbbw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bsaqjeqn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2anklfawm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2uopdsqmj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2bvzaabta.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2grlsymsh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ljyinlks.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2vzqtfxjj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2szdyxcsv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zckisfsh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2kyrprdol.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gsmrqzpq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rlkasdtd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2pcdqfqwn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qndldqfk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sntebncf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2nrwxboqq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zedniqbp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zlprhlcq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kjukbuig.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nhjikgak.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lnlvtoxc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ywbnjvjy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lsdeyeqz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zszqkpun.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2plkseovn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dfpxjrpy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2naoexueo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wbylizdl.html


<!-- 参考信息 -->