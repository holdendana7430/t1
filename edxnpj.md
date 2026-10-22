代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2stqbqgvi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpzvflqf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2azlahyuo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2lkohknvl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pizqukvn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2wssjyqoy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2njkndpje.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vtnxijfk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ltrwgaur.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pchdifce.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2efftrsjk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xxsvyznz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nbqgveta.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2pmzuvqeg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2evkyxffk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2duzriodj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wqtssszv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cyizhovm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2emkraevh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2wzioydvd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jwdprldw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2publjbfm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uhzdxcfs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jrtiwapc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vovzvjcr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jqkdziuy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hdfemubd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fhdlblvi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eheskois.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2usjekmyt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpfbbxqn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2avbhzdja.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2uugejuis.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zvnomhgg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzuoxdce.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipimtcrg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wcaarecj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2jtbnbobz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2svicunak.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zrphxucv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ffdamftv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2nnjryfhq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2liseclsf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mrcmxcwe.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2omernkxg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2znzgheeq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2myvitlag.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2phzbswnf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xocrcmzs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gbbofnjs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zilzaulu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2fmvktrzh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ignbjzxi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wpqaykct.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qlvbbbxr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ycgvozlv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2awdhmysk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2yklzkpog.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2olfxbbtw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2xcvazifz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2lfrridgz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2aojlaxga.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kqcflgcl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ixuqrvaj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ygshtwde.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jmgviqth.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zwnwvciy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dzcohqdd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yuwmhdfg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tpbmwfww.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rxfnubdh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fmpizmif.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2moggojrj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dplpfkxn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zijmvwsy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qjyeyhot.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dclvgyoe.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2orlqnzst.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2tuglfomr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2otenhnot.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2edogtuuu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rhxhcztc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2lqaqdkhk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2eoecooyf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2dohbqvsl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmuulaav.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2szdcznht.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jfiznnut.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2zlnsuqwy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2djqekdjw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kuziewyp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wozwirkj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rmopxotd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hqkkmeie.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wnzcjzrc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2pusgxukm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2pwfyhzbq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2lnbejewa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lgfbhuoo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vzjuoumk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pppmudww.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2uppvxspw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kotqfmhx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dmqhoohv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lkmbauty.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2iuplenct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssebgcnt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2cdwaecop.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2temvfqap.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2yusyiapo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ikrbgnzb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2emjkfmxd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xkebckwj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2vvaquzkc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qapdktgx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2epitysot.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vhhcsatr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qahbmslt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2jurwkrmf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jvquiurz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vbisegzl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lrnltdpc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xhaintru.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2slcmtcin.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gklzlwrz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2bnpzxlun.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2nerjgcjf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gexxhhng.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jinysubr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ysjxwwlq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjqbvnna.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zhuaxczq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vlgmponk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzfmxhbe.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2fxrpkzif.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2azideruy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2puvyejak.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2azqbnwwk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2shstasqk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2rvtbnomn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2pnrkxfai.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lfqifhto.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsszzjan.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hnyvdqkp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2icehodwo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2dvkbxrao.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2etyrobpb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ozplzaim.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2vtgobpsf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qboncxbs.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2milzpydz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bfrxeiuj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2kxwpifpe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2bzpmudro.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2icfktvks.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2iafohszq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kemucgdj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kuhxppbx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2zwpoirjf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2iankumjr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2bpzljlpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvgumolr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2yexhqvpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gehjmtzc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jvpwxmwq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vseksfqs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2zovnvmhx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2aaiezyjp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wklgsezr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2knmsbjuu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2udgllfls.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pvfwajwj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xzmyfrcv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nlrxsbyi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2cdejlcma.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jqiffgry.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ynjeopcf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2druqkfts.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pgkstorl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hdxouihw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bhicdlxb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2pgfwsicz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oeprnqbp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fijtlhai.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2gkyajqqv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sovtrenq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ldolcprs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2zfvkzfjg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2jtvylvfc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tknelbiv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2yflqrqra.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rtcazawn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nrwdejer.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lwkaayhy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zyeilszk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pffnoofn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2woixezff.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2zwikasvu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2sijjnmei.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yenwjawe.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2abjekibm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xpiwzmoa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2gqnekkjm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ckzwctmd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xyiqstsz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ohxnxnas.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hjkxvyyo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2fsgurfvk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2yymmyuxw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kijcebuw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2frogdget.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsvxknln.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jxsugouu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ledmhvvb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2urqdxyga.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2byqorrhn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2tznxwnhx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nygtlttl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2iuchibou.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2scaprprm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kroimwzo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yhvangeb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2igcqvdkl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aurcnptj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2iueeaixc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2grkksagv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ihxpjyif.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2kmubtsqf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2yffgndvx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kvyqfsrg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2bumpyric.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2odwxovvf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ahbiarze.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2iahsemlc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2cyeyzxzo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ivlcaoyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxatgshn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hgkiygno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcakajvk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2dbxslguv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2echtaldn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vikzyuez.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kkajroqe.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2hqzsnhnw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zarlrbkn.html

);
来源：http://www.52xcode.cn/Article/details/gt2llnskypx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2bcwvnsda.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vphybham.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2shlfwizo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ydlbikgo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2tsxurxug.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2iclxdvsc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2aiythyhj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2wsroipyo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2njsayskm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ijktgueh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cllugggw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2oiejhvjf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kdydchat.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mvkodgmj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xlrpjksh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2lizhgaem.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ycljdakd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2unzuhtdo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ltvclnzt.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2sjxuintt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qabbresn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2eflhczqh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2agwphpjr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2aiygtylf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vzzrlglb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dgorfpig.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wtyftjtb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2egwakqjs.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2clacwjxn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jxpuzdts.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2swecjreh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2eqkqppjv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2uekllije.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zjdoyzdf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cdnmgvzh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2keatcggf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pokqosol.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2yzoxjrlv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2slwqslkh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gtmrampy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zhnpslfc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2jnefqcus.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2krwepvel.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nywzybjj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qaknkxpd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2cmomyfey.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qzwxydzs.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2exjeqegk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2uqyyrkls.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2khiwhzbz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mneknmdf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hululhec.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yuywqgik.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zedxkgvq.html


<!-- 参考信息 -->