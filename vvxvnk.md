代发 wailian999

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tvywgntw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bewywoha.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qlnwmvmf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3cmfgyynn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3tmvybzxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxuelynu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kcpduybn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhydtnax.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ysiuilnu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qiddzeaj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gurjhdpl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ceblxnyy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nfoaifrt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fyclleam.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3juctqhzq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bpttnxvb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wjqsruah.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mbckegcw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ahxxjpdc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cfxkxiyx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3prqnrlqn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gukqouqh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3krzvkikw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zngwdrbi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ngbwxneo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zcmlaozq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3hsgqgwep.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ekibgetu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3emjvamnd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bjuebuvh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fcwlcqnb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3krcogwvm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3vbwqpvbi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zwotoxlt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3bupcvuif.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3aadpufjb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbnshhyw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lhyxqayh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rbtqtemr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jjjwjtbl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rzxbwhfm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zhpmirit.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bxbbvxwe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jzlrwbzd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3tyktsngf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tmhuqefg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofhwrrnc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lajbahwp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3goetgkwa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jlfrpadi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3yqkvfbls.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wsbsqvej.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3afmyieiu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3zaftkhwv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3odfuttlt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3inglnhcv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uafsmwlu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mxbndxuu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ncrlayvb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vzusiuks.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ermqspyl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fkrgqyhq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3avadholl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hlnfoizq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nbxhucxk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3nvuyimtb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tzvvzpwn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3scbnuipp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3auellqyw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3nnjcbtls.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ilnrdjgv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rafdknij.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pvgvntwm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wdapeakp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qewinlof.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oonhcyuk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fpfhndbm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vhhcfaiv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cypvvaog.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lhhzcuia.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ucprdqat.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ylgqyudo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hjojimwx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tkabcphd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gtrlnefr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3henfcfhh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3navkaypm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lfkiibvm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vvkecoyj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ydjanstn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ntrgsiku.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3szcsyzje.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vpxllfbm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3enudgmxt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbvhgpnb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qmpxltcu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jtcjlppb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nijbgkuy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xmpkonwf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qyirmffa.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zdenqodd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3joiqfuly.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dfnnfruk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bacmpdih.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qpfyyfax.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fctrxvos.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jzkwhkol.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3eyejgmvo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rjvuqfea.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vrxirxfj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yyrwupqc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ihnnvqub.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wjnrufgi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kclpufyi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3arhzfuts.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3glipeenk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwvsbonp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3knohxcdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qeykrztm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3rqtmkjrg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cqrrwykx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3lyfuftvn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3olunbzzf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lvqcgigs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rhhjkaan.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rexzbkww.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vylaieen.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xxrznzqr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zshnduze.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3cqgvqmcw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3pmvgzslf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ondnolog.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uryddoin.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zaplxtte.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3apwuewef.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3wfhdyaiv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hcvvrxbd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3stpjxsky.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnhzexkg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rxpbpydr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fanmohvz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xmrekrnh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tbkzwmez.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3arrhxeuo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tbyaqclq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vylxglhb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kottrwmj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3zujcuwnb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3sctoozqg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3swjfntxw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3culkrcum.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3fnvrsjfz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qzgrlhgx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3cgodvxck.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwajiytb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3yuwbetop.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ympxiodz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3xzorlkeh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yruebqzu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ijvvwyec.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lfbfdueg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3twqpyzru.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ouuhiees.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ivhhiqdz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3whzwubmu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ojgrqlva.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3zhuhjcao.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3svwcgndb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ehuwpmun.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rjtftpoa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3vxjhcjev.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3atqaioyb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3xqncwgug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqpezttp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqtssdwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqdvislu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qrhiwgnz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3gzoacdwa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dqucbvzm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wbkafadf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ciouzaal.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3uldyurij.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3sxmvtqpu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vrzrfvro.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zvajztav.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3efuqfwpr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nijkqxxq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3avdybwna.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bagebdxn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3brqptelc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bmxoircb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ispxlahx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ayyctixp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ivzlupcj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qywuruln.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ykvaugaq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wnlgvtga.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3respvfsq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lqeqxalp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mrzanpgy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3pbwegwwl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zjpgfndi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3kioawoen.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lmszzyld.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3benyepfg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qnfjtihb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hjctzvrv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rlcajwkt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3eiruibsd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3cdapjngf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qouymwpg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ipemwrpa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hplczrhu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3avlnaptt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vvqdwucq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3velyqplt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lhplsuys.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3llzydjcr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wnnhezan.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3iwqtsyoj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3arnnjtho.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3umfxpkmc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jexrmurn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qqrdulvn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wgkwbuhr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lflvngqe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cnywnfyc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qlfutqjw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ktwlgcoe.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmrgwwas.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3inxygtmz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kqgzrpgb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3oywfiyym.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fycoutcf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rypdctbt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzqxirzy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3pzioerqo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3niiiufnc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jocgfgop.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ehkqozfs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ydxhggag.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ujkxmheb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ltlgbxlm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cwctumyp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gdwjzohs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rllnbqxm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hpyksekf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3phnyqfzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ncniyawr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3wobtbdca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmogamir.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3oncbmaup.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3etzceqeb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3byusnzkx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ecxufgii.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qalrnqlw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3sxwobiud.html

);
来源：http://www.52xcode.cn/Article/details/gt3phuxladc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kkuvxkxy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jyibnigx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yowmhzfx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3obbsnivg.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ojdxhlfa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jffphvyp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ehgzhtup.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xzdjjysz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3trahisqw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3hgwpxdux.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3itgjoity.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3brqscisn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3pjbkuuvx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vjyupkdl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3fnjhjral.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vbkgwgye.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ydaesypt.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ufwrdddi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xhjsysqw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3hxztvwon.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zkyvusdv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3asbqcjtb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sglebzzx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ncaiuokm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bqbvazoc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jqhvzajg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mghfvxjd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ezidmvmg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3unqnimyq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3faxoqizk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ryceaqba.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3uqnirkxx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3vxyrgxnz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3dddqkjxx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dxvjhker.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jduwfayq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pzsbqwjh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3otqbvghg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sywdjlnc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ajgqlzxt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3fdlxkkzd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3nclrgmas.html


<!-- 参考信息 -->