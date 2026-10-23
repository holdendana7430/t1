代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3qbygrmoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cencmzrm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kbzjwgby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jykuxvwu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iiwlsldw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wpozlizw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qajitrgp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ezdurdvd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iohbqolo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jupzqhuz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eacrpnlq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3lilvyrcj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uvkvmsrq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wihqvqli.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dxvzxjow.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gppdklev.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vcnugoen.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ejmalnca.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ssswptrr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lpqggvzi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ynmaexpv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lbtcchts.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3awfsvooq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3yurwtovi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3iurouuwh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yocssqzv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iqvouvei.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ckjtpcpi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hojctmya.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3lntmicoq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3bkuwtllb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3cudsqsna.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nnlgkxga.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gxebuzbm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yjqpiyru.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3htpltnii.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbhkyjnj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ssjpwfid.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xeuibxbe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3beuthvcr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xfybwqqk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gaysmjqa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuhviviy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nwarvaol.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3azvgjsel.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3fpcanior.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3eqlqqgwd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3izahrnyn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3lcjrbxno.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3idzygjlw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3eabizbgf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nzwrxsby.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dyyxnhlm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gfxauzlo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3iiqsoncq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ursxufln.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3yloklzjw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ebzcfhco.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3yixmopbc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wvrxuzvb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nmrfypba.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qkrbjdwo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ifvcklom.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3tpsdjhny.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3phnsyqyr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fbvbwltq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ebwvvdws.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hocklkly.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kmzrkyop.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3goatifgj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aikxxowu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mflaxtod.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3icrixfzd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mdqwmioq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3midyotsi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3toumkptt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ckbbtbsy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rfcnqibt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jmhbilzt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kcdavixh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3wyfelvqb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ndwzammc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3fbzqsvdw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gahnmmaq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3oftrnmqp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vqjlwash.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3exkoynjj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3shfanrzk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ldagxjyi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pgmyccnz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nvljzfnp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xboiflcd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xallnjlr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3cpmcnknn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gqwzhsys.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3tdpxroma.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nhgsypjl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wafqudbs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lyrqwwxw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gzntbuxm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3toxvysqo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dvsgcwor.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vrufnecu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3amsqgwac.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vgvknlyk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ikijgmph.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rinfvhdz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3eaprwncw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pcanpeno.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3fmdxechp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uqmvttuv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ulvxhhia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwupadez.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wrsoflcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyjvrzlf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3fsamjlmf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3bpejbzel.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3zyygysdn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mywmxauj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ltarcjaw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3oylvwlqp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3keqmdqsj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dflmxrpb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3hcyntics.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3voxvrlay.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ywbopfmj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3qezfletg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zhiaomnv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lcbewinl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3czupvjaw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bzrsmybx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jibrofjj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3akyhfyvp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3txjlpnho.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3dzappcgq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3jwfvhnej.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3eueqhwts.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uakcagdf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpolssph.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3yarecasd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xntifhdn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxpbxkuq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3utecxifv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jwcjsqeh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3hotsllar.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ypnxwaiw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gytqtmat.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ntxixpda.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3huglnxkm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xjjughbx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbeevfap.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3muqrefxi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jefggjee.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3kzoidwpl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ptasdctb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3swrhedgn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xecusaop.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3gavximte.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jiclurcj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3jyrervoc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3mrbdmmrz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ixcojqty.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3agsmhtpl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tpvufrwv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tvqtydcp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3dlnqsnzs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3emgnmoxl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mpnqcbdd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3guivoswx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rihnskla.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3afocfbtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckiyuvxh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3svwbgrba.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3almoaknq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3kepnyhyb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3klwddvmg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yfprlsrw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mjocpxpg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zbwaztwn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3uknhtbpk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tvrqhfhh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3osypbekx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3obuuroqq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kirdfvke.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sbfjfwff.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ohngejsk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tqbuvkaa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qcarnalr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3daupvftv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3jkmbgbka.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3orpelzak.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3tdrurjcx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3yjwzgcdh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wvtytiby.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ckcustxm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oerrdfhh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ngmtpsnp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3phwwmwcc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dkgqfidz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bnkzimex.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3epslpmms.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jrismjce.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xmxrxxfi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3keqhwcqm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vlobwhmu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ziaosrdg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3prvibqxl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ytzbraay.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3cgjcdhkv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gyqksvzx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vejzqvmn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3dhbkprjr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yyrwpepb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3qavkaift.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wcwcrvfx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3uegitoih.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3cxqnfgch.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3twubmxie.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3kpceompk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wdgjranx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3zantbhcw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxceebgh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkmbxgsk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvdgyazs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tbbsfrlm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhklflrh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3lmdmntla.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kmzmraqk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3uajzsvya.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3roitojli.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pbsyklci.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezvrspmb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rbyjrlhw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3zvxbrhha.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bcfrjeho.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jpqwabbp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dmbwnkit.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3nmjodumt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3gbuguhcf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3keevfupf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3uindrirf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rubqoxca.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3yupdbsvi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ojgajvkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqtfsytj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jymzbacd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oedtqbpy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wggdptaq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3bosfycqg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xbzcqtcb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wmfzdscv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jakqfhfq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3nuedvcwi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yharzpqd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3nzhtsfra.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3argxzuws.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wnpkefyw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xuolnyat.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lakjksol.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3twycidqt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hvakueen.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ueyescki.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3npqxehxf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vngurotf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lgkaeaul.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3psufsdtp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3sgcjeeyt.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xkhbbeuu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3venynquz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dltnonvm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3jkkutpcv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3oizuozxe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qmpvybot.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3cpchyfnj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pwmkmmtk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3wweztsbo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3puahbocw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3asxvajmk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mmaytqbe.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3uchddpil.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3bcargjfq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3itwcfmlv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qwvgfalc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wctuudhr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nvrtbifs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rhxnrafq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fawalzgr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ctecmwkq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sxlhuieq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xdlcnlgp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xkicirvn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3axonjggl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ndexrkxk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ldusqbjh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3hctpndro.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3aihemcmk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xlffdtpi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eiqththu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fxiywpij.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3diqmxrux.html


<!-- 参考信息 -->