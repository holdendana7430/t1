代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2imkiclan.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mqeainel.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hkpvabtv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ejhfrfkf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2flltlrmk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2grvsgahf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2dgoosepa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ovsqtmtm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2iimrphxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywikmeyy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ioiyetkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uoebwvet.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zjpdxrns.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mguvrjps.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jtbracmp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oqnudsrc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qqkxxqam.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hrsyrrgc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mpxgdkap.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wesnrckt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tgfptyqb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qxvcgdaz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vecmpbgg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kywzduqk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nnxthcua.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ktemmpwb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hxojchco.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nrqrxufw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zigjqopf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2amimealf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wpzoithm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2bhovnawi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2wmodrhro.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2prgjmqdz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2exgdrggp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lbkmlfbc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wdapkcmr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ykcpslmg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2suayjsnt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nbhfyquw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ntcmmtiq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxdpxohs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kkeaxjrj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gkydggdv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tdrwfcnc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vnrfwgef.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2eakitkvz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eacdqwig.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wbdolbpf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2glejhrdn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2avdwspvl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2spdkdabg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mkpgzatp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2itlwkoan.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vwuktvop.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2kaysqfqf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bmbkuxwu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wlzfrtkv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vddprren.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mnauavws.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yfsktltc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tpwohojf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rkcwsakx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2aqmcyqcx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pnlpnayc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ibebtfhl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mpadivly.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2obbeclbc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fekzjpfr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jistawbf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2kwkvkgpn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ijrrxkuq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zjchrbhd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qpxbvznx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tcojnlmj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2obzeviqi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2njknejir.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xxndawug.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2emhovxkp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2obocaqrw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nooftgas.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kujljzue.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2tizgwjkh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2abvcgsps.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vzfyhkmy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2doxxqomh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mxhbypvi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pbpzojfc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xmqbpfpu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lojkloym.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rqgcszld.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mwfubxdi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bpodbeyk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nteusldo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2extyxwor.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ffgqzemb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cleijfzv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2corckmfm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2tbibmges.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2prbswlmh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2npayucec.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2tvdjvvrm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xpgvrpst.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wijdspby.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2idowvuyp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xpxfjjav.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wmkjbacj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2niavkqqi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2auvadwnl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2yfahfboo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hufazdcd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2borvrqhg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2kqhbvxdc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2dzjgmkmd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2muhznyxa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cxjvudaq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vgzvpmaf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kvbjysvz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2exxkiqxs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xbarjbky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvjtcodd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2tjfyvdxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbanynkf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2teuwxhzt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tppfhipu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2pbhwbgeh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jiwkzkaw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hegkseyf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hxyfavin.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2wcohmjbw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2osgwfjcl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2lbfpbqmr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2lyriacks.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fktuidfy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2khpmzmnk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2imzibwdb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pnzogbwt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2adudfnua.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ilolmapc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xzcwthkj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rqnsugeg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hmqtsayq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cybwsuut.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2yvpfpiov.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2hqjpbkpv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2znuhzaby.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqfcmqjy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2egrjrdqp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2zmzaxdff.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajubwpge.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2woqqrkhp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kvorlyhl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2gpzgfpwu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqskffse.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2txgntbmi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2stcspfej.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jsxcefqg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2wpoxcwyw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2woleqdsa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2aedpiyyc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mkmpwgip.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jwyibnbp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pfjqmxzz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fivjaqjh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mgsuivbe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nlinojnc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2skmkwvax.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqpmcvka.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dzqlatuh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vfziiuyb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2zivjwgdm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2agkiesyb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nnbfgeud.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zpvnsyoh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bmdqvgxj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jujuptjt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2easzwdza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgfbrqtv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jvxmqpvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdunzspi.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gyfjwlih.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2byqzovqd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2cljzhhjk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hsdyhqrh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qrxlqlkb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2bthpiweh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2dgnxoibl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mydqvdyl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mtnyiypj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2lwypkjaj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2sfxcipit.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iknddfqd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sfxncoxu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ghxdwgmu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pambghbl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ftqotdka.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2qvoxotdw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2lgddymar.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ssqjzkeh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rsmwobtk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2metqxwvf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uwkazmfe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ewihwmuz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2yirlaphr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mxxeobzm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yldlfsix.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2nlhwnnoi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qbqzeyuc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2irffgtmh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mgsmahmt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zoxptvkk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2goazisap.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cjnpdcvl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2byuontsi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2rcnximcw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vekbgtds.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2fwnkdplx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2mkjnqqrs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qcrbcfnm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xqbekcss.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wdfqtjpm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2vwkeatqu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gnenslmp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2wriqmxyb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2etwmkcpv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rcyklqwi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2nhxjvuka.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2metmolrr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vejnxmjx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtoiomjl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2frljlzzt.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zvtrljjk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cjxdkcna.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2baeyntvb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2jpbntlnn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2lwitmitl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jwvvuvnb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2izxqgttl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zulhuuhb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2buttyjxk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2fdwvowlk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vabcoren.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jtojwpxh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2dtfwwjur.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2foleqwwm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dytotnpv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zcmrgrhh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fplidefq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2tphxcwhx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2dpfwoehi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jbblfrhg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2hwtoazcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpaecwba.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zwswltad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bammkjml.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2uzhblveg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2huvepckh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2goldujri.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ukzmmoge.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ivvdxtbz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2hgliteqf.html

);
来源：http://www.52xcode.cn/Article/details/gt2uiitbmou.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2zltfirah.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2iynzuwvx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mqytpywf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zczmgxhr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2bcjjtjqh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2eswszokx.html

);
来源：http://www.52xcode.cn/Article/details/gt2drbpdxjz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2uyayktsp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zybmzydk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2zeqkvewj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ejtiahlh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vymwamnc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dvthives.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2xfqzydrj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2tsyspsms.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2izflrnxw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ptdlbjrc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2asmvftpe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wigqwmbe.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2efezgoic.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xhzmivyk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2iqqzzepw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fuuvxdqm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2pnyigcyo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wkehtucr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jsyogjln.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2gljtcctt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2afzrbcdp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ccceconn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zjnjzafr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ekkpxdow.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2txzfalat.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ulfmvrfi.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2tzjqjcoc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hxshgxdp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lplvzony.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ptmaoejy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2iwbuhukc.html


<!-- 参考信息 -->