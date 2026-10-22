代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2leubiupb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwpwonxj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2nmbcgezc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ignsdqap.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zdxqxziq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bnzlwmec.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qvsnbytw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wchuqduh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yccrsiuo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sqieivrr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wodpspwr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xhbwpnvu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jopegfpj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2sogrgwox.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zwzqfxyk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ludfwwxf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vtgvldrd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kkzeltyp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jhndhder.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edctynsi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ibcngrjw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zsbibhyu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ftezdbsm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vfvdmzpp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2lxxmdict.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vmygnqsf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dfrbifsm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pdyywdtr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tjeoylga.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2yjlgjdrl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qmfjneel.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2fcwbijak.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nrvzdrju.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngfwjcse.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fvjehkrt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qqlvndbp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mbjxhsxt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2mobgjsad.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kfkygyhc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jwtjtqiw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2igvwknoz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sfqvtzoe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dhzsjtkx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2izzxbmvd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnhvanyb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2sljvgfqy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xdauddrt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zkpyfceq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wykaakhx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qvyaujud.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gxwugzzv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ftkzqbin.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kvyufbfm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mkikjupw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2elusskwg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2lzdwxzlk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2acdxerec.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tqbersjq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wfqlenyj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2upflnbge.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ddyrvncq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ajofsrjj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2rwryikkt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xzedpokr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2svhzndwf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2lmbxkffg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ajlwhqkl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vpifozxl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ihqviojd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2npnbmshl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ilszzfsk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2olygstlw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nbmjjolo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fkxfqfex.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ebyqbtch.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gkcuihyo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uqkmsxbj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2naycxodh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tyargziu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rdgupabw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jxchsgvt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ugnxhvni.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2oimqxicu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ybaknqaz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nomtmole.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2judejsjq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2kfnhawfv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwsckekw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vowumnmg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vblsvvxe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2phtgaywn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fbrzvney.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ljudywlm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bekdlsrt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lelxgsbv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2uixmufav.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zpxkbghv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gnpntkvk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hrlmbmmq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tcmkhrbu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ywhbxcwc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wsivzviq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hfdnggto.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dqipyedk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2brpumxee.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2hhayoluo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tivttvvi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hwaqnuyf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fzrosviu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2dlpcreqa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rpzewexn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tkqplbrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jnahfkbv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2kbgyiauy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wovzdiha.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2uxtgyzfi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2sgwlvfnl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zyjblvpn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2rxpnfdiq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nahwbito.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qjvrbrcg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2tdiuxpyw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2wodlwxvo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rldxkbkw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2osxercsa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hzxrpvgr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2aqozfvhl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wvuyzekc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mqqlfckh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ytaqnnkt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rlqmadws.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ehjpryej.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zmoibtzg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bdlrpins.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2sktmmnpg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2nnyqmwzl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ecxqpfql.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xqcgarew.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvtsxxmd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2whuwzfhk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lekdqtyi.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2eqajfvtj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2otnxbrtp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mvvsxeqd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dylpppqb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzgryozz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tarckrom.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ljkgudvk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2nbaggvzp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2bnvltbyu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qgnkmgcj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ecsbuvij.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2exrfvsui.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ibhgkcgj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jeguuvhc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kfjurdec.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2szxjkujk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2cdjfagks.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sighdkzc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmcljksq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zsnyuaph.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2datrmyjm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ixmguvde.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lsxkcmsv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ilecmcss.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2aqyfgrwc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wlianztg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ehkgqawp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2bvdqiyrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qexraasg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zjhgyigi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abgvcyxy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2duzojwoo.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2cucroadk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cgxfpjmf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ofadxghb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uehdzbhc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dqholvnl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bmckbbtj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qmmnfgtz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2evzddext.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2odwqmbnh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2znfpqqcc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vzwzdret.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wsvcfbeb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2klkdlchx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kicspeuk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ogdcmgej.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hymcvvhz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2seueajyn.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2vclosrxm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2yhotmppg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tystlqip.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mqevjocr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wgudagam.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vuexjzhc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vufjjzdr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2kqdxlgsu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2cwqmpihp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ibqxcpih.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2pvrsgmtg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2otacjrnk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rdtmeaew.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2uhxatuly.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vysghznb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2wsyifoym.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2tkdqangp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cxexmnyr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jxycbmjj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rfgsrefd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2grjserer.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2syxaibhr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2utamsoml.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2kpheicct.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cfmfnnsv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hzkrdwoj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2mleqeber.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2fcwuetir.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ispgtdbw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ifvyirbn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ihhfreut.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ezphpaho.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzirfwno.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wacytkwg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vgxfuzxa.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwngtpko.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2abhjlwmf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mjkthhhc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xfjxuuaz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vmsdunpf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rdcbubim.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wogjkkil.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qmjraftx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wqcefrtm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2tlethobx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jxnhkjui.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ewjldftt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2csuaqifk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zmrfiyhv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hrllihxl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wmacjhfh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lxbkywdi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2abqtznxy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mgdjufov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrfrkdsm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2amfnngox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mahclgte.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zepebxgh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ybyyiraz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lesdqegq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2txlhjjti.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2taoxgnpq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2teqacpel.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cfegryjt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2kuwdcakx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cgkkdzou.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ajjuelmp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lszxacqh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2buntydyo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xfknovek.html

);
来源：http://www.52xcode.cn/Article/details/gt2wklaefll.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2rkmytgmy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2tmogyfne.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cihvjllm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vblyzrxk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ntssyltq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ccbxvwqd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fftgowvd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dwryxxen.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ttjqlbxv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bbpnnbgw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2kprrzycl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2eureglyh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2vmuvonym.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2iafrtqtl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mxiigjud.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rbxvxxgs.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hunawvgt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2moseolan.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2glzgatou.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pvlcshvc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ujqwyxuz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2pgehksnn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iuokydtf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2owbnclzi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2puirfsfw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bznlrqad.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2qbauizqk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dunpcaqc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ldthmpdb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yqczgmyg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2vudqvjyb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kszicfhr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2pohkspqe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2gglhtsmz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dphrbmov.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2sgachapt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cjcxbuqv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uwwydcbf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2zbskmejy.html


<!-- 参考信息 -->