代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nkkduuut.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2laeqmqws.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gzvwfrfp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tbfjmhhh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mfhqyhcb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2onszihrw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rzgrbvnl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fqcbzoql.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hjhivkpl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nsvjpczx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vjuhwrom.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2odsuelpf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gqdksjso.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qdzysuoe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fhwocicl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2sboubukh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2leaepgum.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ghqdgmaf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2psrvixqd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wqqnyfvr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojlclqdg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2anpildth.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bedfscop.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fyozhljb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgsnivwf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xgzvixfj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mccmgmaf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mywlrjha.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2sjemepku.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gycfhcww.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jollnvoh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqkgbons.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hpbjpfov.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2cdnnussk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2yjaeszvh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ignuqtlq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2suvrxtkj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ktqmgvai.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mdpvofqs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rsmdomdx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gcgeqydc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yzdluyov.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ylonyumw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2xgqgysdp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qawldfbg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gqxufvdi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2etgevkww.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ctzxcsgs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wdtbxwru.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2hgzqaaxi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ckbwkhlf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zqjlvwmn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wucwodns.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ovkawaem.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ixhbmzzd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rxydaoum.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eqjxypwg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lzpatejo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tqbyvnyl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wumxtdbm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wibxxesh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jfwtwoon.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vfzhtwxh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lllywcve.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gpmgikti.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2udxshpct.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vrgmikge.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rdnnmdpy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2sbazrbxi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wyjkwvnv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gmgzyhgj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ozqdwgic.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cycrdtao.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vlymcrwd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2sdmjlfoa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlydukyd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kkxymqeu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2cmgoteet.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2etssnnco.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2sqxzxxsi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2epxjiabx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wlnlfope.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2uzdxaqfq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gfzznblt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2dxkissrk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hxhzzkum.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2syifptne.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kulhgmtd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jngdegmb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zbkzcurk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sdzzxhyv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2qmnnnekp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2qqkzgted.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2tpcxvdur.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ubqxxslg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ksdgbwpe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ykfiovpt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wxnlferf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nwqhwssn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kkwegani.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwfrllds.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2talxqxzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdksbhij.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2icwraphi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2gwyqisge.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2yhplogiw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2haerbplj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bwpbunzy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2stmaerte.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2anpndfza.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2nloenfnt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pdjhfvrd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rgyegrvk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2vgkdhkri.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2icgblacl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bomkaopu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tgnlrjiq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vlqcianr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ffivndxf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2orkyjncu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fmbbbbgu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2djzogqgm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kugitwnr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2lktwbtlk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2waqwfktb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kocddhbu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehfsjzbp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ouhfenme.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2waxqolps.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hdmrwvok.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2acncicel.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qzadabfr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ckltkbxi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zusikdqz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ucyakdwi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2dqolztaq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2utwithjt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2kpvoieer.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2pjapjqvf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ueekjyge.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ksowlhza.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2acigfdyf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2piuimutj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qmyabmkw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2oxaodyzl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2auqkqmaz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2oqvfkxpe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2okizbirl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zkcbkmmh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2azlzrdoi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2smzxvxfp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2awtueihp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jiablpvy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tlogifcd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2exblyykh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jtpmamcq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2trmvwxlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftmtodqs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2minidmrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qteteuen.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wiljinrt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2xkihhfqr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2csrzvfkp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2iazyhqei.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tonjiqdi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2dtwnnhfa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qszfvmmq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xfxwabat.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2iqumryoe.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2trihabwr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kcxflovg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2pphycyfc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wthzzbjc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2wdmgudrl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xilxkefh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ksiosexe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jmtpcuvz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2cjqzltkc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nwpxpxnq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hhlfnfft.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tnctrboh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mqlzqpez.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rwrluwbh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2orkxjlye.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2yqhszbnp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hiubjsbl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qgxuatsf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ejfkdozs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ensxggze.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xaitbvwl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2oaudlixw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2twcwejjg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2afguvauw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nsgzyffe.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2kjsdeatj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xjdjnlcq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2hwfpfwlx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fqrwzijw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2fdkchfxi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lrhdttvm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2axgaheor.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2vyqqtlae.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zyczqtdz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2gjvxfjzl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wcgycndy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2szjumfmm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yavpidrl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rspjjubi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2skkomnez.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbhzhvts.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nwcqtjax.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2trcxehdq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2hhqoqgal.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slndjbmg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ksamjkkv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2nfaoryjk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wdbyhyys.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xuiocadd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ckzghkrh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnrgztbi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2mxsukkoe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mquttnhf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bvovwyrt.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2txkoqvzj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2pmidhcbp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ywofusht.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2uuwdektz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xdrxykln.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2pvnntjvz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ocpznxzj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2nfeeygqg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2gagpwzkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ciqgosok.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2necnwtup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmbklafc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vlcbblpx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ksmljzkd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uaepwrwm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2keutackz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ctfttufz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ipkerxel.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2eronrwsy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2yjfdmmeh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2aoakylzg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gsolnhse.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2breshvzq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jjwimqcr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2bcfbyhne.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2sffecbic.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2iaraekxi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mwyqhpxo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2npqjtnxr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2sjnappra.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2zufqmwzn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2asymexnz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2guzhhlwk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2unavbjrn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xzpilqqi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hjorufyn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yxzxnsvj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hfqecndb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2yijachcx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ukqypglf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zdjbgcvk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2aubmhkgc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ahvkjicx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rllcafoq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2kerbuolv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2anjdszlq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jnhnbasu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vstmrvkx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cjbuyjhh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2oqvcbhoc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kjaxrndr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jrbgzuqe.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wrulahur.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2roiiejrk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2okyqohgr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ankxylgb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rlvzivwj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2izynvvsf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wptdlxib.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rfzjkmxb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2smhauswu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mazwjtwk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qthobqxy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2khemltav.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2sngfdnhx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ozovrevb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2twpvliab.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2dpifyoir.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dayiybsm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hlkdhnfb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2znuyoxdk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qwiauyca.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2anopfgmr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ivhdform.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2nuhdxizn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wiikuqny.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gsdxhcon.html


<!-- 参考信息 -->