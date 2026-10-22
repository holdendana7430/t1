代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vrcvsjsl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iqqhrlpl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ltbcokyt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fgurndjl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xppplizx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2wjcfjgvl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zspnzapy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sjmkiukp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qbjbzrde.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jgfdfxnd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nsoproks.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bqdtncvu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qnrizuvf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2eqvgntmc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zruoxerh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jznzhagr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2olegbkzz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dloyszzu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bjmkyucr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ldkmqnpx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gpblduth.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2opwapqkh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2iptfgesr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2nqhymmsn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mtuldhgr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2htbvjsjz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ctwjxnvq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uhjfoykt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2curnvofj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2oswggmkn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lulejkjh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uhufdopl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nnttadep.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2puubvchf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2upsnzkly.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2aecljmuf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xzgxseaw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2fupdxsqd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fszydvoy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uvjnikfn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2jegvqgwy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2owrtsvjn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ijyaxvpv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gmjqrjcd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bimtmtll.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2racjxrhj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ohjyiupk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gqhpjpyl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ahkifaca.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ahqgnviw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2colebhog.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hzskyrso.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wvwvrzqh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2gqjboklz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2stbbflgb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2junsnugs.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2odxqccxn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xmmrrncj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2znefwhlp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zquivrji.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2lcezrksd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kqzwcjgp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2phpdacpl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pfucdjzj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tzlyeiyp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wylajbyl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2buqlvonq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dwlhaunv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lmkprrnm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uxbgjlmi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sdtkwwuq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ezutuzhw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2drndqzzf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gwqxapjd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2svvpmdow.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ktxbukgc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vlwnkjrt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2gcgvhtej.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2zrddsyeg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxohdvpc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cvbiidyg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2sycyfuxl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vzwzkeps.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2lhngcivh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wuzmqdef.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2aaeeclxo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jujklrfr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ipjbtzuv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2iwilavuw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ijggnaie.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vtzegwvv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sulgsihn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sxiogszh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2obbfjbiz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rxdvgtep.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2zuhprrjk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2jqjczzrh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2psexonnh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bwnnmwwy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ghxrygqg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aegcykmz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kefcfxhm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wvssjjsp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fruzdzpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhhanerj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xmkuuplw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sihtoktc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ahknbkdw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2luzlijxy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ytdeioaw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qylpihjc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mhtalakn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ysyexasr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lvotbfhv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2zifshmhn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fjbjlpvu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tyjwkuzr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ddxqhfpr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zveeuemg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dgakyxjo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2huerhthz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ycpyokqn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2czcbgiuu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hdxrgfoh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2irofacio.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ycfobfdw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qzxcorvt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2elfquzyj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zafdqhuw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2idnqrzcd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2auudgtom.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kjiiqbze.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2uabizozv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmpojlfc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2tsgyowvb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2afxkpqkq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2qxwiptew.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wbhxnxvn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xxmrfnvt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2czwcpkew.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xrjcbuul.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2abmydpdo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2eonkdptn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2umgehkyg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qmdzcenp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2rxlspfql.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sumgsens.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vnddkahq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2vtvgfihe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zdujtcsn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtfvtoo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2azqnoyfd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ddgndowu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zplfmjkq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2nngxgxwf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ppzzxxuj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hzkvrmxa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2soxhmedu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2upaojykm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bndwrkuh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2fdvkwnks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifkbjihx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2rovrsklj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhyexbyg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ezxlzidd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2excvwdim.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2befakswj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2shmjecmf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vtmriosd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2yejvsiin.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2xhwzliaw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fobsjuhw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gnaxkybm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2uuxylfno.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dlzakcis.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cobprwrp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2sgvghiwi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rquywfbk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wdygrzge.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2epipxxsn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2angqwqxa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fmziejjz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fgttlowl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2aawbgzvf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2sltmahcx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lbztintb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ooppzllt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2wvknajcj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2tnzsstac.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2stsbvmst.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ovjgkzih.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ztowmatd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ksotjkiv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mcunwfme.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bmekmdtd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ekrnhkuj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kcczbhog.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wjrjfdyu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2yfvllril.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xyadfviw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qxmuuysx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2lkrxgswv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2rubaeein.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2pnmfwkqe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pswhnqxk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2erdlzcrb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uwyckgku.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2petjnrrg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2tlciytsu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2tagtoewy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zwsbadgc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmuvfqec.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bbvjppfv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnlrmrge.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2utuusadj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2fcfyoraw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2bwljfmgo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oodgehgw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2kskvsjoi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2grdqdyao.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ejzzykfx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lawbhbzp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dztgcabo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2goykvdqh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2fscmbjuk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2larlpagl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wfygozmk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2efmzdxqv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2tmldoemj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xtmfjwid.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2wlhltmjw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zwklkyls.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ivadjwaz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2llqwptit.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2bkhthdpo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2hutsaayf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvpeajxq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tqepnust.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dppoxxih.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bacrbwxo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2kkzkfycj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qtzrjywy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zzxrwihf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2hjlwmaad.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2bfxhrtse.html

);
来源：http://www.52xcode.cn/Article/details/gt2hmndzynv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2jkdftqxy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2fqcnbwtx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2czjxaoft.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sgymoyll.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2abtovyes.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2csmpylgp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fdmsanwl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2uhxzcxfg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2pzfefwrg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2puictmmj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2khsoubvk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2gslyjytl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2akugtley.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2gljdwyat.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ogjxjvzz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2uvnfsgpa.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lmcmedfc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2njqpvfwe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2aiudrawd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2dcjvdjkd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2akzmlyzs.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2dipcgiin.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dsyzypdg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fblbtmuy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uirdnakq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ixhsvzzl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2mmekslwt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2qhmufddi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2iayoyzlw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pxebzskc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2tnqwlfsy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zyitfttx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2hrhpxzzb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2prqypjwm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vvsjxbxu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rsmhmsdi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hfiybsmd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xjtlbqbf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2msodbscl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2evxkbjpa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2zyhkudhp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2wqnmefxs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vpdruwlk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2kipfrops.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2luznjqhq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2augsekwu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gxofxyda.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2myzsniss.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ahzmaxka.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dblworwt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2psztgvqn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hxofxhla.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lanchlhw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2yujgatql.html


<!-- 参考信息 -->