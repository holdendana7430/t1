代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3bisiqeby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exncgtij.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rctgghbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqmitpmi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qpmlwppm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pbmtrxgy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3leiyrglz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pnskcydi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3guczimdz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yepmmzkv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzujnbke.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vcqjzjjv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tfzvmwps.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vmxtxver.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wdctwdge.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3egvpuqne.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mrlvlwmc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ayeopgzn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3thadgxit.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jfbpdxsd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nguzypqk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jllvyche.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lgbrolgj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kuijwppi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wlgibuzz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bkfumuge.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mcgxlppl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3omslytam.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zncsrxbl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3uznbcztg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dbqpaneg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3orfixeff.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3osqhkjwn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3isxgyqpp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yodvedhd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fcbyekpw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbtayknf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jmgyefay.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lpkvfzld.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tzsyriaq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3oeugzssa.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zqoqnzwp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrxlpzir.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dhhxyckf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhwlqdrw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3deqsgzsi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3srozaqoa.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hlumehnn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhrlezxc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ucpmwgmk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qbupjytg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hskbtgid.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fvrdujhl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zgfeawsh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3mgfzhyrr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3gmfsigxt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bkyolyjo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3djmxptle.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qlzprsjd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3bodwyirx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3evatwcxr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3pvrwzzqk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3qyaxyzgx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3sfuhqrfq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hjcnzmli.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hdmydgga.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vuyvgnvx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3exbornpr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3mesptdcc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3rufdgnjn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lngaamwz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gpgsvknn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3emuqkhdn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3boklmbqj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tuvjngaj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ctljpflh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3azsmkvxt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oxxsljfd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3szldwfed.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xxqceosp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3elgrekio.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jtgeggmt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lhhkziuv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xjddmhro.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rrmsiirg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3bezrlxkv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3lnnqjbyg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3huclbbaw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mmkyahum.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yiuveypu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fwtpknpu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ykdadtug.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qnjhgxxh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rkfsxblp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lvkpihjx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zyqqjyuw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3neghxyra.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wcpudrqa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vdcoyvtk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uwlnkfqv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gbumvvpa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fuwaysiv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kyoxarwh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3albcancj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dmeobwdx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ywvlugpz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gouvxqan.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xykiqvmx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hhmbwmpp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tkejspuz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jobckuhq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sfixfozo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhzpgxpo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3gcluwogq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxnejmjr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hlvzxaml.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3nqsshuyr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3lzjokzcm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dmmxilbl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3petngeph.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3sekajdmp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wutzietr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xhjpzptd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3uyiksixr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kpgehlmo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ktzgdovz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ezwjcisd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fgbyqhdj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uzenicru.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ijqvrfbf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lrynhois.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3errwktmd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3haqpuudw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rcxisjkb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3sfbdeyrx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3uppyfwxn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3usfbzdhu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kktrtgmo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjnqophq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fwtcmxte.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3yilqmacs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jlmjlhad.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bvoaqueo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3oqmyedmw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vlckbfpy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqlqajdz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjddbicj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3sdrbdixa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3tciydkov.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vtszrbrp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3emcojemo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3cdcwejbb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wlnstuxn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3rgqouqar.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vdpfivik.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wvnmwpgc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3cmuotxnq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xdvpwgly.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3buehapll.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mfpomwwl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3agyuawns.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uapmpvdr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3rfcgjegs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qyvclbpt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tcolahlm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eyvhvlmo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wtnosthy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3bvxpqlny.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3yzdzmena.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfpgcadi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nhyrjmmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyqpnylz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dtimmlur.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3twerypvj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3laqpxmdv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3iklvzsbg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nesvzszg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lrwnqsvi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3diffwhvr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nfufqjyd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3slufqtcx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3gwtyeucx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3acloapjy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cxhvavcv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dsycvtva.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3dhhlfskk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dfnhmggf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ojwxwejt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3yvylpika.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ngcsrzaw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3asfqnfae.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3uahhgjnn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3toestwwb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3aidgghyj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ipmnxmmw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3tncpiysa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3tdqyxtyh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ikpitchi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3fmeojxfh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3mnewakzq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3hxvnuxui.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tzzcnqfn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gonmesax.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jcurvteh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3laaagxvh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3kosjthuq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hgtuenqz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zyfnvuwg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dpaknjju.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3szagwbew.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3bbgtwtqm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3lcfbyqyr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3roujwrvg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3blsemvet.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kfetjnzn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3zlaryagf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3igwxnukj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ackgjnii.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hyqbjvcs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdpauvlb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3zdttfyap.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gvzipojj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fqqpligp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbzbydlr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3jgfubauk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3luosbuzb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zooaqobl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jurnnfsz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ppyrqpfu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hdtbghqd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aygnswrq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvorvwxd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wfvhsgjx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mipoovgd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3bplgcldi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ofbfgdca.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3bjxjljlv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ndkhvwnn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wvzomdca.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dhezmxmj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ejgxnwcv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3mzlytnac.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mfppciae.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3fdapkqco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suixlbrz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zxfwpuft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbjknkxt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hqijbzud.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3pstpwxeg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lkajkins.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vulinrjx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ciwltuuy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3zywxiegk.html

);
来源：http://www.52xcode.cn/Article/details/gt3eyrlolxn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3bsxfuhdw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kafmthlm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xjdiscvo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3msvbfewz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3birydvbp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3mrtgnbpf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jslcoqka.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fwgxwsnl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3onqrxunu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bwcyxhdc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3rpybirbb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ounhatic.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3xuyhadml.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ztpivoqi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3llyrofcd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wqvjmcug.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3fivrdwyh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3dsvkoncy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wyfveigs.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3anvyxoge.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wmrxfnnh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3isjjylna.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qvqvimer.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3qdgavlyn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vbkzwuem.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3osgqwend.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xwvffagk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3cfxuymrb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3emewlwbb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ikdkbggu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nwyutbxn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3nrusisfd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3cotobzwj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3gwozrozf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3inrdshbl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3zrbiudnh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uwwuhorh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3waxtxenm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3eyesejpf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fbcijnny.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3pwcrholl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3phenfrto.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3gzcxhgyj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rfhfwtdp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3toziipnl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ajnqplsn.html


<!-- 参考信息 -->