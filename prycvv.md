代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mfnurgvq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bfyyyqyb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3geykaaie.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kwbjjuzr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ubpuacli.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oaubgzqf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3aeljpatg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lyceptpk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eyjqlijl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3cgditufl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jfbrsodz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3pewhgywe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3uozraqnh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3voyixrmj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fcuqmbht.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uvdrglbq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3qnkfrhan.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ridmvmge.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3thyusitx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vzthzquk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ycuhoxik.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3udbtdfec.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3amnvgihb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ohnezwlc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mbzdhmml.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3sxixxlaf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbxczepa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ljmrpifr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xtgqbvti.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hcwskmnx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuebmwqo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hppbswsy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3sgjcheud.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3fzhfnjrj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3cdsfxmnn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mjhijxnt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsdnfhpy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3isbtmflp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qedwftem.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dbotomwr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3stzreiyv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fdignluo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3goagaxlh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bqvcjuzx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wvcagwxz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ysspnwvc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3wlmojiwb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3dexhqesx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pygnxgga.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zebmwrmt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3vtwjfrae.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3nvdbmlnx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rikfuxmt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zumlldwm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qrowfkut.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3sjsmtbnz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bqnndqlq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3pzzyfpai.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mqzrubsy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jpetdzoi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lhbcqvyp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oxlucaec.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lhgnotdx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vcgvkhez.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tkitwety.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fsndkgqx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yusdhsfh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cctsngow.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bdqtkxhr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3svueqpvy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3gdmvhgev.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dmsqgpiy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jdxlcwfk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hzawftoo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bkpsmijc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3efmkprib.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3xlaidebn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3znvnkpbo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jwcwlyns.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3uslixuwg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vxatvmft.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qgyfwkbm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3qekjigoc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3vvunbprn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdtkywew.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mdpgfzqu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pwpbvqjq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ftjvisoc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qmohlxlx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3yombskxo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lfewcdzh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nppgavvk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wkkmnbnv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3udwxcxve.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rdewbdrq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pbjyzcja.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nyzsqrsc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bpgsmqln.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3aueemomg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kqhsfyou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3peienaus.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wrwwspwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqjwuksh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ehanjccr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3sfoytbeq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3bebmxwzu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3aflemizt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3anyvazzb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jqarlfud.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3xuzkzxrz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3genielfm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dyafdzdh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zkmakjge.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3uuqvgpcq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3uovrnbss.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oifgdwek.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3aoyfktet.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3vwlkusmp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bznockzo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3yvijpbtj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3abvkfmcd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fsyxwawv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3uqznxfji.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3rspniyqw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jvdpojus.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zwctdqpd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojfplweg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qfmgyfwy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uxtloxlo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3saktfopf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3owgszboc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3sonkchmw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tldalrfl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kuyqvkxy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3truciojp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3vdpqptaw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xmnhsple.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ulbkujfy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3vfugpslj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vsahutpl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rmwhoxyz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jgzacxrg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lxynhvdf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nfoqlywz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3swlfyuva.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lyaosoiw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wzsxfbrr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ddlwdkds.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3tdtgbsfs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ogbpqtxj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xfcylsfx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vvwbbgno.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3iwsuznuz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cqicgyxm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qtgmvywu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3pdgvsppx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3gauvnayv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbuvrsgh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3jhyjmqbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zidhpydg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3chbmvwau.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yliavhbh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wrftnhvm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rrdduqqg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xhgoroae.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3koullfju.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3biyhzotb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xdzxgqlf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ztgfjwns.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3pggafmuu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zxgfachu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zmaicguh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cokbrcag.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3obxvicdr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lbpaxsfq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ddacvcun.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmgppokr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3knbykliy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vmdxnntp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3mbpavnfv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3lvdjahun.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vaefsekr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mdwmcqpu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3nyajrchy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xwmrbsyt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3muddiuag.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xbyjmudq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zfkdkpze.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mrwuuqsx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ebelqnwu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tzhzusbv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3psstckjk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ymrwicwt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ffqjkgka.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3gwvjcvxi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3utnrnwav.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3uvdyduph.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xvsgrcvy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3idwxeyaq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3jteqctil.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbfbmel.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jpvxabhp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dfmlnsiu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3aakykwyu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3aapulryx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3qhkseeom.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3njplpyqf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptckoeza.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pbzaofcx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tehhhuno.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3veutqmzb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrmbaoaj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zlaczgwl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wnemjtrb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3smbnilkw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3kwtdxajm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3pyhhoewu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oqudcgxm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wizegdyc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrfzprme.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3qsqcbwik.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3hjrwsvmj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wlulpnrb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3pycyjlae.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pfrcqmxw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wuvmvlwa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fxuzleqh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3npbayfij.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3lpocadqz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jdfmpicr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3sncbfbpz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3iblfzgnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auxdolap.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3aywndxve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdxjklek.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3avpgdpvz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3lsrmxkrx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3oiwuecju.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dhjpzvin.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xfopsvuc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3fuayfbhg.html

);
来源：http://www.52xcode.cn/Article/details/gt3depvvtzx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xefflhch.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mzofnvrt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mnroacee.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3labkaubh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3kkwylmgc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qwpchjqg.html

);
来源：http://www.52xcode.cn/Article/details/gt3twbywmdr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3fmoapikv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3pixljksu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3izldeqpd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fgmbicpt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3inttaqrw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lbpxlzxn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jviclvoz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vdtmsgzj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3oyywknhy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jgjydojn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3dlcsfdhb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rgvlnoup.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wbejwnig.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xpwtseme.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ntsjrxko.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gsmcrxcu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3eamnkqcg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lnohkriy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ndjwgkpy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3tqthjybg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3bnpcmyvd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3nsiahdwt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gjijvjqt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3gpbjhhig.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zpqoduse.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3aurzuizr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3aliyhcir.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rcblgwoq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3iqilvgpy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mcrtxadt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3rikkhdsh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3huzkmzio.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3lnimrtad.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3kydtrzjq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3nfkxsvub.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3rvaafqnx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3cdtkyzfz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kcqhmofo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ebawozkh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3agcwpiqd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vodixlqx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3nlwwijry.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mrwsmrmc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3uwkvewkk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3qvcmgvgv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hcrzvavb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wakavhqb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3yiklbvcm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ofajmkot.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3slsvksvl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3lqoafopk.html


<!-- 参考信息 -->