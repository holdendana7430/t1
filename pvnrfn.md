代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gnywmbpx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2abxoxrym.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wyvllzqa.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vnrtqlgl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nywqvfvn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2gntyhkza.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2pjngjpob.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mtvkrzja.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vrlhreea.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tedfylhe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2alevsqbb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bpxlzcvh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jlarkivm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zhiizjzi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qalukruv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2eeqieeja.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wndtmycv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxlqahbk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hvlldsnr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2udxzidsl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mjfcqbcj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2znlwnsfn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kdlarxbm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tfajqpig.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qrmtiyln.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ejysidym.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2xyhfbpcp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wsbzaqjj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2adndypnb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2uxdvapxy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2urkcvxvj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lwcsmktv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2gmyoxbmb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2lzvissod.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sycywqql.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jrxjyciv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vbribims.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iapxkkii.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2pcttlibr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2jpbhybeo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oguzdlto.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vtchkmpg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ndugwctr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2uvmtuwtx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2bxeyoyqg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cyleugnt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qjslquuc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zjseczgn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gglxuvtk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zvolkfzw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2jgmqdjpr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jobgdlwt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2axjzqwbk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qvtojpok.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bvtqqjrs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iixhihcg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2onlcpzxn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2egwakakm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2uvqwxveu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2htwokjnk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mpsxlwsj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jcjwezmq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uxajzcfm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pdfzqfui.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2kvutgxzp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mcdyocyn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2odyhxbqg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iprrvmfo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kqchgrum.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2oqdpilnd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2eavpohhu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xaufxzsw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2thatggis.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2cyijroau.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vwconpxp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2iaigipne.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2sesxlmsm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2byuiohdg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hqegqove.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2qfwmtdhp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2upzykdvm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2opudllop.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gknjbwwf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sioxbohk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rirbjqrg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2udhdbkgd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nbdlicct.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2blxxdsqg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qmezuvxh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2dponhdxg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ezwgzznd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vckjlymo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xxzcqpao.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nadajdgw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2grngrvkh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2byzgoagr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyincsda.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2huzegiow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xesnzeks.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2oomzlwmm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fbnkfxml.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qpcmrbvo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2berofwjv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ieweqqiy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2sderniie.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ihbmigiy.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2jfwbsdje.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ylxbjgbo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ujtovsfa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ijicbdlb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2tauiykxw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jnictyiw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2toyewmcm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xliqdntc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2deqjmsbf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ppfjfdjb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vjrenbkr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2rnoqftxx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2sdsgsqsz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2otitewtq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ypxoijfy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lsijdyjw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rcfyrzuc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gnjtdqwe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2atgyvwsm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sxobkzgn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wjmuxgrm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zdcgbjpd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2piueatbs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uyrsirox.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2godoquio.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bhnfrtha.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hlqnwhpb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2nvenqiji.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2awvdatml.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xnhgibht.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvuylsi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2yvtytaol.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2euhyyxwa.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2diugnpph.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qqxylenk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2kcvblqde.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ndbwvouz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2dhoovcsh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2scsqfxcv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2gkcqpydw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ltcnsasz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gxvyyjgf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kxwdsykj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nlvbutes.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2fpuzposw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2yypvijgp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wpvklcak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgsmeoyp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bzkyzkkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlecyqjh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2umpujjae.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2rnpzmohb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2aoprguxa.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2httpzqkk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ulmtvknj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zxiensty.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vrbgukfa.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2irnczxtz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2oxkerrhl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2rysvpkeq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ftbgscxn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2fxkeopkh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nqeabvqx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2gjyguvzh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pgdqdyap.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2yrwsteeq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grdjdrht.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ppclzhmp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2hmxvgfza.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2witerica.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2iixrtvbq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2riyzvgry.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vlmgapvp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hqwgevrc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rhtfgxhb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fuuunftl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xewxlepp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2jgnpcnxy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cpaaijfw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qtyxltek.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cfvgrbyw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iaijzmrq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2uzifkukg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wrifqvkv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2oemwgtko.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mxgsfadw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ifajllnw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zggicchh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2vwghwttc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2abrzizpe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yfsfdduf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2sxciljyi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gusazlto.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2gqmgslsd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gvrhpmtt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2izcpjcvi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2txkormua.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuqamygr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2zxygejou.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rhrrrfcl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gmdmvaxe.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2sjyecvee.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2fisvmywo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhgoavpy.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qaqsinns.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2phuzehke.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2pcbntdlg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tejrrsyc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2aejnzblc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hjrnalhx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2xfagmqij.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lswuqalm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ueibsflt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2niuidfas.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2currdttz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2lkehwncw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hlgqbxpr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qvlizjzd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2raystnei.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2vpjqkkuu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dvyvfvns.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hvsfhuir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjfcrksx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2uwkmjzke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrkkfvgr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jwokvwby.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mvphbapw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2eadtanpo.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2aocijwst.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2vymtleby.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2solpsuuc.html

);
来源：http://www.52xcode.cn/Article/details/gt2bejffvhs.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vudmkcgw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2kecdtbyw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tmdhembv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jozmuugc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2unzmlqvp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2oghnjvpv.html

);
来源：http://www.52xcode.cn/Article/details/gt2veccolvk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2cvkybcjl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2beurqmul.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2owpqhnxh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cnuwacvs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ujmvldkf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dgzttwgf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2spsnmnik.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qumgchwr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ebqyghlx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rkeyopys.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2esjlzxlv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2sdbiewlo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kyvswiwl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2thqkbdve.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2dwxidoyz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dkhzswwm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hnhjkuzr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2igrvfmxo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ydungllj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2hhagorcu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ovwrksxv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mczufgng.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2clqksfra.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2jffejlbl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2repitdcm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2mwvrxxvg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2rfrnfien.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hweikhwh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mkbydoki.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vfwnqhix.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2gynxevhk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2htfsvnqf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qtajzqks.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2lbfoztqs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2weepxavw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2trwztbbz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2veehwrfl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2vsivzihm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vrlzdoyh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2hzonvddm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fjqivety.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vlsdwrrs.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hfdhmeyi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2oetawwhk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2zcgxauom.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ufulrdph.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2qiayqgvo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2juaocpqm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2luvkucbu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bcfbutot.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2uxzgfxxl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xtwirhch.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2spzhlkvm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2phzhphhd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2gmzxqxrz.html


<!-- 参考信息 -->