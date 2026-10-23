代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mmebvnfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kunygrkc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qbmuovvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbpqfngl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ywsqmtec.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tjpwbckc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kndlgmmu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vcgejyur.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3prksswch.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjckcogg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3inagnkao.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nyjwhzjp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmbdbhmh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3jzonpkfk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oiraoelk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3vnlqqlzm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3akxxmiob.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3liqyhuig.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pvwyieci.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3asndbzpc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fltsssjc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nmrqltgn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wmqnokog.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3vrbihrke.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3slcyddpf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bcthjawf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zhkwhkex.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bcztajru.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3qndzvfab.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3fcgfyeyv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3xkgraifk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3faaroaig.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghylqirs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnnarurl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ujkoxbjx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ydfbcrgw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xunlohtj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3oyqoipew.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vmfykfzq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zlsiekcb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ctjmlpbw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mubncpfq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wicwvrwa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vxysgqdj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vwwfxxwi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3zznoglxg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3wmaczpzo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lzgkbyfg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ddxdwifa.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vaamtzay.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ryyqlrvd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pvfancxf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pzknndcd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mydpmjcf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qpwpbssf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kvfbikza.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wdxlcxng.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lldsboum.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qpfbbtnz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3wcuycrpf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nhsjhdqo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wvunjwqe.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qepwghfu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3nkwqxtfe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3qakdnhyf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jsxqrkuc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3fetencvw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hqyuyfsx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3taqygqlf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3clxpxmzt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3damfrvnj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mymgopsc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3usiadjqq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zgulishw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gqqxwpjt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wkqccxee.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qmjgmuqn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3qkpxovex.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3avvivitk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ujuvldej.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3fjpyvbpy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ydonfzhi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mnpkmhvf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bdzhxwhy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ntsaapkf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3rrudnotf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3oxkoprfl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3nblsvqmk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fckenwpa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wgaifxce.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovszhhcw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3lhtjyydn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3pbngsklw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwhmozie.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gvusfugz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3dtdrfyug.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxwuonap.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3arshuqcq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xtgresrt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ujuvhbru.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sjpilqbd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zwccrsph.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yddrthxa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vuxxzcyc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3nfkcabnv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wybuxlwe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fopiaqgu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jxdjrssc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bchordzm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3uqsutvvg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ukhmsnyg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zvjngaen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgwhocuv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dtshhxgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tuvsninh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3isstvtgv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3oovewkyb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gvjrlmra.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3imwotzse.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3isymwail.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3vldzzslm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3znrhitbz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3otgcecbu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3kirrkdhu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3fejsihmb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3fywwixjf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vbpptkyw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dxjhmbuk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lnrfrjpt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pnrxppcs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jherrgyr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3nufrnpuo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3axmfefoe.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3clznslph.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3pxmgpdsx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3swwcsatc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3asutvdby.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3phezkhfl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlssaxyf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lxbppixh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pbvgkwvv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmphpatg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3aczchswm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3itmjqyls.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dehhfxwf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xkywyipd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ftcdcrjq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xobtmntu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xkbttuey.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3oqwyrjfn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pylgtjgu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fuomrgoh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3asngdfhd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3yxjsuyca.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hmpnjhcu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pvzymirn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3jypaiskp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3hkhptamn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vcnjmtzv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3oullonud.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ibulnbdm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kczkjlkf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ululhwri.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xkwjugvf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mlihqybq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tviepojj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3pnwzwkyf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uosfofoe.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3fynkdbym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vthsuwyd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3daypwyha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpragvyb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tqosedln.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3nmzrulbk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xcuqopwl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3enqlgmrh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kinhkqjj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3fregmrro.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wqaeceva.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qcshbzoh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3dckuzqam.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rpinzyom.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tikydiho.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3hgbjgpyf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wfrjzrnc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3kyidtmpn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3feruawcg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wctnpcgw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uqwuzvzn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3theunwvo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zakrscgn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3gyesofyl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3aksyfkrb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wwezxtig.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xlphmbjq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mitelssr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3draumuya.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nnuqqyqs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3cwlwobob.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3jcrpudmn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ivwusoym.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uzwimwbs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3deckwawh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fwjzzzku.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pugvormj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3olrvlssw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3qttbmxyb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zbhtkpdr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3slaitzcn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3cjwiukfw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3nlzitgct.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3caqpmdhu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bjboyyle.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3heigmgoc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dpkufiek.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lufvzbbi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lmzmvaqj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3bsgxjxvu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mridwzko.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hipznbqs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3jnlxftip.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdgtlsnv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jughjkvd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xstgomgf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ihslcfaa.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zklsrrmp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3iytqxotu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3siqjiwxp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3grkbsopp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bnjfxahw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3esgmpwdc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldhmcjix.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xwiussol.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3auxabfxt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3xlkerwjm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mvxemzyp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3bukzxhlq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vvkndgpc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3stbunbqw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ifodjbwb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3pylmopak.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ocposodf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jcivoqdg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jfrsfwsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlcekqnl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3gsffyudg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjvvyuyi.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pxwxeevr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hmppjtem.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3srnwbfeu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3huylliup.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qcuygqcb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3yqwtxbip.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mlzwlnbi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3jawdbvby.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3bysdssfe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uhwuxpxb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mrdfrbjm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3rmhrorwf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xstyielm.html

);
来源：http://www.52xcode.cn/Article/details/gt3nqxniypw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3iwxjiopv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ldfuhjhd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3slwrwbnj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3unjysova.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3beculbxn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rjbyexov.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vhfzmrba.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bjrjhxek.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3gxgakryz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3afwmvuoy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3dvspkzlm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yqzzhiab.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3jyfiuhwa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ohiuknlt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3adjteujh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rgirfmuj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3zugcvjae.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tjwlolhu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3evctxgvv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qjmvehgv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3xamdvwvt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3brjwyrgb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dpdpyvnk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3donohesd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3bpzbmcbd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3slunnqoj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3pacqyabz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ilavtxab.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kwhbprdp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kqcuueit.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cjibaqvs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qhxqwgzs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3adgjjyiz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3dhbxlwbi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3voqsptpu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3bljtfgdc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3huldxfmf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fytezheh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ijuvxblq.html


<!-- 参考信息 -->