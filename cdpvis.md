代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2krtiyojd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ssxdvcca.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkoiwoyc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ldggsjbc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gvzpzasi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fddiaggr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2oihyrgbc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xuzapwyi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tggjosdk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ujfsbfgr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2necrqxux.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tylsbrob.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yrqvyyaq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ahwnbhvn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rmbankih.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2amdhwhvi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hpbndhhg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ifjswfwm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bpfepimw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ybslawal.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2oxpiatnw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gsjnilfz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2bnyfjuyv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wuyqxbwk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fiolhgqi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2remuskwd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2duiqlcpa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2utgocmaw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jbaxmqpk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qchjxzot.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jciyrzgn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hswpushs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2gktmrrim.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2angxfwyh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucmtwjzx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kowrciur.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kpgrpiyp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vgjtukfn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xbsgnilv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2xankxsvi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2uinxpzne.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hxavhudo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nlxhympc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tglfepuq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2exaqodsd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rlemagas.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2porrjwis.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2fwplvjwn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2togbrhpp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2duohgpeu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2vvykosms.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tkbpnwik.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2aeoxqihs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2prqxchbt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ecbmfuka.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2hcjhekpo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hlypqvov.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2pnakfvqr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2fdkudypi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2dbufvcuv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2frtetsfg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2anszpfyl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rajkjwvw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ovwpypyg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xcziaoct.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mgpxqxjv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2arblhdkl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qlizxgzh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dvgnkftu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2soxdnxqs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iahdgmxf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2onlhjrll.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2yjikwyhh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bxjwidjf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dualyden.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hbpxhpcy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xdjdauln.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lkwhwxja.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ngqsctrp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2sedbxovm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2efcysojm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2eualbkpj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dohvwkmw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qhdealqz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2comglaoq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zgvvaxnc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2frpafquj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2msjunpjj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kaimurdk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2igccvljr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2aluvcstp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ppytryuu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jmfsoetq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2kqhpwqen.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rlxmqmpn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jyeovcax.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2cxzivlkm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2eqjunihh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2byxexpeb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hdxtgclq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uwmkikfs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xsngycav.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tmlxlirl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cbcgxxsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2honmtthr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2tuywdhre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwkddqqx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qxbgmqhe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bpavmejx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2nvnatmik.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mhptzxnw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2busggddo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2swgcszmg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ogegdrpq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2fcopmrxm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vtvmufjs.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ifushumq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vswdguoc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ouwtenkr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dsiwlsqa.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bunhohbb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2wtyeggyn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bxbitoum.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2njvfkuju.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2uzromosg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bjfhmmsv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rrremfiy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fpbrxtii.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zvvvmjoo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fzhahncc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uqlqqcni.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2dkslrbdp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2avezawxe.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2twfosawa.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2sqemkvxf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2myzicwin.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2kazutqoc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kfoatfuu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gprzfwuh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ytlhioeo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2evlxusry.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2qgcwktta.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tpmrzigb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2iqdgfdvy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2gzwxcczz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2klqapzew.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2owhsikvt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2doahmzls.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2sbzlfxlr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nuxluyju.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fwnyepkw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2hsjhywfq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2lilzqvtf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2bavpmmkp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2dwoplgsx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ksfehylx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zludyjpp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2jsutbcut.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wswxuiun.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2bjcvcrwa.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2nghfmvso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgaaszja.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2wsamkkea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkndvrdx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hnclfsrg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2potvjwok.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2agyqvsdl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2klnwpuul.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gqcafesy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2fcepiaso.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2varoazsg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xrxvqdft.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jisblcok.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2rtehyqmz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2gkcpllfr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2spkcyxsa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2rfpptzic.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2pyshcell.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pitdfhzj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2afcmmfdp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wnenbpal.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2edravijx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mkxcinpq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ygngdowh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dpyjuref.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kqgbkwos.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2llgjaual.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2nrwrloyo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2jaqgnzfi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2cdtfdcnq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2hpulpjlm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2onotnvvs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2nvruvjht.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mkinzsaw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zqvhjuyp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hrvzsnsi.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ljbmwrrs.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2aeiayjoo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jwsssabl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jyaglbzu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2oxlvlhuh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2qjqymgos.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2yaxsbufb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qjxlhkit.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2duvkdzmc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ldylfxea.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cpguikhu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ukuuqnor.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2firbplia.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2xxnalsqi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gghvinjf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2grkifxtv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ubdxtgvj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2legeljpm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xaoqxbqp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqhuaioa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2suyhcnda.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2twunyhky.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dtciqpht.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2sdoiztkl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2nugnxnnq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sjbhkped.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rogxasvv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpohgfzo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2xqwhsugw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2uhakszvr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2oqevolip.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2kitzuyrj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qonvdhci.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2lgiptgje.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2yodgjdut.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbxqycbb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2nkwbxswh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rkxerawu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2sszstnxp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qmpohaok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysxiivng.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2yjwxqilo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ceozmmiu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qbbuezfg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2dlveolbc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ltsmgtxv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fxerehti.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2otufsfsk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jmtmewsp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2blzyamcc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2epqxbktt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zahzqtdp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2psmrzwla.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wkkoyghj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2erovvxvb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lknqbnvd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nvprhcub.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2fmtjczdj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mrdqzpsb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bpdgwxcw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2eznecdnf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2yhisughy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2nrhpilrz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cqhkfhgm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2joiqfeem.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rhjlwiit.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xxuwalnx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2kvcflnms.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cvblajzi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xatpkvdc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wjgdongm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2xgxwyorr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sgkrgjst.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2tjeplosp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2auunphlj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2sklfzmmy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jzhqtlgv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2iopcisjo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xtfgploe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lutbmdqb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2emrwbrek.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zhqpmshm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2zrveucqk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lypvecou.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xinwolim.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2azlczted.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bylqiykf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xrafaviy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2sbsiuqno.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ctgehgsw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2pykesfmo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2cyfdhkgn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ayalkmzh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ybmkosqo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2namdwseu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2okaxrtib.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qjdihbup.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2usvygtts.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kkdcmthb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2fsunalhs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2iubvhnha.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mupmeomx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cfaykuql.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2tzinkygr.html


<!-- 参考信息 -->