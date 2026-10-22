代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zivcjlxt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2imcqqaqt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gkptymko.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tsobsebr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ternpxoo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ugzoaadk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bamebapb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2iikpbevq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2omspggli.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2sxqotqxr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pbfjwpoq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xunxljfa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mpupknef.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vmvjtank.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hksdccwt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbtbffmx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pdynzoqs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2luwyrjpi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kzwyvgum.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pjszjgjf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2zzogbvmv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xiuoqbzl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sqykcmke.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ctowrovn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dyopydyz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2fljlbnni.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2pkefxdqd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2sznxentf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2adlnqqce.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ebaksmgv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gxyjvyiw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2eprqpysm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrtypovj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ivlocljb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2owljbvex.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fhshgtkt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2fkxtaunn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yhytxcni.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnpmsnrs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ythnanmf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhxwavqg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bhkgyvyn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2eifktwan.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yjblljyu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofxnrqlb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tiyhfems.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2izaprkyp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2sfmbphck.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2okpqgeri.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jszaagcn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rwshbabw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2mnfvdphl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gzxacjik.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rtpwhkvl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2axgstyib.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dzwsrenl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jstljexm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2pzcqptes.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2gahxmbcu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2esqyszdo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2otmnofpy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hyubzpuw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2iydtjclq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2mjzxqjff.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hnevdgfk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vjfzjyut.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tmqfvdir.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2svfcjwas.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xuyxlrnp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2azqvsojl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2blctwais.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bcwwrazl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bxwzxkdl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zcedtjfg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uoigyjqc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pploftjo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ymzbsvzp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xiddswnv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2uzptapwd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yxlqwlej.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rbrhuoox.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2cbchxzfb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2sfijoteo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhdzihih.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hpuqpjze.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2slnyjrgk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeqrgxhz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bbweeyyx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ofxeupqq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2eayruoow.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2weukyznf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2tvvjouok.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zlexxdes.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ltmumxqu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2whxeigwn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rvhyjhmi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ocspkawi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vjkbgemh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2asbxnlaj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ycjjtjvh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2qqxxvmfj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2nxlvtelx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bxjuxjtc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zbvaviik.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jvswezqf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2umqtzwqw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ypdbvnem.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ykqobdbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fplaaulq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2stpxrfac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivpgxgjv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gaagssal.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2eferfkvx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2nmigrtxy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nkzscvww.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cejcypch.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2glfnaxuy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2plsuyier.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vnmdloaw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kkuegcye.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tswwqjqk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dceuksxo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2daxlxdko.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hxeaeqiz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vsaoeoqu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2erkhozzl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pijqfxtw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2uisppvkl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hlfpwhie.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2tetjoafb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kebiqddf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2jkgpteri.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2pgotrtyu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xxyelzfw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnxgblcf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wprfftae.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vyqnzjlq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjutyotb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dcvjeiez.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qziojpaf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2nvfxtwtb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wwoxkpzb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgaikqfq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tpbyhkde.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2hsjqfqxe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ccwgttub.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2fcpatuxy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2zshffkab.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ymdkjidt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2pqdaqxtx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yownoewz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2binnlkbh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2buowqoil.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2fawsronk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rmcpvfci.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbmcbick.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hfklmdga.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2brlnboty.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zefdjwwl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2utfmmtgj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cxpjewcg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2swcxkvhm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2amyatxgk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2inpheiaq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xdalxwao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ruvxnolb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bjtinkox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2loidbfmp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zdnyeews.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2fjzurhyz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gxuejnwg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yhelxzaa.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2iwyfjgxp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ymiedmac.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nssitdly.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hwtirrpg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ifdbhnwb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2atzkehva.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mtihttqj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jaicegff.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vgpvsfny.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xiveusxm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pdliuxay.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2suwjbeqj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mfikpbie.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mkmgjgrm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2khrkimii.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hqhbevrp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2qdifvwzj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hqohvzxc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pkmpdemv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mfgjlikr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2udodpslm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pvmchvav.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fwzmteat.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2iipssqyy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2pcgyizsq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ktaalbwu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vpuokitd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uuurujog.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2edsrkmqq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2megwkxgs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2tfdgadre.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zbtmhzhn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2cwhizbbm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2bsdzzkwf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xxkmhwmh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2mxbjjbru.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2iyrbkfjq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bzgmxtuz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jcuszzvz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2nmvjzsiv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ezqynosv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2xxzgwezz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ovikfsja.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sbuuplpv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2spfwqmnd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxdwwzrl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsaxkbsw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2nsmdqked.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pyonnnxx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jftwqygm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rwvzykqe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mmrkjfkc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2rjucwkyh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ztfgsqgx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zkmsbufn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iduhhgpm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2voqioltv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2uygzpffq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2owlrvxbq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ikuziltr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2mrxuoexx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qnwpkdcc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2bpkivptk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2byjnffwu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2gjdpidht.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2nqxgtggb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2bagqurjp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2fnbkvvwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onjgyoar.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2euaokafx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrntpgxy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nflxodgw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2cjdmytxe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xrwhyxcx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zuqnnpoi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mbzrsybw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2liwhsawg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tsznugns.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ffyakaoo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2cjhgoqxq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mjtsdvdy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2izuotaai.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2saxsqthk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ivjkdeuy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2crhdpilc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2nvpygaoe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2qtwphtjy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ljbgccaj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yrvlitoi.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2lmkndjpa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2zxkujxmd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mdrkzglz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kvhbdunt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2qttsorpy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2zwduxtto.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ceynugua.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vmsihpzz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uyaakkmp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rzmipnvl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zzwipfkv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2avaknleq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bckwgyhj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2plrtjyfx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2sfgltjtm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2urycofgo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2nybzsfsb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qfkojyal.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xiotouik.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2woqabjsa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2edfcdozh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2xoweemwq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lganqyqk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lbgcwlus.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2flftpomp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fmtllags.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wjlkkgsa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2donlegny.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tqxamwwt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bwlelqqe.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rbbgbxbs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2oeogsfxc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yiajoiyj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2lwyoxyfz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qixvhmnj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wercltwc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wntfzjjr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ubnnavnw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2wummdllg.html


<!-- 参考信息 -->