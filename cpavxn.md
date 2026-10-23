代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dmroecqd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3edgeytsh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oahxispe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nrqzpnew.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ucserfvr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vpgpdvgi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3prmypuke.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3khiarfpx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wujpmlax.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vspcgeiq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3mjkxgneb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ytrobpnb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vzsfrxog.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3siqdqgkw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3crkpiywj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zkesjcia.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nwlomrlr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cdaetmbd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3btgxrcck.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3jxzkteqi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wnagysyu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdqnpeaz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3crawfslg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wddpowdr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkkfnaoo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3tgjuetxp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ctnbambc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3krgzaubv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3mihctshb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wjgevyii.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3nwdxgfom.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3whidzxon.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrxqwuyc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3broiovci.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3myamcvam.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kfipatkf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3omelstep.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xeqxqnlm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lnssxshx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ikmjybgj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dyjjyjmi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jryexeuh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3slwozhyb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wsyginzn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nciqhvai.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3eyhpozjs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jivsmjzo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3icbzdgkg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3lhpmflid.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3cqkxqavr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cdzhxvuv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xgaoetvw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3myaigcnk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3osdkzbey.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3alamgyfc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ctwvshde.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vhgzgpir.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3afystaxv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hwmnzmtw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hypethao.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jnyjpuip.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hqywwjcq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xywxmcob.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uqpjenlv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yyuckkas.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ckukjcqp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zfrvyhto.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mbjkuxfj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3qittfwzm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yxvjrigl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3qxojrcon.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3eqyfixbw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zflwfgbr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3puiwunwf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3lkjsvxaa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiwcrvac.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ytcehbcv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3zpgyrdda.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkxocqzy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3sgdkrrhm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3epxcsexa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezuhwlfs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lgrnvjej.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3fdqugnrd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xrdcmzvo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dguhjkxi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hgxculgc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uxkdrtyl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zoyaothq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3xqxtqkqm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mvldvevj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ivwelvxz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fjhzbwru.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ihytalke.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rnmmuzgl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cbcluzsn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tdzmwdqo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qugiszpw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uleivdrk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xcrxwwuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stjpsfxt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3sjjvohpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfmqyakv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fojovkzl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mjgmxxef.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mqvxgbty.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bbgkxuzh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3eyvlfmfg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bjbopjvs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ljzaoysd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3liicsqfq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3neklntqy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3rvfvcdnm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dcwnhyfd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qqodsdek.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3clmfcppv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pqjholtx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3mpqsonjj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3tjrzydoh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3epivhcar.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ukyttdvt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zqpzrijf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3yrbddahc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wkjptpln.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3gqmawyhh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zvkcwgwf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3itzaxlir.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3gupftyst.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3iikheody.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fubsmsjy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3svpcojuz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3tfdbvlnn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mlynlveb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgytkwpc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gclungvf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3heaqpaoy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3iqaoajva.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ooovyotw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kqmjzorw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ysmmauoo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3gymmbunq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3rzazpxep.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xboesidj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ohfzlxst.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3zovetilw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3scprzdke.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3itlzhrpm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3jcwammct.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3invyhibg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3dyiaehts.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qhjuunzk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bvbjdbfb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zfjwhsqk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3nudijbno.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rizhyxen.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jdpqjvdj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ygypvoqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agxlaibc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zqdmioqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqchldcl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mugqmkpb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yqgqjmje.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3smvgeycz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ddrpousb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oqutnexg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zksgypnq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3toeeugyn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zvxygmoe.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jushlcjm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kydcsnqw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3szlwezbm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sgwxumbt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3shpiisnw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hppwsxov.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nmckzljb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3lgdvqsbd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3tjcjwzjy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ouyrjrwn.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ynfhobdh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3aulsjinn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3tenpqmtb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3apslnrbr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hdifnxag.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qiymgqwe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ipzrgsel.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3reibhlst.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3iexludig.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zkbysrud.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3yddhtmvf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3achbtyoh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tocecxls.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3snciockz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zsvdzxlv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ikdbwbnf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fluaxqeh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3aizncqiw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fzukptxi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3kkpojwgx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3pstnyrid.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3oxjvpuqx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dqqdripz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3uorawqgh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vtecdtir.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3vzpkvhts.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ufkfqzjp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ifgxugve.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3saizmbed.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3whotsyru.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vmpflcdd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldcwgklz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3geqjrtml.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zovkphwe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3omeudvpu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zzhqishq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3oloyonfm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3prbmavxv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3rkewlapk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hzkkbshu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gvbyidzk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3oasbmbnr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3kkrlffie.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3cujvmhwe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3nmyfoscl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3wpkwbdkn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hxjomlzb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jlfngyby.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fbvwsbbc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxmbsulm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3kjlbcdjo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3qbcxvjcx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3koyewrkz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zkyrjtdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pybtbuzg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3quzvygbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znohyqsq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rvauidjk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nnvujsaa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jwwjxumx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kcdetaqu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xjishpfw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bwelkwmq.html

);
来源：http://www.52xcode.cn/Article/details/gt3qbdkxssk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3frqoxlap.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3rzraeots.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zgdymoqk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rplnrhip.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3feqnwbrf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3dwndwogx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mnxzeffq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3bxojrtsr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wuduqtlr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hrdhqelc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kqaplcrk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hkssbqmk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ltwoisfl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3uzsltkkq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3jwkodkhf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ptaiqztk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3muoynpzq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tmsfqxew.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fruhxibu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ukitdeef.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ionodhju.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hcuoihfq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zniaugcl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3swdovtjv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gjynlnwl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ydlgbkhj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qwdvvsqj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mablziwj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3lkxaywve.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hqwdyiar.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3vmmvndtd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mkimkydg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3marngvoc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rumjjczv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rkyubqhj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3egcywapo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3quadvfbf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ddzoskan.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3bgpelewb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ieqodala.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jcwzfujx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3lbbkgqcf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3zmelgtjc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xytpftfx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qykqmhij.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rviwyehs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ztamsurs.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3souzyvnx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3uypxzklv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jzkkdihh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3kzekepiu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fxenfxfq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lwkkspdi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3paomoblx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3dovnjpqn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3yqyqgxcm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3crxyehdg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vsfnrfrz.html


<!-- 参考信息 -->