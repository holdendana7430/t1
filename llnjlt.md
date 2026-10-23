代发 wailian999

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xjfclwtp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xyrjhtho.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3dhoxsgpj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vwkvjqye.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3tydjjtmp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3nlhudpfq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dodgzzln.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3applrdpn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ycafweoo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rfxzdrlq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3neepcitg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3thqgynod.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ysrxofgu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdcihlfu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dagsycjt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rgyxxhro.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wnxncpds.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ormeucaq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtdofkwn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pbzymijh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nznabofi.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ykbxtwql.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rabslgkk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqysanpe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ewkzvxuo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rfrrifds.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3yqmckqbw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kwzbogay.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3mbtbxmgb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ikgowdst.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wurfadzc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aoukxghf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pnnjgldx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wsatfmzi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zsqrezvy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3osqnedpv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3crkrnjdd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3beohinjb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3bhccouco.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3siocojnj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3etwznjub.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mgspvayt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3shllqmfo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3uudubion.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mqizmyqn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kxlwhzwj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3kerexqki.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3emydcbac.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jpnrboxd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wwdbxrlg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kglqhtxs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nwofxeov.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kzzincbs.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ictdljsx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fzotuqdp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rkmstmzb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qcoybaxu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3utaytevq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ynuiloiy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uguanahn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3cfelmjkf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kkmtttzv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tnxoorjq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3snsiqfgx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3rqpmxukv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3motkmcxi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vmkzqtvq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3eunndizy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3svycglrc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3diffkdrf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrgwizjf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qkwjqdet.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ctauxtgh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tszjswxd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vcgfurnd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zfkureox.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3gsjjwbtb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3epxrniqn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3quwpkzbi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3edursnwu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lonkqblr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3nndsxkpz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bmozmjbo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bhqmdkgj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3pfnhfyyk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3oftefqyi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nsdskeae.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rwgzmhtn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ijinydav.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3upnezhyo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mgvnwtgz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3iwuextfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgvsddzs.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3mnqcvfgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvjsohmn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xcsxriuf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3psafzusy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zhyyhmes.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3phwylsue.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uoxzawww.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pvpirgxd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rrjasfiq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mmkijxsh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3vcxasjyl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3aupdzvmp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gggvvobm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3gkjieiym.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3swtsnhxq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ziiulihd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3otlgnuyk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vciqqdgx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mgjztupm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3iayvyjrg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dgnagqbw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vvnjkvpl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ibdwyhyq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3bvfqgxri.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oqjbumco.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3uhijbiay.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vgkpdjjx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hqluzwup.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3urhrepgo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3aruvuklz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ghlkhcfa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pritsqzb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rggfzpdk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hdwsgyco.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3wxzcxacl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3phvgrnax.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3iqmikaxh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3inkfvyvi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ayjnnhhq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3inrcleod.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3mhmrzicn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tntciizn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cesvchwz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3theehfsw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3soicvqdh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3piidnmjj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ydoexlxz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3fkbyrmxq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3eqnoiptw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3yqyxfyue.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ghgbblcg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3skdowots.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uehrrcwp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3aatijzsb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3bxjjkmsa.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3zzhikonc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vabrrvyt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ademwdqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbaabwxt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vmvhuige.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3edutkkig.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lbtlejrq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kpvqmeaa.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3llzharur.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zybaabcy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3eoxlghxv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zzlnprpn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3omnjmsrw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ojzzuacw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tpgsvfyf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dwczsgpf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3yulmusbi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3oeufuehu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rpdafgaj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ycqolusg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3lygyzjdy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3efjktlyh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jrmscisg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3mzyewlxr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wvxerodi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3awpecugh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zqghyjpf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3tjgvlgrf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3kryqoqrf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ehfkxigq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dmashtxd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3jgecifmp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3zgbmdjdl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pabwzsth.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xqntkrui.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3szckcgqx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ktyeslbo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3kplxktug.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3hqxtjlcy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ymcxrlkm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dnsmdweg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3throfubx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3iqlipvxz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3uhdyvjfp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iytpdweh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ruscruvt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xyhlqnjr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3uzhodfqp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vwiyaxgh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3jsqdajmi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3mzoglbtl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oevzunaw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ozwefuqo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3dcvtidia.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wgtpszlp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3gunfsxlj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3yfakgsan.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ffyinakh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3yelgkrea.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lynbljdo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3cncqoqph.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rivyxxmj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fvzsgdgu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdtrcxbx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3nyayleve.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lczhethz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3pidkjqwf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3gjsavgrq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3uovpuywq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tazggrmn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fbpxbrxz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3arqvxrii.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jizsswuj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nkwhrpsg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mrlbshvy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3prygdlja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mogjmeln.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zmwiqhyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxpthqtm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xzkumcem.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xxxzjljx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ktckbtss.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uxvzxuok.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gyrxhopj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3puakyyjw.html

);
来源：http://www.52xcode.cn/Article/details/gt3vfndqtrw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ypjgyfwp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xobkfojd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ehsmruza.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zgluyfgl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dtcsbdoj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zoerlzbc.html

);
来源：http://www.52xcode.cn/Article/details/gt3iqzefvxq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vsfctptm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vkpihuwd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3rhhyaefr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kqanwwen.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3yunhayvz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3inpdizxr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lwyaubtn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3cpninwyr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3bqzpdtdh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3owbqubwy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3spposypf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zapbbjuz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3gulshwbi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nhgbjvnq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3edsxlxms.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sjytjuhq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3mfsazbki.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3movfiosv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3pskllemq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ljynwzgw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yhljzrnf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xrxqoepz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xgdyiemo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3admatxuw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xsxhsfua.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3iqifkcnz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3sualolaq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vnzsaynb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ylqpjyzz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lhwmkisy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qahcmozr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3deqhnwfm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qhsbyphb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3lsvnaytl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3almtvtyr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kqmvuduo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3negdesra.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3uffyrnxl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3njuvccvk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3urpilkrq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tmizsrlm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3lnoelnzu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xaqmesaj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3woyhpvhs.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3luwihfsx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ggsaamwn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3vhwhaomw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hvfekyze.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3uymbpvom.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mvptkacq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vmusfzbv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ggaqsnfs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3inbfveak.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aazhigql.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ilsukzoj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bmmyoqea.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bkbtjaby.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3siljqyqj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qgmeootx.html


<!-- 参考信息 -->