代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tdcyhxvk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lzecdwel.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gkcmjpsf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2lgxsjlsh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bkbxfrkt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rnatdabs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vgsthnvh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahsppxxv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ohwcayeb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ppklahym.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qwzovaxp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2aiszwhko.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ptjnituu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vjskmvxq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lopdwnax.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nfdypmib.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jclpfhyh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2leqxfmon.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bxgbpank.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2jmgpvnev.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vonxoogb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2casrpwqu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qtmwjkqe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bcpbpsuy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjuiquan.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2urgrfxay.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pviixjyr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lmovplku.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2vlmexfyh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qfswwxnf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2sgmpilwt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qcyjgkoa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2slykakof.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2dxnvfioo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2edtuylkk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ukpfllrk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkqsjiqr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sohqiowj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fysbgtmx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gfpckdni.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mnrlqeze.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wemywfsl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zikevuqu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2uirymugz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dqrhslwo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2phzxiquc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2vhrqpcmt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mzdcgqic.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mrispztk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kbvopwzp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2euypuacu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ksxonagb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2kejsdtql.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jrkfdzpp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2bktwarlm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ztmseyrk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2osxavfqx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rzhapwqt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2osfvdnwj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dbsirkis.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2herzcbtt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pzuwveiy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2bhsnsmxz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2onxahvri.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nbfwwvko.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wtjskacq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uvyryxer.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aiqksscm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2xyqucblb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qzfsbmrx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2afxspmxs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ovjouqvr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yxvuvctj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2stbskbhr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2biznaxmq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2wkkjtflu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gnkwyfmd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2igzxugcp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xnrkjbyz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ocnsloxs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ylwurhmf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nycokdsc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2bnfckexq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2pkkrnvrs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2twuycrrt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pklnwkju.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tqkpmmhr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vwuafvyt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jhgatqcu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lkofpvha.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mxvunubn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2irqpxasf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2kjgxrdkn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2pbpjnyrs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2paliqfie.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ktxslvvk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2btpdmsbb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2lvthopyl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2drsxyhny.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2knjbjipu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrqxhdzr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2kdkxwdxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ciwusoom.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2noswvtug.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fniqnufo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ojtvbwkt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2qyponukt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hafzekvy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cmtqnsds.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2tlrpucpd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2knvslkeu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2thzxfgzd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iwthndyj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2xglggnzk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vbtdgpcu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wsdzlglp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yklrwzsu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cysgnciw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qyoelqbw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mwliepjg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rkgxebha.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nycqnqws.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qsrvwsnp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2cqyougpd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kmjmrrji.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nnmdjkjh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hubinqks.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ocezztjf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ykqjfpyh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqurqerq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vlpgjeme.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pxolzkat.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ekydlvva.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvyrtfqo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pflbiuoe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rhnbelko.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rwkdklxw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2wxnlmgte.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2omjflvsd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jofpxmsj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sfmthzna.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jndddwij.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cndzganv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tixbjkup.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2itsfznao.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zufrddza.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wmonityo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2cvnchhrn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2mcmgvieq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2vviaombu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2xyelvpmu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qvrdvxvn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ugruhvfe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ikcgyvri.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2gimudprl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2uhuxpxbn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ibfexpec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgfmfjiy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2crfojszf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asagwimf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2scdmxina.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2sztxkmyn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2szwksqyk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qbktoetg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fpvnkgoz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gdczuzca.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pfdldmsr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2qiukloik.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2oyvceins.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2jzcxfdgy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mrvikqsx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ajztjbet.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jazwcofu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kwncvjlt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nmezdmhp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rrqbkcwz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hkqzlarj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2aripnaht.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2seaglloz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ligcfuur.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2atxpwuxm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nsstjduc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dexsukpw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2glqcoreo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nqruqabn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bnxlbdiy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vdveklfp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2itrptlbz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2fbheqpsh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qqouzwxx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ydazovtq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2odcwvzsj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2twpptehg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2kiiwbeye.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ryshqvuo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ngsswxde.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2aowewmve.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rdflkotd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2kzmkkfoi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qiiuklrs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mcbbffzz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2vkvduwni.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2msdykujn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2coxzntum.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2olaiacik.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ufghgskz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2quvnwano.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljgjbmgb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2uozpuxht.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2amlmumiq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlqkrhcv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2jetvegke.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ckwooeda.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrutmuxn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2mtjhbelo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vurzdgxo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ervzkyyz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rbqnbxmq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zhmhzcmc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2aauoefiv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ujxkwwoz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fczflhup.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2vnszbvox.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2tsapiqhj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2neskcltj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jhgtgokt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tvrcpqaq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbjxgyrb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hrzbpild.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2mwtxvdtn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2yaepnnyx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2axyodlll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qppaircq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ptlcwgxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqokqkog.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ybygluwx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2djqsnpjf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jgyoolqq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2afkraclc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2wpfcdujx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wyvhzpmw.html

);
来源：http://www.52xcode.cn/Article/details/gt2arkuwfxi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2myzrelkw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2icsigqnv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mdjwbnfk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vmxpipkx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2teabitgz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2kfyvtiem.html

);
来源：http://www.52xcode.cn/Article/details/gt2ptpqynfx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2obkixbvi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dzzswpjb.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bgqdutxa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2obghwulj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2goutsqwp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2iznnnsdq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2wjxevewn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2jftmbaxn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2sefvhymu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iaktldre.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vkfqylbz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vohpftqx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2yifrssqs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2uoncvenf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ljhpqjeb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jcgdtior.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ggpsldlv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2izratufp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jrrujhba.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2bltpeiac.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2pqvutmbg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ftvzzcyu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dkvaumji.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2undfyzpw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mxyjgykx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bysysklq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2yfmshkdm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tydfdcsf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2qkymyuzn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tjsnuirc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lpzwgdpr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ojtdgzfu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tzwzahda.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2aflbrwue.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2adteckjy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mftlblye.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uwdeveir.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2eqeziemj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2iwhjwdra.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ohzidbon.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2eljscwgt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2rkhfzhwb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2bmcwenao.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2zlzigvie.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gzwligbu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2goxbyrki.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2oxwngzim.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ebivwvra.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ajvrfuen.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gfveyqui.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hvsccrar.html


<!-- 参考信息 -->