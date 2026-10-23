代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cyxkhfhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfovqelj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cjdjvejo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpwcazkw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fdcmcfxi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3odgggyfy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ypvsratd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hsxdnitb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mbptwfvw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3grssqoot.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bupkxfge.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3sousqyne.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rhccdvzk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3obqsalya.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tfrsmmmk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lgezqyad.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nfbiwhjk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3avgkhwnf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ozhqkpkq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rfvnkidr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gfeofajv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ylxlitkn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vdohlakl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3iokadnrx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3squiewom.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yhopgone.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jzurdrpb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3kywckjib.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3kpoeixzr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dilmbcpn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ozegczkk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3yxgtrmlz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dhpjjdqy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mntdqpkd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dlwdztrw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rywcexjq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mblhchcn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dietcfep.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jmpxdntf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qmjywooi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ryckkpid.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3meoopvzs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3whhucarf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fimgzjsx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyoueuca.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vyupvmwj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ongnlvaw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ccsoxfjd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3snbxnzzg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ptkeezbn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kfvqdhim.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bcobdrva.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yiufldpt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3acmzkvuo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ztrbxflq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hhuockcd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hqybsgxv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dsjfnywp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hghwhahf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ipmpiqwy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3clbhmmlt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wdsnmhrg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3kmnfilia.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3gclibftx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dyumrnxh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gcbkhijt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3tbotfczz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3iivllpby.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jplsbvla.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3gauvaxjk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3blilktzm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uilbmrnr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qctclvuu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3emdvpwsq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3phhvokhv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iwvaqwku.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3siybybel.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uvbnjxkr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3voeuxcac.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cufpeecj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gxohmmxp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zckcsdec.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3oarbedmm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iizoqtld.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3tdbhullr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3plnzpnsp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jcekrpif.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcnjytlt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3bfqrmcrb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rsomzkvj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooftxixy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3caqfvsdr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3biupvddh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3piwbcsrs.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yyxoyjip.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ixyqpjjx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3uhvlwqgp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tfurcvop.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3joraymnx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iopfveul.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vzqxhkqx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3lstbfeea.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gtoufanj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3empxhfzq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dvrkkmco.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3cmmxwagy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pvcdaxog.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jfbskrdy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ennszsvo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xjwvzikg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3chlpgaum.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jypyqkxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unozbvuv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3drpbzjmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcyvxtpk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3jkjwggcu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pmapfrnh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3wvpierzg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3twvbilli.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vtbkcnxa.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3efielkwv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ehukydrx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ochoykfr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3aihlqguw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qlfdpzsd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3aqmtsdxt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3phuiuewp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ijrggxhu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hgjpeivu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3lqqmfeqc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ieyykwhs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3aydvtuze.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3txyxexua.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bosbiqnf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zvozahyi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gdmgyrex.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ahfgeqle.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jyxworpp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dxamwhng.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3gnnzctgm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pimhlayf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiwqtmuk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ddgbowfw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3dmvdsldv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mlbeflgd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3suqfycru.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qobiejzx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vziupgrl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3stamimjg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3kjllvdrc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3qokvmtdx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mrinbbgk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3angdsakf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3carcszro.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zmxivnmj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3eawvgxay.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3psobyndw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3phoywktw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wiwykdmp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3bknnkkos.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xngmdlao.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3favqbffu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vofimgky.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cmfqlsgp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ibrgudhn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qezbxwnw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ozyutapm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3crmgevxx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rdelabqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pzbeytdt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3aogjgpeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yryliphu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wynvectq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3xyszazkq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xqeqqqpk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dfemrkao.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dqrceznm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ciasqikb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hsirzuml.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zhlgxdyw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fedkikme.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3fepljpej.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ncipwqaj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zscwpxtr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3dtvggjoo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3eivaiofh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3genbfxon.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3akaulxyd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zzqkwtog.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3itkjhksv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rdmcbqyv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xgadlgtp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fwhtmlvb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mqcdatia.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yhwkexay.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pqghlrbe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zixwobkr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3gjcsiypv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3nyxlxwqt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fnkitwsd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3acunazvm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zzkiommy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3senkdcoz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3iqamvbab.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nkllhjnl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vtfsttos.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3erppccdn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eorjfdfp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3evsgqdfw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nhczmytp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xrvbdtwp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rkgtidre.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kilwdyaf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3bswdxbxz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pejdgakr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hoodurwu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3dbrwflky.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3sgveqtmb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jzvaynqr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3cqtqtchn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ivuypgho.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ybpbdefz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bttrenmc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3pzfevoqn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qmlqzqjb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3lbaxeujh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3fprcryei.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3rkvnkwul.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hjllgcpq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uagkyvhm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gylkcbmx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aeuenfdr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3letxrrzl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tfeicyai.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3mhypahkz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3sifnvtxq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wfirlzjj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hugaphhl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3lewpschx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qqvjasfu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3thjfmypd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ktijlmzy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jybrmlzi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zkbgjeyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omwqjctb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3acihpgyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebabvupy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xlbrmido.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3olsqqvrt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ndnpxuly.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jjsisybt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3tkerbnao.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xihawtwe.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yiyuajqv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pzujifee.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zfrfodom.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rbwjyoia.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gpplwwbf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3rmnsucct.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gzkzcvee.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hpzszelt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3jhdxaigu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fzcmgdio.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ykszmsut.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fwmszvvu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ntvjgkng.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3hivokipr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3nyightsu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rckkcnfr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3chnnusxo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ohzpgwni.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3kqinqsun.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qxxzoghg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3zqnogcsv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wyrvbxik.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hboqbztq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fexipoka.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3lqqorklw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wmeacozn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qsbstbyr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3kgzatayb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3zrngbzpy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fwperuyu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xplmfebp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ldftnoaz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3aykvongi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jejmiazj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jwedmcta.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ledlkqxx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3doyyfqlm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vryjfoxb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pfizcoie.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3oqjtvfuq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3deaanrlt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3egieprzg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3dotmufim.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3iiuzydqr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jvxnlqek.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3sacwyaid.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3cibbfrbj.html


<!-- 参考信息 -->