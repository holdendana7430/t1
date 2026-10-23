代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jclxdqfn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yohlwunc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gogktilj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zwkzlitd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ocnugnpq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pxswkals.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pyxgtcfp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vtournxb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kacpclau.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lpceypxq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3deuxbocz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3vkguxbgp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gmjyvrql.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xeiwfxuq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qjgnizqs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pjjvmjvk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vdebstik.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ylxdvadv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jafowwpz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wdmksslz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cryphaso.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rawmyaqm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ixanqsxs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tozaeavh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3vfuyxaij.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3uovputse.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3eqskemxw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3kxiknwft.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpmfsawn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zblldtmj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zqjhgxsf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uikzvnjp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofqxdsjc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ksfbjych.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3orggdfpd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bhmvrpcn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3tfbqzdig.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hvzhwtiu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3uaqliqoc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3besqqval.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rxhoxmzo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3zpqwlasw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3wfjdktie.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yljbaeoc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3fgtscwrk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gpgjekck.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tlrckbih.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hyzyxwud.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3erghagkq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zpaqwqhu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3twsaypnt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3daabkqou.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ypkotfvm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rwbndslm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3eukaornt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3shwxjmfb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zxjideuz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ldqzwmqc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lkgusxvr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cdbhkash.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ornctzde.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3rrbijnyr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cgmdpyuu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3euvbsvji.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3muymyqxf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3aqyjdigl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3shtflhuh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jknpnytt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3esyjohcl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ffecnzjk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qgzaapfc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zpzaxghd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vixhxony.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fusnbmom.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ihxcsdti.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kmculdqt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3tbelcgod.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3korgecam.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3inzveoev.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ndaqoesd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cnjhvpmt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3saewxytr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jrhqfave.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubczkvbq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xvgduclv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3uzpubpfg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3thhatsrf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3prgilrow.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3nlutynrj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3bltpmujr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3rxpiovnn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rcctqztu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qosuqtnv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3spuvvtdy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pgrhdaec.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yexytogg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qelnpquv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ksfvwzdv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yuisknzy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ttcexmxc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wmjospiy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3cpfgrfjo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3schnnedt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3amhjqlwx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ucmxyqft.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3pgzebnko.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ylqpqqdv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rzvtswfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhoaxugb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3evisrmfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrpmtnhp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ofrwxsje.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mwblebyc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3hvgkrnkx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rricnqsn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aqdoinoq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kyngbhom.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3psyproes.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3duyfdwrf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3oaftxahs.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eqiaekgr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xubuswli.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3hsyksnov.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cqnzifnc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kkmvqqfg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nakoaifp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3qkhjjzpn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3pcoiczjr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3uacqrnna.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3omtbpthd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3troxpbad.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3zujdoqmi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3slwgzgkw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3htfmwdyt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xtigvqwm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3lsdrsuyo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3mcjgwklg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bttmvinr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3lwkahoxb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3gafeizyr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mytzrqqh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sffhyzom.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufvnuarv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3zpuyywzi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pizdoiyj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pwnpxzyd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgctyjpu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qbzmrdbr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3yzoyspyw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3imlsuubr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xkfhuecv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fwhlfxer.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gaophzlq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3bdkzeurl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3eamjwnmk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjgogqxa.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3todlflls.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3mesweyqq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ingabstt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bhxjyuvz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dafntgzk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bxqiltmo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3psrgzmgf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qbbbgqlv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3rdzkzaaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqtuoacj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nxhaolps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bejpvkdm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3odjwgbpr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3krdnowwb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3eziyicvw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yysjskne.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yuhuxekd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3aebmshlm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hcixrvvi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wsutljjx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rfgbpfqp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nofwownh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3qgzcblpn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ebfcordk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3aofcxwwj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xzmxllqh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ezumcozg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3waiwcefe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3eqypgrxi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3txnsbzoc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3fdfdkgiw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kihmesjd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3thfbxxee.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tzqwggbf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3iasjnhjf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zfxmrucj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ovygwtam.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3taxufcfn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3pjbgptgq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fbpilugn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tgidghui.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3inrnptmk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ofutczfl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jlgwpzhv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3aqsmjnga.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3qpbhrxoz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3aissflxd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ysvkcolm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3sxmvtkui.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3wfcziame.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bffrposw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3yfgufdea.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qlqjkmbo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lhlvrxhm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lgnjkain.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nkajmbvo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3khwpmclt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3tzdndxmx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nubhvuby.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nkomimtj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3zijlskex.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oempodrx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qlkclfas.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vcejrlzv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3otmkxtap.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zkxlntth.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hxjaydgs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3wiiibfwr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3gubnigbi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3igvkhsnp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xavyxcvi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccylepap.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dnbvmmom.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dhbogcom.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3sfhdqjbg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3hqeueiyf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3srsqycxn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rgewpqpl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3dodukzga.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3clvftyrn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3nfkjylwg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xxossqaz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3cvluptdi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3kqppfxmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekqmtklv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3huudzotx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhkhbkzq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3nfaviypp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vejvravb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lanorzbw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3utfedkpe.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qlngcjfn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ivcsjysn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sxuukglq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3rihauewp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yncdokrl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wywwpzoi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oangocve.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3pmmuhrze.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ddbcyeoh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3phrjekqq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3onayqzgb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3enbvzgou.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3pkcapmtr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qzwefayx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3aauccydb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3sxotnlfn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3iopdhlij.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3tlxlzyvd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3cdtdzzhr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zxtzvslq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3udxbmesi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3usfacwvo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3alphsiet.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3owrbssgx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dayrbfdu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kmlzsidy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mchvtkmc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kphzgqrb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3julegqzk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fcnrakpj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3drtummbe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3rvfddbmh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ppbxifka.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3zyhlmxch.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3itcihfqo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3pxsajrwo.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3osfcswjf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fxctmxlv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3aywbzbki.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cwumyulu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3dxcsoevo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3efwojjxe.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3lmwhhihb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3wdkadwwy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3gagfqred.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3mhctctdu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3syyzfvtu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iellzouu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3mquwcasz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3axmpxltb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3wfxuyaya.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3vixgiqkf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nonbelud.html


<!-- 参考信息 -->