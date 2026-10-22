代发 wailian999

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2stptaedl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zxwybnum.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mkzaoesu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2wmhrigop.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2etpbdpcw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mqslciwj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dqbwmwzo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2meyygluf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2vxeqdraz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ohftbhoa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2lhfmbfmo.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2uoikxvkt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2esnwqlkl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hknjostt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jmqcfdms.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lbigszim.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tkiutcwn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2nstuqjus.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sovrzsax.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fokwbimf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2kongjere.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wjbwvoxo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ftoipjhv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcvktimv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gmcalzwo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2farqgzie.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hxohfsiq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2rqpzuxft.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2uplcksjc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ibpporxs.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2oeqziqlx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2aynjycno.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bzllhsaj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zamuxhpb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qplfxdik.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qjvolbch.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2erjmimdi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2amyrtmao.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fpfrqayz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vrbcetrd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2comlcgrc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2qqxsauoa.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cxiakdij.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bgvgagfy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2krwhnbqg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vgfftnty.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wpbyixdm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qbqartzf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rtglumdm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2fohykmin.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sksmlvpg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2anjzlpwt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hvucypfh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bmcgnhpb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zaoidwdm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ysvmgizs.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zemrgehw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hulwzurf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2azqgmiro.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xefgbbuc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2cvccbvmx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jzuhurqa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2akgkpeez.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ulybmazi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2imabwcyy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2pfebbqaw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ggwwtqby.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioaiaqvm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cowxmesf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yfzbrwei.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2acwnmgxl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rbupxzdr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ravsjjqn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnurrehz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cnmoaouw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wzofegyx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2rvxxrfyi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tnhickyd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ytbzqkah.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gwtcowfe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2svgseslt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2myphcagz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wadcxdlo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2slcfslrk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2oyorqvdn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wpncacfl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mpuhcepk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2skgjdrgj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wwcwyksp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2itwzjfzq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2cprkdrbu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cdidblln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufpuouhh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qlgkrrux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gccstirx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2chkkavbb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wbggmqug.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mduepgfj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xqgwcwyl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ndqmpwxx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jgofviln.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2zndtxvir.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2qummsseg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fxohkbxw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2puhczkhm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2enxnedak.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2vedwdsmc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bbgylmmu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vbqepyij.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2pftikono.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2sksuywkd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qvmxjqls.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dndlsymz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2admisvip.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gsbzdhcf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ndrfsuox.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2iqvipuik.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vtuvrlig.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tujoffcr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2uldiclzy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bfxyphgp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bgihsjnk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vvvwbukd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pgojxehf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jipxwvyf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dcbkpras.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbwqhbvl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bgibeedv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2cbirnmqk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2grvzubun.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2slcvljpf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dukvfomw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2flmiviwp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2oyipxneg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vhuxocob.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rosxiqcz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ygztwpel.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2agxtvpnm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2osmabbhl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2cerumyaw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2sfizyuge.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2shkwcjwp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2bxntmole.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2apepytsr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hggbthyh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jtuvswdv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2qrqmydjo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2gpjckauw.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2pjseobed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sovkwyap.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jharakga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkpyowvr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ylntuamq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2yfpujgdc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mvjxjskl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uuojegak.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jufzlrzu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jmczaiyd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2pejerhmp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2esqtxcoc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2wrlcjzrb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2eupotxab.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mxbwqnsq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2dzlgfkep.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2tbjqatha.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2rpgxftoz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fwytuism.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2oaqucfqk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2iirfotbq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2eqiorngs.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2giftbrlp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2kxydiuiy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2wvvsgwit.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zywypvmf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qrwgblvs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2frxwnqnf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2akpwkrte.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2uonlbstz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2lwwkuqgp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mhtpimak.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gfldnaaq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tsbaqiik.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vznpradf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ltjvpgch.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lqvbhpvo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2recyywzu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2amgrrpdi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wqzmpnut.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2bpftlwcx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2kvpszjwz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2bxuidkdm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2tosrrkod.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2opajagob.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2adqrzmhl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2udlarajs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jtjuqatq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qsfbkyrj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2kvzjynhv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fxkuoxgy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksjlvmxs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2jvjvpnjy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mocgmjia.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2drafisqk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2exqshdpu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2aukcezou.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2iozzahae.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2cpohrlnx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2nikjndao.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2rvvxlfeg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dnomaaql.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2droeoaey.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2svaqzngi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2mmjlpkjq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hdxyboii.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2vrfsmbub.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2tjunhfge.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xrecvkis.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nauyarcp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2evoftlym.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zhxpdujn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vspjhcjh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2vzhdovip.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lgalsusy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qolspnbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrzntagi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rajmhiai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkghztnn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2tsokvvqx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2cvigpuqb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vjwubtqj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fjqfirse.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2hukchczj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2vasqclfo.html

);
来源：http://www.52xcode.cn/Article/details/gt2ghogiuaf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2wrcyyvpd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2jnsxcmma.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tmqkezab.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2spzlmtln.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2bashohro.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2omrnzhwp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2snjjstze.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2bujtooro.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2sdoosecn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lynmshxu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jsvdywjy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2sfliuxlo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ztbujlga.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2hdvzevef.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xgplqoae.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mcopzmzm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2mvkzzhdp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2gyqavgnm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cjzuzmug.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uexxjhbp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ayeepkyo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2fvjcgepn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qczgqunc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ciemtrwt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bweeditq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2lkgisnmh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2nvqkxwng.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zyzhdnxw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2scorcqxz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tzuljewa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2uaopgnat.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2xpfzvbnu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2fbobxohx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2hyguyhvz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tafwmjlx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2iyklmacv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vftgaabr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2vipixzzh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2wpdlgqev.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2valwhkzg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2esiicxew.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ymvjgluf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2uhtfajph.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2trayzxxc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kyoymgvm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tnzhouol.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gccpkedv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2duwcbabt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hbbtsxeh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2rxbdplem.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2netrlpkp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2imfamfpe.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ccytsijz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ajmleave.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2sorclhfd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2bbrkmzpk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mooeptix.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2tmbqzdof.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bgkfwzxk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rgtwwkry.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vkmjuygu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jjtwuykq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2beorqqxf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2toqmqnyh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2roxwasnm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2weqchdju.html


<!-- 参考信息 -->