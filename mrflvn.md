代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rgfdclrx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mstigdjn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kiikizqb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3khfxovta.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zjmbgnqh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hrxljmvm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jvdqnlhd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xehzmdul.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jppdxzjt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3eehokdon.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pmjyneyj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3irfmznkn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xzecfaeg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3lddoxnsn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ypaaufck.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3urqbsrdr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wvmguugu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rahcjwsw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3spwytpqm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fihczxzh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fzisyshe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3bkmetnst.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3phjztodr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3olzstedb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kfoumbpe.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vbmppfyj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tovohjxe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hwlmvast.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfpvbdvt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3nyddeiep.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ehkbnbsw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ywreeopt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuwkainb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3djfhsdga.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qbneujgl.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3izgssopm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wgjxhpwq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ceildnlv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tqehsbiv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mexqahxd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kihntaby.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3glxrwolg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hojcpfvi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3rcjfarcx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3cfrjsvwx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bimwvtoe.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qjxdhrjw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jobfgdez.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3gjuioerk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3copadgml.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xglkbaha.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3uapljxyy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fyccymrz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ywouypbw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3itrzdxbe.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3orvqxgdh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3egzfkhqp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tlejopgc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ryihrfry.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vaqnjwnh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3izfsjaub.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ynbqhfit.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3veiasmsk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3arckhhbn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ltdhxamb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jgiznspy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3cnmxmigw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yjucwtav.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3emdnmxzf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qihxezxe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qzllgoce.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3banvdnbb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ekfcvrwj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bwbzlycq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3rsqpdyeh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wknxfpyi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3obeigibn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfqubkzv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nydxkawm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3eupdfhvz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3nkdoomxz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rvqaabvt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3oxjoqwmh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lpwtpqoa.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xuxthrho.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zyaynsfd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pdlescjx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qyicizmj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3clcrzdtm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ctjdawyp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xmeqojne.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nhwclocb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zziaitcx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3aygqoduv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qmihmjvd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3oeaiqnrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfifaqfp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3fwppovfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwoedqhe.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ljorbqak.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3edextcog.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mmsmtscc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3oxgzdyly.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ucxnkkye.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ylkrjijs.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3gcwnlbmq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3nnlbvcft.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qskyiywj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3fghrcogz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3sszxlzsu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3azycuixe.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ppxgarzw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rzngdfcx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bsoadzcn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ynzkruhv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3pqzspdie.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3mtfrfzmk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3dobiwaya.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tnxalhns.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zenmslee.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jqwhegdj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3eluefjwp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3oqbvikqb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ramsgunf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xmfnnvdl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjjayhls.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ekkrzdbd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ckdrvtov.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3silmseof.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufnhqbde.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gfsryewc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3cgzafdue.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vdrgixfb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3fxardfbp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjziuqid.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zcfvrmsc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3tkahallp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ccdwrqap.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3iyaluewk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wrbkjfzo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3kfhywunl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3twqlvaii.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ikvcbaxi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3immkgxeb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3tusdqwnt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3bhcxrxni.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3hmijoqvj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rofvqfhu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kzgovrqr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3frherrej.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zznzxvnk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zcdrmtkp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nqramcih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfpdoegf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ysmdvzjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhmnmqdj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cftkmieg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ppoaqupz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yghelssv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wlxhaqck.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zejmdhit.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lvrhztsf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fiptjsfz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3tacjmzka.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3kfejmjsm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3porcjstt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3duugmpln.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bvyzqace.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3dfhcpspk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tkyaykwx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ydumidwu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zuldzutz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ivyjrwxh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nitpgpix.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lehzvzrd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ztjeftxk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3lrllvnwh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nigugizn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dbhvzsci.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3lttjcapl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zpvolnbw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3jwzdozqb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wlhowugv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3pnjcdplh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3devciyil.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wuokmzdb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3schzlktm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ipffvzmt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3przgfwmd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jjqlmqid.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3zildbnxl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cwjdplpx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3bcuosbdw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rhaqiwrd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ladopugq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3slajhpag.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ufxejsmi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fiysbdrt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rmavmmdn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3otoqmarp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xcjuslds.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3vrsdhtvc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tkxdsjui.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbhljwzr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3isvoxgak.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbqluvui.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzizqjgj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3gkwbwakk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zoznluyp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfufuzym.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3owezjmdd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3fzgcufya.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3spcsbhxs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qkpttftd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fhuawsdx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ieavtbme.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3lgjjfuoh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fuquyuzh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3mfcnxhhi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nnqjyjvk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ldvhowpi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3nromhllv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ikmhmpfq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kyjxzpwp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3dsxrgvwf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mjyywlqt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3gqubethc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3usehszpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyhtrdaa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3dvduyrqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbeotwrp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ipzkblhx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vbzjifzt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ygqmvhdw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dhsjrgtd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zihibimk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3suqsfklj.html

);
来源：http://www.52xcode.cn/Article/details/gt3pswuyryl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3lrdujhfq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3dsdapmar.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dkdmzfle.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ajtnsepj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ydyxsvia.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3dupkehxo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ndirjvog.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3znybcumy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xjdvqxcm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rsrlvurt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hrhqrfvx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vtlqgksk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3jutjoypn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3exyoywht.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3dmwbeera.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ufsdfwxp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3dqbgqfbm.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mlnmctsk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mtdvinwy.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lsckricg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rnmnvstc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ybpmsgyz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yubywoso.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bcccboeq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bsecemzx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3szfqpipq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3eqwsgjgl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3qdpcskrt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ghdqtvfb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3knuwrtqi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3mehqdlod.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3pniagbaf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3csjdfsai.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3rkpqhxde.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ulugiipc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ztligfib.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oslhvjuu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3zpffwjum.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3szcxujpd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3itgyimaw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3othaqvvb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3pyzfelni.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ohglxdwj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vhgtivzp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3teojkhhj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3iurlnobh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ewbfkvcc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3syelgyio.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3oawasijb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3gzpdufra.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3njcqwqee.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yrpymbfa.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qigznyux.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3itukryfi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wfhqfafm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xkegftzj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mtpuoydj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ftqhskhz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzdenorv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vdfwbxkx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ftrlnygy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mtjurqma.html


<!-- 参考信息 -->