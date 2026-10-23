代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ifslyyfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llpbpmqu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3goxpnlxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhrkmgid.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tgplvyzb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ysjiwamb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3aeuoajou.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tmnltmht.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qpbvngat.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bswjluox.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iioueuxv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ncsehcuy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsjyicmy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kjwodglk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rlikqbfd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zjcupzap.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ppawfgtd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mxuwcrsy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kkklosrn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ijpdjlfw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3naadevth.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fbqbrtut.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3kinprneh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3nyzokcnq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cqawngwz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cwcmjjzy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yjsiyhwv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wpzzlqsm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ndsfcvab.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3vqvjgbcd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vaqrhsqz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3tgssvtra.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nvzjlmfx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zeknagzw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kioamjoo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3simcrffs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wsnwehdv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lyvmgzko.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cbzpjvba.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rspgjphc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3swedhyyh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mvexoptm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3efwveojo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3apswzclk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hckbfono.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3okmdmdrd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qwnlmzac.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fdpllotp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kbtlvzgn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mlzenvoo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nopoqbds.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3erbuzruq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ayzjswti.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lffkbora.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3nvmuoiyc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fkhsagvn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mdhjsjct.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hebogouj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tmcawvhr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3cigxyytp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ztpgjxvs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3viqahihg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3amtwmvqb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qlrcmzfd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3lgbjgngk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3megxdvzf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3auwgrstf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gxdapwnl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gljusepi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3oyoyewmd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3evmvlsiu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ykogyjnl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3idnktsbt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wnbeqnnz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3raqpyhel.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uninsygj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uflpwlka.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3pgemfmox.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hzzxjhbw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fqvoundd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ecxjnxbn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3inscfitg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rpywwihj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rbwjdyju.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xofrajlu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3udeczfbs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zrefqprb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dipithlh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zcvbrpkd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3btnjhspk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3wwbviwnt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jujtrkwn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jrxjabyr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ebzefhet.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ykfgrofj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3gmbjdufi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3llylgsmh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hoddogwd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bhzfgyrj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lnxcxdxh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ndldczqu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ixmtuviy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xxlbhykx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vdlrsvtr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ihnevfag.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3saiomdrs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dnfqbezg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yxuknjzz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dshyclki.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3onubxzwa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mtjhkthp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3snbqqdjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olziecbu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bgxwjvuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsjhamms.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3llgpldud.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hrujmxhk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3mybegjcw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3aunlobif.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uwcogjmt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fixkbntr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3evffgrje.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3lzgomtmo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ztifbjkn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kesdtpie.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xjrexkwt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3crinserz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kfopknoj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vkhesmsn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3femcmpnf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3dhwtqccr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mhjssatb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3helpnsar.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kvbgrvjo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vjkayylk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ezbnfxec.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3gwxggken.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3afrrvmcb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceggtrmp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3jecgzygt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3cmpztnic.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tkllmgbb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3uodhlozc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3oxfmusao.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tpvptmrr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bgkskbyb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qmybpttj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3kjxzvbmw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xoxihmus.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hsyoaaqj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3oftqhxoa.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bkfeetnb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3juwzfbxa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qjodtzco.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vpmmfkon.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hvprzeie.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jiejblso.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3rncwqumx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3poolflzn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wizigdlp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3unicydob.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3daebqlcw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dyaxoltn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tmltasoe.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pnaojltn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tbfthxbt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wjagwsqh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3fhmtapkt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3mwbqwmoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxhmmxsc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3qsbaflgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpyiuaet.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ggcjrbcz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3duedzfkf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ttkynrol.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ebtprfcs.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3umjvrmbp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fwtkseao.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3uuhptuhe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3chtyshcq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mjtihbln.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qxlnjhnw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3dnkflbng.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zhrxpsen.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3xdqjloqk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3blfjpjuo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fdeiwfnk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3afpimfuz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3qgsdiqpz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yrwvvuxq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3opbouxyp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3mpzluuhq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zpmwcwmx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3frpytini.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3durnhkfu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3deadtwxl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3fvcldnzb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3fjvqnjvu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kbquaoyx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3emdoxjrb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3cpuqkazk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lwldxrpy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vjujluoh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gcosrgsv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wgiesdig.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3iwanfdyt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3dapxgool.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mcydddok.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3avpbmtdv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gtclwanc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3rxdwujoi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3etfvzbav.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jiwhmwpa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jlsphzsi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3adcqqbki.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ymrpovxi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3odpbtcmk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3depdwmis.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wtahwxdr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhfsuqit.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3saefeduv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3adogxizy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3oplhusir.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3qghlswmc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3odscbuee.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3srxmrdoa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gfimyotu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wwuvkpzx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uaieqfag.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ojoffrzl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ljcymhgh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3htynyhnz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ccdtjykg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wiydiggt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vozsyzan.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3dtpjrawg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ykopadqt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dimbfxgt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vikmqksm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ocbcnnfd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3usboetad.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jbkxwjkb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3aueaelbp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3lyhkupxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfkycpqk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wjfgcrsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpnfratp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xmsdqnfv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3flhwlrnv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vrfbzskx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rqaoinmk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lmgaoezt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3obawqdxy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3svqfjzyy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3gnfojyca.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ywydlavf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hsyhurse.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vheozbki.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ouunapju.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3gfiqdsyn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zabbdbmp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3trmldfiz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3aemygvxl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3nkhfhmip.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3frepzemu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ktvwqfbr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3mgmfjsju.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qpalsqmn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3svflvden.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3lwcfnznd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pcmlftzd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mxjlodcb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rzcfmaae.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3kuyjetsl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jxhthbww.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3kiapvztj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pyzglzrv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xqpntbqi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3seugtufm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3jozhifpe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3hoqsourf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3elsktiyt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3gjnmvzfh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3spvnwqrd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3tnidevcj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3hyigyjtl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3izprgofj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3fhtjjhuc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3msaxrtvz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3khvknudl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mkpfdpmc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ysxmicpj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kopywkwx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3mdehzhdl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3azgvqcxx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3cqyiormw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3aiklmdly.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dpliwcik.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bsboyhjr.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3hmvqipkf.html


<!-- 参考信息 -->