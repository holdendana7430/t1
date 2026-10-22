代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ogiuxmlc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uewwphji.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hwzajdcf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pgqilkhc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kfdptecj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gvkkklzq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tjyndxki.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2cjwdxwjd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2nemtcpue.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2haipvhtf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2eevldycn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2lpaiwmjm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jwgaqtdx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2fmzmpiuk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ylkzkidu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xxbnlwof.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wtkknyfh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bfiqhpjf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2penbwcvk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hmzchldk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyzncnmb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2zgggptqg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rxttijnn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hpdxrdco.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zxtryuvh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lotvzcwh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2chhszwwx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2imgaamwb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nmbxgejt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2sjoysgoo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jtqypssk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2bulbbhkf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzlecndq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zbxacmlt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nxiwteat.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ahantusv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2krctmqrd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uersrgwx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2kmirpmtx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ubdditau.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eisxjwyf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bqjxsdpd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kqipjzpe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ttvcyzje.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2euywmkvl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2dakmgvyo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mpzmtxjr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jklxuihy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pxdamokp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2cprnpbgt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mhhphdhj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pzosejkg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pgmefabf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2nhjcyskq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rccrvpyq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wksnwoxx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jhvadtzy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fwccagoi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wpihtqou.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qhojryol.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ebxktebt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hjeiaekn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yxvanmcu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tqizkbov.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2yujjmikf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ysfszonm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qnlpolyz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yxecpadf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2egxilphq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2hcazftua.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2lwnsazxz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkpmosfv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wxboxyta.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2hsnmegow.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hqwkudzw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mngvanyr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2oowgggay.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gikcycjo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2obgnlyxy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ubjbhcmj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rghwhley.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bfpobnsf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zgqimtfd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jnmcpzed.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hyuurzln.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2gacanmnm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mnvtiham.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xahilpkw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2eedzuijt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2cnimmiyb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2obfdfmkc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2leuzrvdd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lbsrnpgq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2expsizot.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2xfkdmzto.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ixaqzypj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qaxxwfrl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2bwgkchmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okmbwcct.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2iicqgpwq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vefbqouz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tklaqfdw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tbdxkbzb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zmsxksls.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2upwpglgv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ukcsuedp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2seairosq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2gmpzctwo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2netifpmj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2lykeyvsr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mhphurbj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wqbwotbz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qvmzytrq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vixldhpc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2myqfengy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2dxgjfgnz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2woxuzngc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fcpxaaha.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gquocfkc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ynzyyfrm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2gsdinqrd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zanspmcn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwbschnm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tkkdtnol.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gproamvj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gbghyudw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qsttwuhd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ghohctrk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2dsgmypmm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbpfgiyt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bqoceojp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jgtsdedb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2genpfmrq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2amylsqnj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2onercrwk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jnxcmetw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qcqirein.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2brvxrpqf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2llvsbrfq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2osahjeck.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ymiqaetn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2pzypffhf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bdljypvr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuxqopdy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2fukcjmqj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zrrbppri.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rzafeyob.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wwqtivcy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2orlnnxtk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2jynzznls.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2alshpvxx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2aeryfapq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ilhszenq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hobtlwpu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ooeaedeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfnkcjmq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2sazdewys.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2lygwrtpx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ibroomkf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lxjxmadq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2twajutlb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fqqdjiiz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qoayjtma.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2sdqlempv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gtmbqalx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ivabcbbs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2kwndwzqy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2bmmtjumn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wjnqniwd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mhbxuaio.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2agcyikzl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2hcvcunro.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2xuzmifbg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2aqjdzotv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qfcquwhq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2tkglkvoi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fjkokapd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hcxozvxr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mspomkia.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xuxhhvai.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2kibshktp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pidztbub.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qurgtarv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ladfoppa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2mozewtzy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rbkdpsua.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nrnmdgff.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fojksuyb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hylctmha.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2bfhtnodi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2akowhvst.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2egntkweu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ondcnuat.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ibkfmkec.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2nfjzmglo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2punwcwlu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sbxzajur.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rrlwjtrl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ekumnwgs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2tvxmpmle.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2vgpdecnm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mspkcaqd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zfqvttnm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2golzizlc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qcxruyqb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2risoeazb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fedlghus.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nujcsqde.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zefyyqzf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsbmxrml.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pghrfgix.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wixnaubq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2bibmhntb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jnzlrbyq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2icjxacbn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2thgoqncj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2jzgiybvj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hnamkjar.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2iedzzmtf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ufspdttu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gqcmnqff.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ekmhiuiv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ncthgzeb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uqcgyiqm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ogiyzzry.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2mkclxzvs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2rxeuzngw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2lzcpoiqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqubfauk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fsgnqryk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lskgpppn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2srgywluc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2hpklslgk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gpotbpiw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bmbkscvh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ytczjrdn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2zuihfhrc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jqcdkvsv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2nividkpw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jcisusjg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mrzmtvyj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rryxjmoz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2fjtmzpuf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2evrzjalh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cvdxpulk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hzyyfagl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2lywzersu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ipwewkgz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ifljmgnj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2dobyskaw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2gkarvbdp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xywmqqfj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2tspfmnvg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ngtyjihp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ljpwwxcp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2iyjpvrtv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ljdpnedh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2naxrrjec.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jagzrjpi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mminbecw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nxlakbeq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2iqzybcfq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fylipimq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2uclntdmk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2bdacaaef.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ysvfcaxy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2fdnuutth.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oxkfmtmj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2tuukyxvr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2bkfukuaa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2nbwgktmo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pyfekpgn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvizvmtq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2dyzamkpb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lgdbmeew.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xavfwalk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2leqdroyb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ulcbxdfp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rdhgohuo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2zxuchzmi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cwgcopyj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zbbrwkvm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mvotyvtw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2luegvege.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ihraqdvv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rvklzuct.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ttzemjyj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wscrpjbv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ikjolbwh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rsvmpbaf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klrxhgmy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2brofjgxt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2twlfxcra.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2rabjgnhu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cywjyhmk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sudheukw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjpoyyuz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ototyyli.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hfydxibw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ohsvxezy.html


<!-- 参考信息 -->