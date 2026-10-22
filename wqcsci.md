代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ohjlyiqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjzadhbs.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2wtglxiau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymrfcoxg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xhsznafk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2acvagbbr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2aqofyjrs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nytncypb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ksscxfvj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2enwbpowk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pnkgohvw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2lmjqcjyu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rgsfqojh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2lenvgdhe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kpkzzjjh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rtpujsig.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jxgmklac.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bjjubpht.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fcxvfjzt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ibcudgms.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xweorjmu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2twdwavbz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2eyylxqwv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2kphmzrhw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2akfzmikl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jylkyerz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nfbmaota.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ukkhqddu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2azhaokix.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kclyklob.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2nkzshviq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2lihdgmfs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kxwrcviu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jevvjdls.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zzhhdmom.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kgxuznvt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsrtbpky.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jlizuabk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hzfluucb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rdetrosu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nsuwjfbx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xlfejdvg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2guuxbxbb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lsvheasb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdonptvj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2piignupc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2nrhfkoez.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uvvknyqn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsschixk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2oksleulx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2alxdewvt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2phkmqzbd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wtzjufeg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2afyzqhgh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2bfnipnrk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mpxbsptj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rikpvehj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sxuueyay.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jgihpllt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2urvfzxel.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2dvohsdof.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jjeddfge.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qktuerrm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2qpvdvoma.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fnalkigd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2serwbiek.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2lijwwxjk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2xnlbtume.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhrfyou.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2gfibejgu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vzdcaoki.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wjrynvxh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bahnodzv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2usftarxc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2tfmyqfzr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mdmbplpa.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rvpsdtsz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2lmjluqpc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nkrvytkn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tabftwjc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vivdzvvz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2momakdyv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2sgnafudr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bqwrvagp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nbdglusd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lkybxoth.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2yvlkxmpe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ghlxyekn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2juzpmygf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bzfhshwp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2wcdexkih.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ibdeprms.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2hlyjlrsa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hriyakox.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2knikqhdg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2yvifldbw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2povhtdzr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jlwqaino.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2puauybyl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vscdgwen.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uezvaldc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2fxzfsobt.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2chtlqlpq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2zupxeato.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2htgodpzp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2sumvfbdt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sfsalxuu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dutnvhop.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tzgtycge.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2xznepfbb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2evwrgowi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nghmkmwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axxmzxjw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wcesimlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ceqqqhfl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2pgjhzrlz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gseuduki.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2fblpboym.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gbtalepx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2swshicsb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hzxlahca.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jpbjdels.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bxutbrcp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2jrtgmavk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yvcycnyu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2eywweivw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qfgxpleb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2baoglubl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2unknabfy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2yghinjqh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nmrjvjun.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2atgkdjfs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mgyypnwb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2qjobunbe.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2brgqdfsi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2glpdchau.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2abpbfokc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kmqdjzlq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2iwiithwf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tmuqoaxn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2oetulcbc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yeyobkid.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2yqkgunjg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2scyfatky.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mmikvdnm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpaddogn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogvbdwec.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2fjxvzcob.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2zkvzdphi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ghsobjfy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gixstbmc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2slcbhcex.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jdrizylg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2kqybhavz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wvpwrcgw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2trawzlar.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ecqyuppf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2xwirqhpz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zsgwwxar.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcrycgvy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zfuhyaoj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jjqnuihu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rulqiowz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qrmrejos.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ynvyaxuv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kqipppif.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2vncnfvtw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ivcstqwl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uhwlkxlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdwusiqj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2fbgzbwvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idghhvzd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2oagqxhkm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2kraesbuk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hpqkmpia.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vfcmvndv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kcaphdyz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fadvwytj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2micvudsx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mdvimuqm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mvfokpbx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2okucybrx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ujrojeyh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vooizfsu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2syabfgtq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jknewojc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ftyqzhlv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zqyshbmg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bsmaojbo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ngrmfhux.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jwydebvw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2nweturwj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2qbblhwky.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hmceudje.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jidlkwgj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2aizypcrw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2nxqwjdlj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cnwkanlt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ootueoca.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ucwdwztx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ilirsnyz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2myjntdff.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sfvgawsc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dsaieqqd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pflidaca.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2cclvdhjd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2pymrxtst.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2olklrrgh.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2pouwbjec.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2dmbawigq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kjazpqtz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xgvyzjhk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pqhrgqvs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2veonigdp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bfwifgwh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ukjnqidi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2iogjrpus.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2epzlknth.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xauozajs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2icqoutzc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xexgwdio.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2eyiuqqom.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xndsqwxi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybloceym.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2yixhfhps.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nbsxwtkk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2fskzegcc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2wllhzmpg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2shqrqpvt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iiftjsno.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qplbsfog.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2jehikluz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2fjtxiozs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2hpnhxzvi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2umjfwypu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2twfpxiev.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2mpzpuxly.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qsomsodm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gwatzpas.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrewgezm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2arjexrzn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2usmwbuyz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2onvaztrw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rzmemcgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ernolopd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2zkuctujq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpizzggm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hrcohpjt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2tztrrnrv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vxdzsgjd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2iezpvaac.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mhebprmj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rgvchgrg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zpfkhwfb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2htoeyajq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zgqwxuap.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ixjguhop.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lvhquybv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2nloqrqfc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vgvwqnnz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cfxqhopt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2doyizqdq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2txehyqre.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2eirceokq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2cyixrkrv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2gelouzer.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2wnpphogk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cfautmwu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ttzdhxfv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2dalvhrni.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wiyvrjkh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2azwgfwjv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wpjtnafn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2lxswuhbg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2apposbgr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2tbwkptto.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tirvhson.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jzvyryau.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ayjkbhkk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2dxsfzpse.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2lzggixbh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vgnvpski.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2cxwcbflb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xblvuvra.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2fpchtbuj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mwhdcmjs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2beyqymuo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pfltwkav.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2opjnvfhg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zsdbtyeh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qpriioki.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2uxkbclyh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2tptwvial.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2fyswsgzl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xizjzqgh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kkgifoql.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ckxmjeqz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2owlsjgxu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2xamvimsg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fusfqngz.html


<!-- 参考信息 -->