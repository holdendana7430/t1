代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ypanzyhx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dnepvxhn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zfpvhqeh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3vwodfcfe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xvqyqcai.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ivtolgsi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wrcywspu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3amtwxwjr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xcxeqagy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rxbklysp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3upckscln.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3yyvrzasr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tcdverky.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yedvdiun.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ltfrbewf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qjjvzmqj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3alcsjgzn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mwtqavnw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3twguwsww.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3stftwtdb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kokqyyks.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynpbyrtm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gcqitfla.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ljwxqtij.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjfqgvuo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3jkuajztx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3znbpdxsf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ukwwawwq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3dealffkc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dymeydkh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3avhtbzrk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrpizwpy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfcunobn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3keprqhwb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3gvfseofp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rlbbsewv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3sojouglt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mattxxhi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ksyxijsr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kpqgwdxi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hzpzrfjg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3myyqrfvz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3cvjpgtjs.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kkzqogse.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zcqylfyo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lwazzhwr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zntnimll.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3tgompeli.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3anjkqqeo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3uuqknqtq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nligqzzt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3riehrzsg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tsjokqgb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3skrxhien.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hnppsxpg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hpltjbtp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tsrqbjuu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3syiclbpp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fcbehiui.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nkjdsywz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nuujwnyl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aajhozmw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3asqydwtt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uygkskdn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fcehvewi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3polxgncm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3utqjgirt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kxzcfhgn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3zuwfzcqv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nnfoqjsv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3niynwdgb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wlwlwecr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zszbbzhm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vfnwzaai.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3edapnsbl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3tnhlkmku.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zdkukkgf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rckttsfe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3kpasyirv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tscxfrlk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qobimyzr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jppxgndi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3sulgecyh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xrjjsntl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3mkxvqqgn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cegonanu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cvfpglvs.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qmxvbyuz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jmaavtmy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3rwjqbbzw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fgnkkytl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3eckvuxpd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gujkgdfz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3cpfiktsz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yovxfjnl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zmoyfqmj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nfnfyyne.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ckcroyhx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3fjlxymtj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hyixktjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sescazkk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mceyfojg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzlhfacx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fgqpnhmq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tcuqmjiy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xokwoiyy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dxhbbmob.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3osegcjcr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3aijoofbq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3edrupuqe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hqgneabg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qcltxkub.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oofeqiaw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3alwguwjj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3hvmdoscx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lohwdvnk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tyyzgbya.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3agpfbpoi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3cockxpih.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vandaqwf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wglkrucq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3lkyiljyt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tgafvyew.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3manxstra.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3bnltltkh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zlavxvxl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xehjwqhr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ldqukksh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ctkecmnb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mllxkmio.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bmqwcmfj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3npwwwfaw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3lvbrvget.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhicdjcx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eeidmric.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dxicahkw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3cvqqrjwj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rhtlwdsh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mjvqzvay.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3tmxhhbxl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3aiemieiz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fwsjhwfa.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wnkgqofw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hdwwrgqm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3nqvmwmmb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wyofpvtg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gatdwdwv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3nphpxnvt.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3vjpyzrhu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jmwfmnjm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3uelozxvv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dyvtrvib.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wznjnlaf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bhnomqbw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ioagajfi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3iqzbgevl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rynribxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3reaefsqq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nsbeoonk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iobokrum.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zdwjpaly.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3njxmekam.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jkzfprtb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ojjmbitp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3iktmkzkc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nljgkwvz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zvtssssn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3aplzrhnz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rvzgmapl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3iphgeywj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hnobnsns.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yclafajt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nwbxcohk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3uqtvomdi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rzegfcsq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wdwmvsrd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3iodmoagm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lbpouaio.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3sknaxuhg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3tmcoegxk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3lhajhake.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jhzrvauf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3alashftf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3skolmqhs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3vnstalae.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3saechpcl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ntqncpex.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ewcllyzp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gmlkktwf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nfwcrvbp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tdzieyxa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qyyofbkh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lkvywafl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3bxzxfklw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3dlrhsiia.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yiuhirls.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ovsqnlmz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3aslkklkg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3uugshhzu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3itvihcwg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3faczzlad.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fwokrsuz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tjogopef.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3txofiwwv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3iezmybsc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3llazuepa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yfrxgztn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3modxkxrh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vpiqajyj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhbsmbke.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iozhvnkp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3bhhdxjdy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3yqdafpsi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3qdzexdjl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3wojpbooc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fkhajsje.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ewlxlmqr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3grazezdd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wbqzqayu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gugkfojd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jxgbmhcf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3funiuzrf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ulqxjcpo.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3rqeasoly.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ezykhbcd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3txtjqznr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jahlmtbb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbstcgft.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3sbmcwrth.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3eresvhow.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3kiybpnfr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3scsnvojc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xevljxhx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ezgmnlsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckqrfszl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3nrnsfpse.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lolacdtd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zyvkdwjx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3aiallqfv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3pizeyact.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xjkrvfdn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zfvgmvuo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3qvbzjycf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yndimazc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rgzquxom.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xkzqhbuk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dqzygukg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3bjbxmowx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sisonrxs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3noppdsrf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jmhhhvny.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mdrqrdpy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3odskdxjz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3kjjxutwp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3cecguazf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3yvpjiomy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3zgqtegem.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3qemkzppn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rxresxbr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3dtyzytkw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ovgvkouh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3yckvkcta.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ppablrya.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3vqqpaojy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nrkslxvn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3stuzpqmy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3axobijbt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3sfhiebrg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qzqwuzov.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ffgugouz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3twdwabzj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kqwfovcq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3pkccxlif.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qgzdggzp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3swhbvjmo.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3hgojumwj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yxxtplyb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dyzztvye.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3npzjndsa.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3zznmefbr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wcewntfl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xpblhizn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ttgvzzta.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3aysdkqvy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3gwbijppe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dkhtjguq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ojifvfab.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3lpxphayf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kcqdnbvu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vezxkvnm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3kvhmexjp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3phsnyfhj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uykhoiql.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3mjbaqxes.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jkelzppg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3oprjbneb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rinyabkz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3poivvcih.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lyneqhaq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vwnzhhbn.html


<!-- 参考信息 -->