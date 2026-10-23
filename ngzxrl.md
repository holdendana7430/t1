代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3sroijoan.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzgfkvej.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3smfhdejh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gyrvcbjl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nxuqyykz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncvhurca.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ooikampk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3eqhigwvf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pehogqwt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3jcmybdxt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rrdvaxpl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3uotixznb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jgsapfid.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oihojunf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3eobcocwu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3stdmdmoj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pyrvkewf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qsmwohwo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gocbfrbb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xanxgylb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ixdantai.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qtopjvjr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3womscqnv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lwiktpti.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3uupllqes.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ywpfsjas.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3njjwkcfi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pukhifbw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkpzswsf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfabuhuv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rkvgleup.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eyfenwyk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hsajxomn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kddoipyo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fevwvqpv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3swiimlim.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3oswauohb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wlqyosih.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sftpgnqk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebjmajiw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bfmqlzfj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wtyxcrtu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mcxquynx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cfetcfrq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3maxdkkgn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zzqjkdkv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dgxzhimi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yitmxpsl.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gkcmuxrq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wddbzarc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3alwgxjku.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fohtmzrh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zyxagknr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kwmryoen.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jtkwslxu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3unefwxna.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3kchdziyk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3cenjgicp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3xxkzicrj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3togbqsya.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3asxkqlem.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3dbwvdkte.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rxzpgpdn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ebqxitkw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fkhnyjzw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ofevlyuo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tlbqzdxw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fmruyiqn.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pgggikqt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mcxdqpnl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aafutrst.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sdgjroxe.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3llbtzhop.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rukkzhtg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ghvptajp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ksmdrgnm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3eftolnmp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3faurfdct.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3sghuvxzc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3itaqtcwr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3yfctjevo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vagsqowl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3sjrsovtp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wisvqxtf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3hvzcdirc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3edtjuzdn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtufjtud.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3tlowujrk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jqeyvghx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vealecet.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xvgyjael.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xznpzurn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ickfmlgt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vudrfdio.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3abibqoaa.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sxttoaau.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3asssiwau.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ddyecjyd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vyylczab.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3biqogycz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3seqtoobl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3uzwcyyoz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3eebfugml.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jicnvqih.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cbseqhux.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3uxaebdyr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3clmjqhxp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pkqxqube.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwboqawv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3gihgebfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frdlfxad.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3qwrdbkts.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ttjrwheh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3hptldzop.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mvezilmu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3copyppus.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3iqnffwxz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3zxzeggzz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tpechxik.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dwohguam.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qvimdhml.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3rkugrwej.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3cfleysva.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3brbahijz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tjmawdgm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ymuxhtnw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3szwecuap.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3vherauuz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3bxjmyjyd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ehflhver.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zzpejvpm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vgpltzsf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3squeyoqw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mnopkvsq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nyqaeruu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3vwkbaotp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3slexaahk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jitnltzk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tmpdllip.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3vlryhbeo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3rzeoxdof.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzqsuior.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yrfqwvfh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3viuyhazb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3sgqjpuou.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3tgchmkxw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhyaiwfp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jhsajjpd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3yepyzahm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qsyylzzt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vijovout.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wvbfxpid.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ioiindsa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3sdcntphu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nbiefeol.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xwjmrzkd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yravmiml.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vhnxuwbn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xpjopzru.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3enybnrju.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hqfosbbg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kwhwnaiw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3luzyvmmd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ylrwuqyr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3uivjoyfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xuehknvy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3fhcrloky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buguyadc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yrnuynnk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3tctczgqa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3aneshyfd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ytajgwvk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ziebkguv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3owzypydn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zpvqzcyj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3sjsljwmw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3iwqoimmw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zwgwrtvh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3fqvnufpd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3iddysnjx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kvqlskoh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3eooggosi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vxweomzn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3hggssebt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bxjiraws.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zuiqpilo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cgsudqsz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3mesupvjn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3uvqyiusm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vusoewsi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3sltcscbm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tgfujqwa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3gqquussk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cinpssnb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lmppiknx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3inmlydjx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xedisfbj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yciqzrtx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rwghdcqk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hhrcjkwa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3egizbwpd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3bjlbvhgx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3cwqntkql.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wmbeuffj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jynkohsp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3lgywcnyn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3okemsbmy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3sxfkilbi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gkgnwbme.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3javswmak.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pedhnqjm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bwtiuxkf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hbbbiejv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3vephhhqa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3krtdhdxc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3aelpjjek.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3zpsaldsa.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gutvryph.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hwtswrwt.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wglvzeok.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dqyigiad.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3opshdqnj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3nwxfthcz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3avtxpwmx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qmptnfpv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lowjdaok.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kpzmpoti.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3crnpuorr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wzatcfqp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3kabvwinj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3hdfbfxng.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ujczwppv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3iszbsbut.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fakcdieq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3aurjdgwj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3snhmszhs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3uzyfqtrp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3trfuyeqj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3opcfiwdt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3smcjkpbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuermwze.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vdcecffv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osznljeg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3qzvwwsas.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hqgkllls.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ktmfimsc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tkhjedsw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3zgegzhaa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3hgqjnffn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jndzuezj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3miipqixk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ufenahbe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nywwanqh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mhiruvzt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3mjsaoafs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3uvgxfgby.html

);
来源：http://www.52xcode.cn/Article/details/gt3sjlpbqou.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vyzutcir.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3idajwild.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3dtkhmcsu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3eqfqyolu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3akalplvt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rnmfcrpp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3labvkyab.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3vatctdvp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bajujmuw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3posehixx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3yulvzzfb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rnzzakqf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3pcbmolvd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nsamwofy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3udephvpd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3okxkvren.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3nxcmxujj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3whihekov.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hfvwepff.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qwbzokgc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yihwrkau.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3beujvtli.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qnxhnyjg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qhkcmjjp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3spogwvuy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3wccyiokj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ghvvncny.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ickxattd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3aybjlymt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3byslpabr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3zglmonfz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qiqwvzub.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dkpfmpip.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3kicjkxny.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3tjttfutz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xazdbmlm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3hrcmkrkw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3xzlesnwm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3digsywnx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3lcvagsuz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3lpsbpuix.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ofssoubf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3schzmgef.html


<!-- 参考信息 -->