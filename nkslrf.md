代发 wailian999

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3naiakfsb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ultviilq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3notqckcl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qseomuyi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3qfjbgqbw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jsznowuk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sehqmxdn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3mbdvfwgo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bdkhhppi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jebzlzkr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hltgrwkt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gqaizbbe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pupaejwn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wufbwceo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nmgsmncb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3prhljmiz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dxvdovju.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wjmbhwxt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bpkjtakv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rmaieetf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ulezltbz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qzliovch.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3epihnxhf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlysjsxi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqkpjusz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ewirexqt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3venynncc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3estspbxl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxjvnznw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3taagyjuj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xegezhxi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3snlgdeif.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nyqdmmco.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3disqsitp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dokcceuf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3fmbfujmb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ugvcgkfo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sysuypvw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3vqyvozlf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3unjyhmre.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ngxcqgcq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3uoqqtbgp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vkiiahtc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jquwgyow.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3qyzhgtpc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3rbyxkuwu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3kanvjhii.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tkffzjjp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3znyznjsi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kbyqsjtk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vjfpsrjy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pupntkyk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3duulkcyh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bggcsllb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3srcjlduk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iyqlqpps.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tctxrdjw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fiogrzox.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wygcldqp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qvobxrtt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3sojunbea.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3scvgqkre.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gssvlhyk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tvxrkfsd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3raqiglwn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3plmcwdco.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3stlndkoo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsdjsxsd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nohlgimj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ojvfbxbo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppltohas.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zvcdrpia.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3wcxkfntf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ulrbifys.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3moqjqiau.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dghelttz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3mklzziym.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ilqcfycv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sbpvaxke.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gepxoxmy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bvejihgi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fmapavut.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xhozlzfg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3xcdoilrd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3djxirpwf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3yvvtyujr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xndhrsdf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3aveqpbql.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lgnjgbxe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3huzlfrxv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3agutiavc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3egyrznvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzormrsn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3sijqvfyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcvmtzvz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ydozzcdg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3iyibuvur.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3agixjeyy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3erltfgdm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3enrqdash.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qmwgmxqb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3firgaqnx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhfenrk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pcimciqu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mfdaykdn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3axjwjhtk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3twchgbld.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nphmhfbc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sflpzque.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xkhqimfp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nrtdznqn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3rsttrmcc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3cladyeex.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ocupikdl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3dhlzdiuv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3hqtbdrje.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ytsbexit.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nfumvejr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3egisnzhi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3qcdyctbv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hmgeddpm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tiheihed.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bezbrdtm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3pynxqqcn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mdlvoohd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhzhhrse.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ngiubjkl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3bhnwjypc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ewucpojv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dlifcmct.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndxsjxql.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3pioygjqk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3btkbwcwa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fghpsarw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ivnyqlkw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3usurukcg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3yrhuwtgn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3rgncxlux.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rqistfkg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3towmmhrb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3eytknyho.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vrqzoacl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kzcdwdka.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rwncxnrz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3imootpwx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3khqtqhvr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3awftwdaq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3kqqbkoso.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3gkqxshbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3creffrrk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3tyrtuhrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfjhqjyk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rjbjcryg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3pxqdaerp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mhnobcyo.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ztxgflqw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dxhmxxqb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lmwatqpe.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ttleuudb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3homydkjd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nguidbmq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3zwdzttko.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3toevomyo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cdncwtsn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vkvsxclm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ewdwxdzc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vzzszblz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3nnquiiyw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3eryvjrdv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3pizyxpst.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3pgqzldmb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rmsmyhdq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3uriwasij.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vxvouoma.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zcqsccgp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3nmephrex.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3etbkdzbw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdzrhty.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3euxgxtkq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3kxkdaqjy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3zakvzdkn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nmstrasr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ogvclkky.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vbuvekee.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kubqklho.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3kqogixey.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3dtzjioiz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3curvrxwg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3hwhsaadg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mdkqmyuh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3atykceky.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3mvooisby.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ydxfldkw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gnnvgohs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sccsgksu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kujwcwxx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3felnpzfx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pvemmepz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3orfawjrw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lvnzxcgz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3etmcmvdd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3skujryyn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzgrbcyp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vkclhkyf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3htdljxku.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3lxjulyvs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mvaogprd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hglktfmh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3oawktwvc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mgvxmwde.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xdzrezbc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbmcyjcu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ujlglruf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kbtuhfbp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3gyzspqpw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ikibzdwn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3oxwqhbry.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ytpifwpw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wbrguxsz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3itfydmlo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3akipydbs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3wfbiawkp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3fahgzqof.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3pzhmiklr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shfeblfz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3msuqelil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nanqrpsk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3aphcjoxr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3rvfsaaii.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3olmhdyes.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3teiubbga.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3klugqmyv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ubeixeco.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fehnbtyj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ykzrjqwg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3wmufgoer.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jufvtdsp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qpsdqwlz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3woapppiw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3sjtrbxjn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mmdrjdfg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3monqjybw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hmfunpye.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3oreysbek.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dcqopqmv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ojxywccn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3jhkmnhbl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vcqoowxu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3cozsrbyg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3zywiavkv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3oikbmuet.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tjdlgpxc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3luvergnw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3yuqrfsbz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tnpwmrjc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3hzwdjflp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3simucghu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vbmymgix.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hoalhoqu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vswekden.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3lbdfvkoh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3gmknbvxl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3rqdxsxyt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gyhvwype.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3yddaffkt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3zxfvgpqi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3tvkmedsx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nnlcthwc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ihvzckxv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uqcmugtf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fjdztbsc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3yvslguwd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ykbyohpc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3olozociv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3cnwztorg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jclhltzt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3vmmihcur.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fatpvljq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mwvwycku.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bpvoccck.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kbdbital.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3dcqoggia.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3cjvhpafk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3musgqjkq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jtcjkphp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pbpljfaj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wqveqfbm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3khwkchce.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3oyysekrr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tvvwhiwo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lwvfdsgt.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ktrfqprj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3exozmdok.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jcnoezkc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eqnecjyy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nzvcdobf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lrhxakih.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fspfszyd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3staksckr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3icrzjnmp.html


<!-- 参考信息 -->