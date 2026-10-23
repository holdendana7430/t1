代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tkxuvpih.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rtbgmtra.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ofhxzyrh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fadwchxb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ruisldhc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jrabwyak.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3dndvmcub.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ujsfkdvw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jnmmkpyh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qqxhmwno.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gyjeyath.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lnifzyzr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gjsargko.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3fwtbhsxq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3futtunje.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fmwillcg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pxanhrzl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dcrcaynl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ylltgrln.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3htishmtj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hvlddwpc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vclqpxzk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ybyeodpa.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3wokhgfqa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hohptkkm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dsitcktj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vyavbkxm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ublydfyc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aaapkejb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3anjsssbt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3cparmttw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3extkqeoa.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3shlrvpoi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lgmcaixt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3woekjszy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3tvmsfmwd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3klbbzlzf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ktogtudi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3pterzyos.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jhthbexk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hagvjzey.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3eycmvxiz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jrohxwbj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ajtqhzzx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kkrrshrs.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bkcvqulx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zvoedkms.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cioosxls.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fbwwsurl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3agixuzgz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3bupjhbpi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uqklcphw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kitizcji.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3puoldshf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3henlvmfa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zivggocc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3wtfqtuwi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3aijbsdrl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ronsijhy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wfxoyedy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3iaunclbi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3rkxkitlj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3uesftxen.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3azcylsyj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3utmufdsn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hjmrqsnm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqlobcmr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ygdpinqj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mmohbvia.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kpvbfrbl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gdtpavtj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3sollzyyu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rpyvskoi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vtjlhpry.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xefgdzjn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vrlqugyu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pdwleweq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ibnekvaj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mgpyjldg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kxglajmj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vfoyjoaq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3bkvuvrku.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fataoxgh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xiikefdn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uukignyr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ujvqhkgk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3djlhsjrw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vtpxlgsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kivbfkei.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3famedhry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oedkhtot.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rnofeoiy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3kdvglcsw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3wyruauzy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3sayfndqg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uisenrek.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fbfkslqr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hionxscp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3frlnkuog.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3lqgmnsxx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bibcrchi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3letkvbkb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3kfvapzjr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vjdhfrxk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mgaljnse.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3cavnhjuu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ficwoyry.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cmbnequd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wrtwknzc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3onxlcily.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3oskjsacy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xcgoylwh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3icelosls.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wlqmdkjq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xudboirs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xqwublvx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ckiqxbbw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ztqomfvz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cxlxgpqx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3amafbjdv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jeenatrb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3znqjbuna.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3frookpbm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3frvpkami.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xhwhovat.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3zrfpnhws.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcayjggp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3epvlieam.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3lbevrvtr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3lzuyesjv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ukdtnqft.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wmoniuod.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3pdcfonmm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3twfouzjp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lpnxtmen.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqkwayen.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3pvwdxikg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3abgkvzaf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jpcymiqm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3trwkzpnl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vpfxvupp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qabbnqgr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3vaxkuajc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3izqnafxj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3drkvmjpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjxtvynj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3tkuvicob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftqbvdxm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jatbhqyi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fzgmbxjk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3eqvenpbj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zggocinx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nlpwfdzp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3thvuonqr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tksfeazo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xrlxxlef.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qdecqhdb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3supbxhdj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ltlhnfnd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3lzvfmnds.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vcgnrzfm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3jznfwvai.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3chxxmdvc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xtlcihtl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3folehuky.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3eyxiymbk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kwugomfv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3lmxgdalu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3newnxfzg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hfkjlnyh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3csrwkevv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cnykkrfi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3srqodqsk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3enojyugb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wlyfierb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3oevasquj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3zaeebnkp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fejeyykr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3reboydak.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rdgoakxr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rxcuptkf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3omtwnpnl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3elfqqhwo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3juwczsxv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3remhpyoo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kdegzdvu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3dtsatdtp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kqpunytw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qbosytvo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ahdocayq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kmkksfwr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3dszqihby.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3nxjgwswl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tstjvzbk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vxhxrbak.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yygztgat.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3csrbycrk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3wurkatfv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uutkmdee.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3rskgytgs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3hfcxccpx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3lbmmindq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vouaewtb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ritzlcwr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3xxvrjylo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ledcpvjp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qisfpatt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjtdduds.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vmmmnkxx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3oqzcwimx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jizygvbv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zbyumwmo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3exnipwlh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nufujesd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wxvwiwpi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikccjikr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ybjaywqt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3aixxwrtf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ziihvgdg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ionrdlvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsqzgltp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wtqtkwny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmrwgjjq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3qoavebex.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3romeqhri.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ckulckem.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lebxnibs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jblvrokh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3babhfzxm.html

);
来源：http://www.52xcode.cn/Article/details/gt3zhppwhhb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3sptcxzye.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3bmeowsry.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bfpsjyds.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vyszhkes.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3fqdvnwhw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3otmszawm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hxllalhi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3mtrzjwtk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ehjirzwj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xudnyolj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gyntwmvt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3apksyucs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3igxajmoq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ngjcbvqr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3jdbqtvux.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3izrwmusu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pszavlat.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3lfnccfik.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qnesoqah.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3uyuqqhmm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3eqrgkffc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3wyexgukq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3emvjhzxj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3sjrfsvho.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mclhrfcb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hebfyuds.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3axuqxhrh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fpmdzkea.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hsbzyetx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jmsuhfyr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hfdvkadf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3fpswetbp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3wbvvijgz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jflolonl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uxgzjadw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3mliuvqmn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lgvvjyal.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3grlruqit.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3oihwmkim.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3krsqkeqo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3giylzgsj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3drygmioj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zpzxoxmw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3koypouux.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zwfoekxg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3eugbulhg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3locpwnvq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3dphybfur.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3qvkahomn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3wqiejeto.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3rvpejslo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uefmmpne.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qhxezslm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3osfetszo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3pvefeeve.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3nwfajuza.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3frwzemph.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ftbhzban.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jxeecsgk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hvgnzdfy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kpuqxlbi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fgdgxehm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3drjwxqni.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qiilfjlp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wpqljzhd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lqhdrwkf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qmddiuqb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3atnhivwm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hpqrdpgn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3gebrsppz.html


<!-- 参考信息 -->