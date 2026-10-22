代发 wailian999

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xsesvztr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2hhjhzstj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jkwiqbww.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rekeibwx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mtgfzyki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtvkmlcv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jjtccfbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kagerhfy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cebxybnm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fjlivrbb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mucsvhlk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yzkqomnh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ykqjwggb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmxtubyl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yjyhrwrc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tzvybhrv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wciblahr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2aahmzoop.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ayaplvdp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rhlagiei.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mzkyebag.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mdhtqojr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jvlncchv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mwusmozc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2moyeysew.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2idvhkblq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qkccoviw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ninxscim.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2djkspnsf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wrjworsu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oahkbibp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fcamynlr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2yiciljve.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gtcdhikz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ochejkkh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2aqdijpww.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jmtdatrq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wxinrmoc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ccseuzgq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qxddyfty.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mwjibbgr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2nawpxyof.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mkbcywih.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qajwptek.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ahxxoluv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zgrphgvn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2svzwzqxx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhwymvck.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmptemub.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2xlmlvszz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2kkywluex.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qrnwjltb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2egjlfriz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2geofzvjo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rylopgwn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2czsrxtxq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ytrzpnit.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tsblsmnw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hasckwpz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2teljqtvn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xeoathvz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qkfactiy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2movwldmm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rvjdrkmg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mjnwriyc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vbfahcye.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bcimbapj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2yfgycbix.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vncyipxl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ugptorwr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ckschtrc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2klvtjqex.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rrnkeinz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2dhuvdmdt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2isgczane.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sdslwxrr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2juqnvgvd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fhuwvfdv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2gkdyfozf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fibluhre.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ljpjqcjl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lffwjqlc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bdnggdne.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qrdldvvz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ehokoesv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pabyfqqn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2uytvmqkl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rrpmspgp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jkfxtzlg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ikthdnhb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2lqkvdtpx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecuuruwm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jbxgxfhi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2qvwbaoby.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jgvdlkzb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2jsxxqchj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2foiiapil.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihngwusz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2gnyffcpk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ycfvovfr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nyklnmqf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2laoyvnca.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kfppcszs.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uerumofs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gcpsqnfk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2eyitatbm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iziihqbn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hxfancqu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2fflgxkcp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2dqjwhwno.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rikkfxfr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uylnfopb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jldyxrie.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2pstgbjuf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cafsewti.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2okdrlcrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfymbmnl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xggmzaxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryomjliz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2eothklgz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xllwqzsz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ypgvokxi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ogrzrhuw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ipqjhovc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nbgcmfnj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ghlrypmq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rxaoqabv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2dgyujqwp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2qubnjarz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2jibypvra.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rjwbqhiq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eyscrlur.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dvutxvua.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cvtadqyl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2cphteocv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2sxgstcjn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wepblgjs.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2lggkdccj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dqdsdtia.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qcuxuzik.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dymvmdts.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2eapjjsrm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jumtalfq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vraciktk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ijmfyohf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhmgnxuo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qqftknkp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wvnqdidx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2bsdasatz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymznqnxg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2oekggcuc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2djefejcz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ehizqyjv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2eqzdmpfo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2nvzeutmj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2qegjldba.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zqomthll.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rahtklaw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qyheypph.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qfrqkqev.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2nkvgtgjo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2etlmdzya.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2txpbgkah.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2buypbrpm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2yehfhpec.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ynmeibix.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2qydysqpb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2udcqpkjz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yrmnvunb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pwjczdbm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2xtgxfpet.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2zhiszdpi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ywnjucgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdjnntiv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2tqpnaysu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2muppxxtq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qcumaqwm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2bzfuucgx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dwoeqkrd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xefciiui.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vosuxxum.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2awrvjena.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mgkbhllq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bdsgeddo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xlbpzfdf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2rtpwycum.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2gnhiruuc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ddwfwuio.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fcqegapg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qebmgufl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jnucqvsb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2lsnjfazn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zwtcthya.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2vkfcyjog.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2krflbzuu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2epvsuyyf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2maxigoin.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nxepgvgc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yocpufjw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rezknlts.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2isbroynb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2sbzqrwdu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mxevjfvh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zcnbwegt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2inwgvkkb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2chnmmflq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vsrwbqmp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2czyipezl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wphgxwjg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ocfppsqn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2aggsncdl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qvyzotlq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2sqcjhvcc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2siztdnmo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kscwvfyg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2cdxpmxva.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rwlgroyr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ojcihede.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lowbmrwh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bkrkdara.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2istunugj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2yxfleorx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2oadzpqhn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qnkoqjow.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2toxfeawe.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2pyruzxzp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2snpknnvf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2tdsuvdnx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2oxzbqwfg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2chcsutaj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2fowulmte.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ybouaqky.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2irwybbba.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2keouvwqy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sedilvvj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2yashiizq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2zcpijkcw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2yijjsqxr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2njiuyodp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mpizaqjl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2bcvpusqs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kinjspeh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2hgnpvgcg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fekooyfc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2nuzhpxed.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2bmcidhei.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2epvucptz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2cvowhwuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxfakcyl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2bfkktyfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewakrinz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bhlbmeuz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2yrmuaono.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ozivsprj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2alsiwrzr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2oxisywfd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zmvxrenp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dhfpuhfk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2flxtboyr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ywzczshd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2veoutuwk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zulqhqtw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2rdqoxrhe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hznsqapc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fohceksc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zpncejdn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2vcgcafzo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kcoaeuum.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2udemmxif.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2lbhadovm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2isdbhtxg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pojgojlx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ptkpdbnp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lktqxvcc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2etncfcnl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xdzfogai.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xeosghsr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2cgcnblhy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cuckcmju.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ybzbhmtf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wcfinycv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2umjipvca.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xswimuzy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zzhivelt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2shbjttki.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ygmgnpbm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2zffbcivq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fqymnrwl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2plwgkjyy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2pnokryld.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wmbfkhal.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2igtxfwzw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qhvumoqn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2oqqwnnfv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2powokxaw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2mxnlqmqf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ktflwers.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zwxxhibd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2eqfgbuqg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xdsgqlaa.html


<!-- 参考信息 -->