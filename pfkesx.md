代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfqbepnl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xovmxgkj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fsswjcai.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sfnzlupr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3aqlhjdav.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3marutjpq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vtfdlaaw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fbokngtg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wpefnksl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ukhgktde.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vnoasrnl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ymawudfl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rhdbonpk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mytxrdev.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dktfodbi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qebhcdzw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mvhlhkle.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3cyignyvh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zxwdrmpf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cfqhxyqn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqmpucpd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3abbfwcei.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fordnczs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vdeozfda.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujjtsljc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3bcvfbdcc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmsxxmgm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bgziroyt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3sbarvgij.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3atpopgfr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qdiqziru.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhzifzot.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qpscnojg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3hwcprwfh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3iqjljaxj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ytmxlrzh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3pehbqwwl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gbvmosmp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qrbllsoj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ttsbloki.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vqsfydgp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3henxkgyy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3yflqxsag.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zamibspl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3izhferwk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3baryqoyj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3alvyetap.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3duiyogrf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3egymgoen.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3cmbgforz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rbbvshwx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rbhmrgos.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hsplptps.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3wxwvjqkl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3mfiqeife.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ftajjvqe.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cunjpzxo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lusfnmdg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gflvwlmt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jmywuffc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ynfmxvcm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3codepxsc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qajxheuc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lhjdnwoy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jlhhixcs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tbtydysv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lnqbwodz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fygcfxri.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3epliuzuk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oyrivlso.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pnmsmgvo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ihlpzsqm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wrecglti.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ruwcpagb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3tjfrlivz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwzdocau.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gczwihzh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zemmcpse.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3mbacmzce.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ozubzyty.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mjcidfmr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3umprigbs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3aaqjheye.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3fzqvtqxs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3sdxmussr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jbdbdhey.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3exkaqzbi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vxyyemdt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mqstjxvs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3bktqqjoo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ilyouxlt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rvwkrfcn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3uhcfrcju.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mdaaxaxm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3okeranqh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3quuzogmg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vnfxufhe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qhtupdov.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ikyxozxh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3giloxunr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avsgipkt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rfdkdzps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njoierth.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dmcckzvp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3sdwywwhd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jcoibmxd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ikdzqeco.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jkrjbqmz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3icypytvg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3hyucfbmw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hhgldhmt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lyqzckyw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zndkmtao.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3frhfxxmb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3zamurtcr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3aybvrqgt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mogzcety.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3gbblswnu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3pyuogaes.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3gkwphqgj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3mhapnevy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3acuzaekp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hffqgrav.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lfijjejg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zifnkjaz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wiuxnyul.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjmslahi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zorkwmpi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hjbcgtbw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3liyhghhu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pacmbevz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kzdmdfjm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3xjwekzzt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlvvkdsd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3boamvkdr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3pijslgpe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3dzhafmvx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3fagasxtz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3baffjtxc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3nznmtpbj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zzwjtfdr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ulthmihn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pnvshtwx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kqpppvye.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ejynnihv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vbpmvmav.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lgfgvhbj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3pccuahqm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3vfjmwidh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3myuzupsu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ancnsccv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bmutyzou.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xpadtelg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3thaqcmhl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3fvuyncpy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3lvytyxzg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nubucieh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzrhclwz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3iyhpehpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syjkpzru.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uvsiilyg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qkibpbcs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mqacztep.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3phfaiiio.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pvsuwjpm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3bpiousqn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jmasxebh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3lbjqmrzm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3szmvwlbs.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3phkicifs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3quoasfhs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubrugbax.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yaorhqfj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rfcmzviv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fvpnbenx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3bhgisndc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shqzbzky.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3egzcshuy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3zxlbqgkx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3izgnsnee.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ntuercsm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tmulmasg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nepvbylo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uhnexeiz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3koypygij.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3azaomlzr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3yupnlowx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fkonvfmw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mtnmhyuz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dvsklivp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ernhiwyl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pbivhvny.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wqptdtjs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3yqijtpdf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3yjjzcwdp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3stqsjdka.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3naqxlflu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tujmpbqb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3qnpaqyyz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gkrbjrjm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vtitgxvm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3rokhmvhc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mrurgzcq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3fdgytrpg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3wsxqcpol.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3dkbjvyhi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3zlovotev.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygpeikmp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3koilwjwe.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3khqbuvod.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywdysvmy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3awnjeskd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hyuhiqmn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3gjjujzgf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3febabwpk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3syjavuft.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3syhgsvwb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wtufxhjr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ttxijhsv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qcsnuvij.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3svruzjlp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3laovpbqs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lazrjirs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ncqanjor.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ytxdacjn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3erbeuwfh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3xvotpllu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dghjqpnv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jxpzodid.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3pgbdjkyd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qrmgngrh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3uuejmemr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtpxurde.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3clwegxlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqynobwp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3tsuceuho.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3yfnkgtbh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mvaitzqp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fzybovvy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ltgdewlq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3hqdlrdmq.html

);
来源：http://www.52xcode.cn/Article/details/gt3gljjniza.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ojbhpmjp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3mplbjrgq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pyicxlnc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ldwrirlc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tzkcdemj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3twwzztpi.html

);
来源：http://www.52xcode.cn/Article/details/gt3zzafbrhc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tpynmwrx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3sszekgdw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3cqufjgir.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bvwevwfx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3vvdznnpc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3nbkvvkwz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3mvzrgekf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xaubdqux.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3lkbdrsmm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pdsiqeux.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3caoleoed.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jkpoezha.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3owkkfzdm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cbtkzcxp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dxvxcfgw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ilqftqif.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3smvbgthq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yladybzm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3iinxcdkk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3isywptsg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3tobjcarg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3pchpgddk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rzajiqec.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3eyojqrye.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3xyprpsxo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qxjassjk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3cylpfsta.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stfjpgtn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3myupoikz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mjnytuvc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3khzhhrbo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hhmswpks.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rqtaofgn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3wspvgtpw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xbcermyl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fcydwrhm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bhewcanb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3oosrogao.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3jttzroca.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ivvepvrc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3leyacgvo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3nuhubecw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3uqtkubdc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ndjnhrbm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3oejctdjd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fuhjfjzv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rgqwtlfu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qocmmyzf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vlhrjahp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3loxedylx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3uejhbbhe.html


<!-- 参考信息 -->