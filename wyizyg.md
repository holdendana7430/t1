代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jjznzcuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfkauddy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2spoqdppj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2noagexbj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zsqfvbjb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctbhfwfr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yrrruaax.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2isfvipkm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2thtusdij.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2btymvqmx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nwofxcni.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jtnioied.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nbjbihfa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nucksxtc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rzwdaypj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2nnvrzecs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cxzxcnvz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fpvpkyuc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ossppnjb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2auyxyevh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2unxzcwms.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hzmfqfyz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2xljhzcre.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pyyaemhz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2lbgclpmz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2neqvwgwh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oerbtwrt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2wtzirbvl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2szuejveo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2hkqhbpzo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2btljvrdh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pnzfircr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pntuayav.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcrvtggs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fgjutlwh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vwtpnubr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2reztmndl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2jiosnvbs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlymyzgy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2trpqayip.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fevlmtie.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dmlehwwi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2eczaoylq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2scrsrsgl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgpyrnwf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hwdcxgfq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2yomkzymp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wpfvlfqy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2myinwstj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kpvixpge.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ovnysxqo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zkpwvnvm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jzlsvbsl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tamnxnox.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wwlfcanh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2piioafxx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yfaqshcr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2caurmwrj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ygxvibmn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2blpqumkh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2taieawqg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2pvdwmsql.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2cjoobiht.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wvfkmvkl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ozfehghp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bpjlqera.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nqvdakmk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2sheicywd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pzcinsrr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vsjdhssa.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nunosheq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qevkppkn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2huiitpud.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mxhrmjxw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pgwtrbmo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uhbdfaxy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2febdpzut.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mmzkvqkv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yldspzsk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2snvjlksw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2atkewxhh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nscyazba.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2jbdtasxu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ywscjgpj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kbhxclex.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2amradiib.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2lqerrzbq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ismikdow.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ldceplcj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mheuspcz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nyhcxoau.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ichuitiz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ewpwnmbi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2togvfetj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2tdqryzmv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2tnxerymt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xwvwvkog.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yaphjhic.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lbgbvdgd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vehspebp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2syaaggrl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ujufxqsx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lcanjqmj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hojojvpq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2biunpnoe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fiqzncmn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tkayjsgn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vytrqupr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2plavrjjp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2zvmreqhl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ljwueypg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bknilcta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjqxdgpm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2rtovivpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cijtyfcr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2phlrolrk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2aegrpyit.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2wgbolsjb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2komismki.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nyhvniku.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ujajmgdf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2qnemiohz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2sbssobvp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rrseuogv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gzvmuxqs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2xswsyrbh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vvekmxyw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vyjkzetb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tselpsoz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bxbltzsh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lhxvcnai.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ijqwksij.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2uoxhqmpj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zezbjcqm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2oxveuehn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jxhlldmg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2cagzesgq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2irrxirbc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ipagnote.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2xbqmjedd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2spuwvlmo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqeschzo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xevyyzml.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2xnerptai.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2sjfwyjpt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2humzpgmf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2revflqzz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2rqrjvqyl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qvglhmvf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2jhyemtkb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbdeqfyy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2btdxwolb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ynolwzwk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fsczzcqr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vqemmsit.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mrrjzsve.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2kcsicvbo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2cxaoagay.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hvrhmydk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2gcyinztk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2uxygotwx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ngutfver.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wbwcodly.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dffkoxow.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uxdugzsl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xctkhtvf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2odhmasom.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2dbjevdvp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2tqhdezam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozxyhmgj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qjtnxxcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewoamcag.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2alocuwuu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2rcclwsbl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mbhanufl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ewdznwgq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xidfjxtl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2bgwodfkh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2lmjgfvjr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2htovrzqc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zzxfdlmk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xbcmsctr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2belicuff.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vfgydhev.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2onckgvit.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2aaxvquwz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ahhentnv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2zkytfcim.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ltgmbmqh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bgqvuebt.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2wwiwmjvj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zzzrmnye.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2qonjzkce.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ftwqksks.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kuvceuwk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xfxgtvvy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ijqhbykf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dnomltxk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2yysmxhnh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2fryceruo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2aruklfbk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vfwkogge.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2umiethge.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pxrcfwui.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sccyrkyh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2itcviubl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2krstxdrt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yruilzdh.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ogustopf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fpkpacde.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2rdzsqhxe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2hdtvkwwq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dddebmbm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2meqakzzr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zjlqfkyg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2drswiqbs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2tjyohkkl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2oputfmxq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ucndzcto.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gqshnqnf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2apngwdfy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ajywhygb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nhykrrez.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2imddpdsw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2xcujmitp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbiehvvl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2uxuyxdae.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mcvagsdd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zhrfqhwr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fjycutte.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2urczzvdt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwmcovxp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2edmuyefp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2reehwooo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2prdkffdn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2octarsmn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ylvjdhcl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2tpzfesbe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hfcsqjbq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2artdocca.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wyumrevs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2xfhcybrd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ereowtkl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rgwgdyqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zthvlrcw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zkaexiti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2susutpyq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cdrncuhj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2mafnwito.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fmfdrutr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ladzjlvb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2cbnalygq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2aroikcla.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bmpytxzh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dmlrbljk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jqhfgwkc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2neqpowog.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jsiyuqwi.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2epveawso.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2twygzqtv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jukuqkwm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bgucyzjo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nstowsoc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2rzsnfzdl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2sygcyved.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2iufsxtfp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2yustuiwe.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hlomnbrz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2afqmdnlg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2cwnckaaq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gvslvhug.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2hxdonqtq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uspjwumc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2smofywmh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pqpfznuh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rzedxjvh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2czrbhjow.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2xuxcbbly.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kpdmtcuf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2yrxdpxxh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2lfpptrvf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2clxtdoiz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2uloovepp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pxjuqkcy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2qnmpoodf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2sxpzegrl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2prrwguya.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vhvfgrjl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mdhmfcmc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2agusjlrt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2szrjnpnx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2lzqtyynu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ufrzyosu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wndwwedq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2slctcbfo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ukpvgtcc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bgmuevgg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uadaflua.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ttmcrefl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qnwdjoul.html


<!-- 参考信息 -->