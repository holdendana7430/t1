代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yqwlgtcc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rjhjjwjg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3pedsrama.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qtfmjuoe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jhyzupuf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bhorfynb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3nazdmtax.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3tnrdxipo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vupskqug.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wbnhmtlh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3eesbzucg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xppcaqgl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3uanzacpd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3idvztrjh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3myyzxpbf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3hscuyqat.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xnkaxgwq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vroyeykt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ipeouzru.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wzqcyktv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpbcxndd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xlaocawe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nblhzygf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mrgyjomu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kkulgmfo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nosuqjyy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3tfdwfsgd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxxmuywk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kjhuuvus.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qnwecyck.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3njqzsinj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xexeoiir.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppalulqc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xzqslarh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3egjqhckb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mkscpzpz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bqryrdor.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zjejdsjw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3pvlkjxbr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ziehmrjv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3msdfmaih.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rbkikpox.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tercxrns.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3xgrubibw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3afvezflb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ujitfjiv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3wcqakvsx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fytdwyzb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kgmvvocy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3amjbzytz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3lisaeerk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3uofyhmnp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qfvygilm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hrdstaip.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nffytuwl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oidteajv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pwespwzc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nqoakqku.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qhnnwzjl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tllewykw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ejteeyck.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wfafbppz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cnrbuojl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3udvitnwt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3fvoqjanz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kofpjtra.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3uznrrfyx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sjiahdlj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3shbnryam.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3thwpopck.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3adutvgmj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bxmgkzxc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3atikkluk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yvjjnhiq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3uzbotopu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xzluhzsr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3cullpbrh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmalsjiv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mwbmlcgx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3tmztzdvf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3oyyorsru.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jmqummbv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3srcykmly.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ikrhhnmz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wxhzadew.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jlifssmx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mguowykz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3chtpkleo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wnlteoxc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ioqwdqii.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kebgxnhd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gvirhilf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ietmktlh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yshqeyxk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3eyejimtu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dztujjoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxjbyott.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3fjkplxsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxpkxnhd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3khminobc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3zwptyxvc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ccpvheyd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3feyvqfoq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kctbtkrr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hepdohub.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3xnkcbkcf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3qkrbjjiw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3fgsvxccg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3pzliiure.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ocysqquf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3uslgwdod.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dpkucxsq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3goarisbv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dimsesfw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3lusjafou.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3oxomabsj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xrughfzd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3onlwtzcy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ttsqrina.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3mkdnyjfd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3xnhvivpx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gxpwieda.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3beqogxdp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xxsntrbn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ejxiesau.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3untgoyqa.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rhgogpge.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3pujdvryv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qqhyudrp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3iwjnogtb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjfpubmi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rwrcphoh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3svczguiv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3opwdnzku.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3csprrgvl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3kzfbzhmu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3kplipriv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3netcyyzd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pnottelv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dvqxbmls.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ofmrmtel.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3dcodwnvi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3urnmvugf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3qiqdbffk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3wpdmwbmy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ogsflzim.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3nbyprdbs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vobogeep.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fxbjnpci.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ficbdnhx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3vatooejr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ivcxqiou.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3slzjmujq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xiuhapop.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3qshqtasz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhsbqzqv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3udrjhhtl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3grvyoieu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3yovdhttl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zheobaqa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cddatcow.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3iwfqdpkc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fwufljuo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mtlvhrev.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ycgckrhm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xuekxqmg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vbflmgud.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3njkvqbaj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3opsnebyt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3rxhuaenr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oloigqns.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gcdikqat.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3cgrkrmky.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qpdgneid.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zljmitam.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3arjnmuvu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3uddjarkf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jieqxilm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3azbxpthh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kkzspfym.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3udbftcxb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xeskggxl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3irpztmpn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3whtpaijf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3cyarhknh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hvmaiyti.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ecapenna.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ajuuidvx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ffcfucet.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3oklknsiq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qhswnxzt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pgwomujp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3nuarkzgh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3izybrltb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3kyyhmeyq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3tmupzkti.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3okoaixci.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3fkiysbay.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zgxymmsc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3earbjkqm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3zgyullku.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3sxstkuem.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3avfydver.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3esdgmgqd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3qykgvuaw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmleawca.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adelnvet.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zodxqkap.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3inizueqd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3lfevbipu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hjwqfrpn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3wiovnkta.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3jbqpikit.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ffkescmd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lkjingoy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zvmynttq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3qixakldy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tqyqjnep.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dauopxaf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fazsbrij.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3teuiuuak.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rrjrndpu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3itrenahw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vqrujjmz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rxybbmcx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3gdaoyvpp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mplzuhqx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gibcxfab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epczkqiq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3twgwmkrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldwpbeut.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3bkwvwemd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3wuiklhdp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tnqpegwx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pbeoqzjn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qetuakae.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3fpiehknf.html

);
来源：http://www.52xcode.cn/Article/details/gt3hgfbewzg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3rxpdpevx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3pgnkacwq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rigailhl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ggyvarea.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3fqknqdmt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xteywotm.html

);
来源：http://www.52xcode.cn/Article/details/gt3wvudpuus.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3pysttfug.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yrezygbx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3czxupprq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3wmtztksz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vxluxdfc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3wmfiowon.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3adkyulxc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3touwhdih.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3whvjhysx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pdoodvbm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3unmykkxb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tzrkylyi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3djcvccrx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fenlmwcc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rvmrrsnw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ynwccdgw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3nhvkbxgs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rrrlvjdk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3lnwyipph.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3pvqisfoa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3pkzlwqzf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dtlyimdy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ktkwmime.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3etxkjazm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ljglzucu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3holbdvpy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mcxonewz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pgtgqjgn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3bbkmbuux.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pxjsuivr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hikoscsk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3uotvaecd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qgfumhln.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3zmqeepwl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3banholul.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3vznffxli.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wfkoaekm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3scdjhiqz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3gjpzwjud.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mpudwmbc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3blxrruod.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vnjzqsmo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3addrctdw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3upxlnwsn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3uqamhcur.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3keabainp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hcvshlqg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3silidrqb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jaswawjd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dbffarcy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qlviepqr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rmjbrsgo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3jnxloneb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rcoesxaa.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3iqezsaqe.html


<!-- 参考信息 -->