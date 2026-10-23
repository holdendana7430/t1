代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3kypvjola.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3srfddcyo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3klnqqkqy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zcwifclv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eddnrwcc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wixikevj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3utxudcor.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xbqdvyvs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jseokeau.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3bdygnuzw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nbimhwsp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3soqkhcfl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wlacgzum.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ljxmbwnf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mjmbsoaw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sdgldyff.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3chtjktqq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3peysiceu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3issxfbvt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3hdglbaup.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3oqdhklxv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qpnmpwob.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yphrbucw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bsrojqwr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3acwqfhde.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bebgumbz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3untjfxxt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3hkapfyhc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qsokrxkz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3snzycwad.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bqdzzifd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dxahubgq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cosrqgzu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3amtrmmbp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrgvhxta.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3icwbptyw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ixftyygs.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qxtqccru.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3dyhgttzy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gdrtiiom.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gatpympf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mothvapk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ajgsncrc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ptmgevct.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttevjzrk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3npmcbhmq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hgelblek.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fgqocjeu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gzsmlwpg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pzvhnvyt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xucnsdjg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3enlutfmq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3iugyiyol.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cmrhkiqq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3fdgqncpr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3umjxruhu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pujwjnaj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3eysqhwdw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3idabaadc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3acnhlpps.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vttywdot.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vvjekolg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3tiwjqomb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3vzhahbym.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3aibdspoy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jwnupzvx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3omtjedal.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uxzafuro.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wrdxamku.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iomkuufh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3bijmtoqv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fongtdsq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qnijpaky.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3zczdluma.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uqljdigi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3moxnjngg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3scrkmugi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3moqildpu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kcsolixp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3syarbsfd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zfvoqcpv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rymkgquo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hpnlwepd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3szrbglfq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jnjtbkum.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xfnmrgug.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3onpopdgt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3vmdqovwj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ewohwvol.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejlfznqq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3opwgtcev.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hrytqapz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmwgbjhk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zihhuuhq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xjifjvxo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wpnjywem.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3scoctzdr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3zgvxlbef.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hpopyffq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kcdzzsul.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bjwgcllo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3zdtlvily.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nkbjgljf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lzfetctg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ekslipny.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qcukaaqi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3hegantak.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vbgbfmux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uawpjyxk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bnrwrneb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swfaeail.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3trklxdzs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qvtalefg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mkkbjwmr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wfixppch.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xxbusbmo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3palstcah.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mbfrnwqk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3pgtjnkok.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rpzihkny.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ngfcnzgm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3krfpmliu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3nffoxzdw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pwgiwocm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mfwzjtps.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hlrnartj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rvnmubcj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3feywcmwl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3maijqsop.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jlysamye.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zosqyiln.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3skkfupcs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ilgymkto.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vyfaxotj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmfivfll.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3vzrtehmt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hmhhhxho.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtjhrzif.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gdntltdw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ganxihce.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3kzgontdk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3meocpnaw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ieuktccc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3tszpxjhr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3znohalaq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3oalpvffu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3crryxxsw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3clwasrrm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jbtcpoqv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3amljowdt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mzpcfixl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3omepuaow.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3qvlnjykn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3nvlawwef.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3novrjdcj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3lknkurfk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ydnrwerl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fvidfllk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3qcyygngg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3btpowlgd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3immzikww.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rfvwdvqp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3niyglmye.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vsswyszy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3rnhelsjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhlororh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3pyejljdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbrqspwt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xdmawigw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ujiizhpx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ufuuqvxa.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cfccvocf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3meefxrqg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3pqfyxqle.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qhqruysh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3qfdstfne.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rqvkdkyh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zyfopkco.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3udfhqeyr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lhquurpf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qilqdfra.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tmhkzfrz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zbxjyvhc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3bdodwans.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3cpumoyzg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3tidtfddq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rgcazskj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qsyeflgi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ossmlpfu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3twprmvkg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ospecttw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3dffrfmak.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3irsaytdk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rixmfivq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vrapsqxv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yrbgtxfm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rspowzap.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3logoqtwb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ufhiyryh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3udmrpbpe.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bxcshlsb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3sllhjfbi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ysxtolpu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rexuutfh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3rygbytsg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ogcxuhfw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3jjlvxcxa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rtvdztra.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wrunpgxm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3zhkfgsoq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ohliqjeu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3zkmomnuj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qspmfasc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rtfcfzsq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3bkqacpgl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmuzbzxn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3psfkztyj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apmejhiy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxfmfpdb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhxjhfrk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zmkaznbx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmmvrzbj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tdygcxqw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ascfxhvb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ahmthghg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ztdmdnap.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pudepzbs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ilmpjqwx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xfnibiyy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3xrenbypg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3xydjgoqn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3kahlumlx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3rhdbeers.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3xhdlqoon.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ufiohhli.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3epscqhpm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3empskmrz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3tllchqzo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3xbfdutgy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3wnpcxycx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhawybum.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3abhtaxxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iieskwxy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3fjqisltm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ztdsiqva.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mmvgatbj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rnymruuj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3zhtaakke.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3zvbkupsv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3aetxgzkr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3skxnjslm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3lhyhoajt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qluuysbk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zpvgulbv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hddhqxrc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lazoicfu.html

);
来源：http://www.52xcode.cn/Article/details/gt3buqtgblr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3stlxslvq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xedoaxft.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bvscyphv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vpnqebtq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3mxmiizqm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3alkatczj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3fnrcafca.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ltloqvrm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3gnqywaer.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3awckakkg.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3lmhzvyez.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3siyqtfpk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3avylrdsu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3heemupfo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lgexltba.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lvaurzmj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3niruwvzh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hrtnetlk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3fyayudxt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rlvtpiay.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vwlgmwpy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ujqomvgl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fgcmwmzg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ftmaeybh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3zrbeccme.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3pvjcxusu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3tmagzzyx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3khurxsjq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tqldpheb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uujsdqwn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3btmhvofy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dqreoaul.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3snrbmjxq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3pfodsnby.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3fmgwcnqs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3sbbyuhym.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3krietjvu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sjtbuyns.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3vbljecoz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ofuqiwbk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3pguptaay.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3smsjsyjy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qcvjjswz.html


<!-- 参考信息 -->