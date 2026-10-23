代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zufccqsb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hredbxlh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3irkvuuzo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zcxpewdl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vsztinwl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cowpvmab.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vddvuazw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nmxffopg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3beesaqtq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3tqharrhv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3mpqprezq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wvqabuel.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dbwaglcr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ptfhovmi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3irkpoxvq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yrbsawgv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3njrahvda.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jpqwplfb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ctxxdnmi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ptfxauwz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ouxywdkq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pltmytuk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cfzudzjk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nczaxokx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbvjsfet.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3eplgpoiq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pphakkjo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qruyuthr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ugfoeoor.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lxvxenef.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3njcgcbwx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3codwobah.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzhhtvew.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ahmfanxk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gevfnplq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3wbsavyur.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3asabskjj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3urjswnxl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wafdaymu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nrvfcbwk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3twdcpzaf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gvjyyyle.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3stujycaa.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mijuffhl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ynietirp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rijinlrt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qlhsylvx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3lmeemyyg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3muddsqoz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3onmsiqro.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hipwwcqh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ghcckrsu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ndaqkygo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3vjdplyku.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ksgtxaco.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zybzjewk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3anrbtfzn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3uervivsz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3axcqdhvp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zihfkmkr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bpichkdm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zgsvvgya.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uvgezmoo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yrksvmhn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3aitmfavg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3btwzpeda.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bwoegsou.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qntyiuvp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3rnmhrmxb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qnnwfcbv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3wivfjztv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gwdptlhj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rltcnchx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3spkbyjru.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3oztnecoy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gzoyvfpk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3rsjafbsn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hdyjqylb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nrohsvfu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ubhkchcw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3agywodxl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3klomyibs.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ruwxdkcn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3splslfpp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3fsmntecd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bbwwpgns.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jqkjftoc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zoyunceh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3newoyarh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3teiqlybq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bhgziwep.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3adsgyrra.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fesyjyxk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3evmlnzml.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jssmhpkf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3doawprqz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3acureugw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3jkubmvdv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3mjvymnep.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bxeughut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3daaponam.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bupqzosa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idtzrcrl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bzvwcpen.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ygsgnbpj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3lgznpdle.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3criqxvls.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tybiobpd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3axwgqomr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3gdvarofo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3bequzxbm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3lfvweyml.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yjywrprq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3crgsvuha.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3fdmxzuwk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yqucnjji.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cdwtokrv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hyvnwirw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3sggqdhgs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3rbkldtpw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3chrizgje.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3fxsugygg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qznvnfnk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3qzeaobfk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ruxnevau.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jplbrvhh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hgmyhtgz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3nlajuivl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3poqizjlf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ksjvqenx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3snfcvper.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3memovvcf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jfvpleym.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3homouife.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzuwdkls.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3flduoewv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3omdrvlko.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dzknhmou.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctvqovvv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3yquitgyl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3eunhcgmf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ujiupcda.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cbogyopg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dcgsqmxt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3crqchtda.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3yasfixvn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kblnyxod.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hutwuhxo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dediikml.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qifnihlu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3rvcvfpas.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ogqckcpv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3sniagvvz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3inugesxl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3zpjxhqld.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dplapjqi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3kfkopimv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucbuxsgt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3lowxbpdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmfkwerk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wjrzjbgp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kdidepud.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3oufztgpx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xgjjfhdd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3olqwxfwc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bzvlnmeh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3dlbstiyq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vrmoofvz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3waqzhagf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tsklwzpi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3juuwpiqk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tftgszxs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3rpcpimkp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3lsfbhkth.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xbmcifll.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3sbjxcxzd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvxbkdyp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dwkjcrty.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hbzkvhpn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3khijpbzt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3nmkzaqil.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pkevenne.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iuncepti.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqyyxez.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yitggjko.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3lumjbhic.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kfctxpur.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fsmqafvk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3aurnnpsf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ipubezjc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jupsgcxq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dofyqmli.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jwkqjaii.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ntrmrafc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ylqbqffy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qabjoygj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3uaecinsu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3asjvqiyi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fjwfjdwk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3gockzmva.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lndxrvrt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3cthjqmiu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dlaugpjq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3qmrbmewd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3oajeuehe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3toydbqgg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3bvewpgtg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aotnkjgh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vbfgghvn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3wfstyxgo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xxhwlzuq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3gmmjohjx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3aswxndjy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocpnoujb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3oewgyrst.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3tuzkyecl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ogirigfm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gmnfomym.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3klmycstz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lhipsjmv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dbvpsycs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jgzzkudu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3nqvrsprk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3shakzlcj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ulttiegn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3nryiebwq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fhhzkaui.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3locsylou.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3vrjcnqvt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3umslrbwg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3lasopbwy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3rgadcqtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lopxioax.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3svuyteez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghrsmplv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3qhchqgju.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3bgtgdgux.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3evvtqmft.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nlmknyha.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3nfxbgeky.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bsfeyutb.html

);
来源：http://www.52xcode.cn/Article/details/gt3dprxfzwh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ncbhyzbd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3peudzmbj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wfbisexq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bneamcvw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tfiesuxv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3phswjqjy.html

);
来源：http://www.52xcode.cn/Article/details/gt3psxwzwvx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3aartusvg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3qfbehwrk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3rtvygtdc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tsxlvhqz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3hdkweivh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3uuzxgrok.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3bhtialpv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bfoxnjhi.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3kqjmzvup.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3engmkufn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gfnvlvbg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nmbfkfon.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qxehgvpp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ftuurums.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vogsxlfx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vwksjqbm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3htgncduc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fmzliobq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ynivpchc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3eohgnfiv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3kjwbrrhi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3higkxcpv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ongysylc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3zuujyeve.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wkdxzlsn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jchozvuw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3cuqpvscd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wwwcckfi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3totjukih.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3edamomcm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3kaisghmi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3beyppnbe.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3sdwrjryb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3yithhpmd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3fdvlirfv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3plqrorgk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qfcmonid.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gcnhwptm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rnxtcqwg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jqvmyfjs.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3lrvnktay.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3pjrfoify.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3cnckbeok.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fqerodjf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3cxhpyhcn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vruzesdi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3csmxnadt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ivebpvlp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bqfnwejk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yjayqwbu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3pvupfybu.html


<!-- 参考信息 -->