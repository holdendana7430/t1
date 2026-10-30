代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsdcvage.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fanxiaobao.xyz/Article/details/gejsppgmk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gyfnktltq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gyvhhgqqe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrsdcrcu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gcephksju.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsmgevmc.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gfuuxlxls.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gwhdqccuu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmpmnvsm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqslvcqcb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gzidyqush.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fanxiaobao.xyz/Article/details/gqfqqruuw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gyvlqzdik.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/guhmesybv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gwktyausr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqtxgsqn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnnkclva.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmcrtuex.sHtML

[N04] 斐波那契数列
来源：http://blog.fanxiaobao.xyz/Article/details/gmjtrwjgf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gfgctcehk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fanxiaobao.xyz/Article/details/gdbtwrbes.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gickkmput.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gedtzsyaj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkqnckmw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fanxiaobao.xyz/Article/details/gppeqhdsk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gwohetraj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmpeitur.sHtML

[N05] 最大公约数
来源：http://blog.fanxiaobao.xyz/Article/details/gvhqurfoq.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusvsnbnm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gshskayyw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaazslvzv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gngjwnpbn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fanxiaobao.xyz/Article/details/gdqgimcsl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqyegplg.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnrudanq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqymitask.sHtML

[N06] 判断回文字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyljxyzzf.sHtML

Py:   s == s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/gzkhbtgfk.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fanxiaobao.xyz/Article/details/grbhwvcob.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzswmprtm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gkdbuxluo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxudrbks.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gnddvsaux.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gxftctukv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/gzrileyuh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcifxphle.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fanxiaobao.xyz/Article/details/gshpmbojw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpesykrly.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fanxiaobao.xyz/Article/details/gegatkfnt.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fanxiaobao.xyz/Article/details/gyendbnim.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldjscqwo.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaodtcpl.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaxoxovy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fanxiaobao.xyz/Article/details/gwsanhfbe.sHtML

[N08] 生成全排列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grybnhqmz.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gszpsviur.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/gehvjjwwg.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgissgmb.sHtML

TS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gsftsjjcn.sHtML

Java: // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/giprfbmwg.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gezhxcbpu.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gbswzpjlc.sHtML

C#:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gibzrqjha.sHtML

[N09] 栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/ghazjpjcz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/grwmvupgg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gkuxadaus.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gxhbknuly.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gevddopsk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gytqwpriq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fanxiaobao.xyz/Article/details/gaqqrsbtj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/ghptiwivc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gzuxklqut.sHtML

[N10] 链表节点定义
来源：http://m.share.fanxiaobao.xyz/Article/details/glootekfb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgqkqtam.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fanxiaobao.xyz/Article/details/girlntmpy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gefwzhleu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gmsgrenex.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdypcgtc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fanxiaobao.xyz/Article/details/gafozqhoq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fanxiaobao.xyz/Article/details/gktfnnesi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzxqoxepu.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzuuadsq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fanxiaobao.xyz/Article/details/ghcoeledp.sHtML

PHP:  // 手写递归函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwhmxgmtq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucihggmb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcvbmalr.sHtML

Java: // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgubdifn.sHtML

Go:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gheuzfxlv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fanxiaobao.xyz/Article/details/gvqrefkgu.sHtML

C#:   // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwjzpbdu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fanxiaobao.xyz/Article/details/gbibqemqc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fanxiaobao.xyz/Article/details/gxnlqyvcw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fanxiaobao.xyz/Article/details/griueihzr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gjnqagyad.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gharxcsip.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gqeodyouq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fanxiaobao.xyz/Article/details/gtusgobuh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/graisavta.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gsfrxsosa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjxvpvug.sHtML

O. 并发与异步
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxupieqy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiduromq.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/grlmxqbpe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gspndtedb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzhbgcgx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhhuoebs.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpevajuk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcgifqpg.sHtML

Go:   go f()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzgukkqf.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrrgnfvv.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpwkxmoz.sHtML

[O02] 使用线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gblblzinj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gttjxlzgn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlvaikui.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtauzmzh.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/geuduyxwv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fanxiaobao.xyz/Article/details/goysguguo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fanxiaobao.xyz/Article/details/guntmvppz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fanxiaobao.xyz/Article/details/ghcdlbdmd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fanxiaobao.xyz/Article/details/gpizuybmh.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfvsekhf.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqqhofpu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkvhfdyf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fanxiaobao.xyz/Article/details/gsglmjoex.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gpecjgqjm.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gljmgdzbm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fanxiaobao.xyz/Article/details/gigdbtsqd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gtnbclhxy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggldrecnb.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gxysxinyn.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlanjphh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fanxiaobao.xyz/Article/details/gihabbuwd.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gflzyzaxi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmesymulb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fanxiaobao.xyz/Article/details/gwmptciys.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjcmusqn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fanxiaobao.xyz/Article/details/gxhqethub.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gowuahyux.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genbcuxzg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkydscey.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fanxiaobao.xyz/Article/details/guagidvwj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfkzquzn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfjffuti.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fanxiaobao.xyz/Article/details/gbftqeokz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdjrxhoo.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gyhlpcanz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fanxiaobao.xyz/Article/details/gyprfdnnv.sHtML

[O06] 使用进程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnphgory.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fanxiaobao.xyz/Article/details/gxohqbkqb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxwjcoya.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcpblstn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktzizofe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gwatmqzdh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fanxiaobao.xyz/Article/details/gufytemmi.sHtML

Ruby: // fork 块
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcwccsnd.sHtML

C#:   Parallel.For
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmlhihde.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtoscfiek.sHtML

P. 常用工具函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpjpcqrl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghdtnsauf.sHtML

[P01] 生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdxtqcce.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fanxiaobao.xyz/Article/details/grnyxqzux.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnonahgh.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/ggpcqvuji.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpljbnioc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gadcytcog.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdwksgqx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/geugbmuax.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzolfztv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fanxiaobao.xyz/Article/details/gwclvrssn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgyzfdeh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gbmysiget.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqgvwtri.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeorwjxe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgavhtrq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gocwstzip.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gyljeybee.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcktiplx.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbqtxnxl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjepcibyw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fanxiaobao.xyz/Article/details/gzlgphtyx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfxshsox.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaspmmowc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fanxiaobao.xyz/Article/details/ghacldxwt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/goqvmmbft.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gganbolyy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedfbtejj.sHtML

[P04] 求长度
来源：http://blog.fanxiaobao.xyz/Article/details/gvxoxmtiv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugmocbzm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfxkkevr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmwcfwjg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrmgrohw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gfoxfekwz.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fanxiaobao.xyz/Article/details/gxkvgmvif.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyxkhjdf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/gquwewxno.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrkwauls.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfhjlxgq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fanxiaobao.xyz/Article/details/gevmzkllm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fanxiaobao.xyz/Article/details/gsngmtjsx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gspakfoqp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fanxiaobao.xyz/Article/details/gndmnrnyf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gyvvfsfiu.sHtML

Ruby: a == b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjijvbdmv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmqtfxje.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvagbhth.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlyjeuii.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaouigga.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fanxiaobao.xyz/Article/details/gzoysxsib.sHtML

TS:   if (x == null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gsibllspu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyebykqhl.sHtML

Go:   if x == nil {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqkmyqtvi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpkncrof.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmdcutzm.sHtML

[P07] 防抖与节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmyfqdhk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvqgbwxt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gahsrztcw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaavejqc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gixwptdaw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmtuladz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fanxiaobao.xyz/Article/details/gywiezrwt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gsclnaiha.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/gjvyuqktu.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbjkmfdt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsenznij.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gskftaube.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fanxiaobao.xyz/Article/details/gukxrmgpd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxozbimcn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fanxiaobao.xyz/Article/details/gdkxdlgjr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fanxiaobao.xyz/Article/details/gluzptcso.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyzettow.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fanxiaobao.xyz/Article/details/gfduizlal.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gujgwkjrr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcluhidm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghhauoezx.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/gduzsyzpz.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gnatjhoso.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwqnfxpi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcetrtzs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fanxiaobao.xyz/Article/details/gnnygplig.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/gswooeach.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gsdzqtkmp.sHtML

[Q02] 创建带外键的表
来源：http://3g.fanxiaobao.xyz/Article/details/gsjfqppep.sHtML

CREATE TABLE orders (
来源：http://www.share.fanxiaobao.xyz/Article/details/gceahelxk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqaquarb.sHtML

user_id INT NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/ghebalyac.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkcjvbgw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fanxiaobao.xyz/Article/details/gnawhjcip.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxnzlpee.sHtML

[Q03] 增加列
来源：http://3g.fanxiaobao.xyz/Article/details/gsonlslxz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/glnlsjzqu.sHtML

[Q04] 修改列类型
来源：http://wap.fanxiaobao.xyz/Article/details/gfbbvzjbn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhkkwmrl.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gfpyhquyu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gygcaeixf.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnpnwfzq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/gjlvxxssl.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gowplnqpv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/geljbbysi.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gvenxfwxu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaaluzvo.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/glizivcmq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gilpufwgk.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gtqsjbnjw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfbezwvj.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsfpraie.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyhixsgl.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmvmphen.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gvjvchkbl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhfofyrs.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gtgonuogv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmqkokoc.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/gitudmjgs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gnpsijfrk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqndxefs.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaogmbpxz.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqxpbctzd.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gwuncqddw.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmccgtxc.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/ghdejxpea.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkylyumq.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxnfkcwy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxagawcz.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gwecthjri.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowiqlcbg.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gyihffyzz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gvgsjqfbc.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsqfxgxm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/galqndaau.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxpywjyd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyguaekyk.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpieqfgps.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzoepcrq.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghygqeicb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexfggcym.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gzgennyzf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/grdtxajkt.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhbmqcip.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjwelvbj.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmycthqs.sHtML


<!-- 参考信息 -->