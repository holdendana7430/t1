代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rglxmaps.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gairlbtn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3etavgfry.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dflpfzht.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ezuatkuf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xhjsgpes.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yongkwiw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3resgzzws.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ygkxisks.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3videyjkn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3drztnplp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3znqectkv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3grdkgpuh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3vmpkznwq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3quzrygzq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3nlyjabqd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dzphvhzw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lmsqyulg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vasbpczx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tqmvangs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3sndsytve.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3gfpscdij.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kuzmdjri.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ziudmoav.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kxdycdxa.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fbfqzncp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaprqjid.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eqxhdwff.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vavnvjdo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gezmgkra.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3enkvjxit.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3antigtzb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xeyxuiyx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vatpgsfv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nghozawk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pjfrdokw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3syveymoj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eavjeqxt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3hhuqxzfa.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3vehdgsjl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ajcwnepm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kvndzjom.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gfuuzppf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3syalqyxv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3uwodlzbs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3zdizghad.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hrwnweks.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rbzymnod.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xgilbqjy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3vmbnflwp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3hazajkrw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3xtzfaanm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bhilaziz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3odxdwgtv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jewjbfwg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ehchhkoh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jxffowub.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pxdikikk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3tiwgpnro.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pdcauelr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ujjfzwtb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uelgpioe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cnhksluq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vrnkcrtg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wflegmxz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ajhbrlxd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3jswqjolw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zwhvehwo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qhrcfskx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ykwxihyc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3sxzrjiqm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3byzpbyjb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qjkusdig.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pjswqlmn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebptglbl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ttqxxovc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ynecltvb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzhlvddu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vfwqlydu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jeervbmz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3akoirqzm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vlayrfxm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ppohkule.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ndadkcec.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nksrojqe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3hcnhmlhr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zoxfgqnd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mvxbvjjt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3slcyvorx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ohymukdw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ftauhyqi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xenpogjl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3alteupds.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hhzuhpws.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3uraicvzj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ekimahqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmsoqtqt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3jbddnbnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kekddrlo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ubdieynw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3khimyrvh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3kijkfnlf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gbukzmyo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ryqvkkqs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hlplxbhl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3tlezjogy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3zlvayxpo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kxoeofnp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mqtwagdh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3rhnntbiv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3bvnmzycp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hdhgbtqg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dbvajekk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xvjkhxwr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fivqtani.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3bdsggrie.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3laqecgty.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zdpfiyzl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3uvbikbmg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nxoskjxo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3khbzrpyk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3evpiiuwn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jrisndmo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3quvopmwv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3erkzlrfs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fpivtqej.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mjyuobcd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ndvniafi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zbumfmtf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eborhzdz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3oqpqqmmd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3sabryrcu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3uyvwrqtt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3musqxshy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3huazlwum.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fgeuxsmn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vdjieyds.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3duulyyuc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ahnnqmir.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fuagfuga.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3menbttyr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jpqcwbhj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vslfhsra.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3rtikqoen.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kpiarbmh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3amujmnre.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3nlsvhnzb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qbpgwdkv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3opjaribx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hkatctws.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3eweijzzn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3muxpfvjy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yxagljmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3moapopff.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejtdvltr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3heuagzge.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ztjibkmk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3janpaozf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3wquomgry.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uoixcuzk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3udhjjklw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ajkirefy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pjjndtcr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3csdonqbg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rsdctoce.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3riglmpmu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xmwozcgw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qmweyjvl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ytrosoov.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zasmhcrb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ppkgeqcd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qbeiwqrv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3jivrxlzw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3nxfxoanr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3flbxxypu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3espzmbkd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3exzxkvcf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3knxmndfa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rcrpkval.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jwzrmozb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3mwxyvase.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3psuxirzq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3hhftakry.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fthpiqmg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qxfuwyid.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3psqaxbnm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3uolhdagq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mhzzkfyo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vhausfat.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mscgnrzd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fkqedycl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wyemhfqr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3yxgqquun.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3adxukvez.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3gacghkxu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vqdbrkvg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vabwtuxq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3wtwlwwoq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3luhazugw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bhwvljhn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jedwxobm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3fddepcsk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3xldywlju.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbqdljfv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3czmvbows.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3skbsovzw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gxcgccmm.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3titmwsgd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3pqhasblc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3yxhyskxv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xbhurvqd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3psicpmpv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3mqzimewh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mucrnqre.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mqtiouzu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqjkxldh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ycjalzeh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3orkopgbe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3tbwtkmyz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3yuvmtfbj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ijyiukwo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bufgmieg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3imdzcbno.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlrhbggk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3shnbuylv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3hmkihcka.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3iayridzn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3giuhfvhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3voxfleqh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3trnaveiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpwcjimu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3kcnheehi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3mgewpkud.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xqlfvedw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vebuhsxu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3bjxdmhzr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qtloyoqp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ktkizxsa.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3uxhmkuji.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ijwqpxcc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pypafaoq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vsaenhio.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3vjxmspsi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3dkormagk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rmtgwctg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ddyhopao.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3fffdzkcy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3botmhqbl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gwmkrrib.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wmkbaefp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mmknsfpd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3qhfojldc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jnvuwcoo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3psltmxqz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xrwntbgw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ykketpwb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nftbapef.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3tuaeabxm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nggsjwlh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zunqtaqj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3twnrmtsi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tbdqnlmx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xdblalsn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3cgdkjwqx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3dlqrayig.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qztdrnjl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3fckeadzh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zudzoufk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3slstxyvs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3utiwqgar.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3xorfmphx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3oykphhwd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pjnfzcey.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rxcqklog.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aogxanty.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nyesxoat.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uwqjekkv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xfgxgesj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3uogmgyoj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3sjpfmddt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jjnqzwod.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xhgoeouj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3mkfecjpz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3otphehwl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nxuofocz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3fsmkvssj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3dcflefiu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qabewlkk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3yyxdpixg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uglihujw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jnwgdojn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zhsedbyv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3eclwqfcc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3mbgqdvpt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mwxvkipl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tjwqyour.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vrdjwcbh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qezuhndk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qbvqlklj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pzoitxsy.html


<!-- 参考信息 -->