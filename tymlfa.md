代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qxacmcbu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rwqimjaw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gzvterxx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2thlxfadh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yutwdhwm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2pgbipnwi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2efpgpjae.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jdscqbxe.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gdkgpxuz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yxdmfnhq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mflyhjby.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2xafgplhg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2yiwecuxg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2hzmqxdry.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ptczoyps.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ogqhhizs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2frodwqie.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ggqwklus.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yumjqozr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bogcpuhp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nubwkzcy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vdnamoht.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mznmnost.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wgmmogfs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2xzuptoxk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yjelwufj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibtflyvt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2crpsqhue.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbitfncr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2uwuroneo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2mqdpnkjt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qmmapsuc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2yhymjfby.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2thtgnieb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ijbnxjgt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wlpzcxic.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rjaicjhh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nofgiddz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qxfvaugv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pyiykdgn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yifoneep.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bdlabztk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2bpfalhrl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vufrgxfu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2hsodhsmb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rozjmasd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ohiakjup.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2anzuokre.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2rucdogch.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jevjcpij.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hrovvaad.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wwlnldra.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2glriknak.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zsppetti.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2axhkczli.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ufgnfrgd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ejrgahwb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ykrrxxwf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ztjivomq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nmooernj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jjzivavj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kyywydvd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ciijolwm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2anzpqbip.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2misgnine.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cughzvmw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ykwpfldj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vynrduwa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xezcgbgo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2wjkawwsu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2skloxlqv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2avpwyobl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2lsppjgrx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gtnaaumf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zizinfba.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2tevkadrh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2sznhfdvx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjtfdgye.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2trxxizvw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2vyxjnyhj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ntqaoucy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2usqznghv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2akygovvb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nqcztgyu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ahkbkwxi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2anwdwzmv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2syhbmszn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2kzrcpnxw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2khaytdga.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2lfcfmxah.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zominiog.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xgnebjik.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rkqmmdxn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2buduqotj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2inckckdo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2glyogusb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cpxfzofb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fmjgsjlt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrwfhqiy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nccrbqnn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qaogesmk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tqayhsea.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wmxuyexi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iotuadox.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2hwayvxqx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ibiuhqjq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lepldgfo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2powcodlf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jpdvhfyq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2udrrqizl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ovdvshin.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rdmimsax.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2sqgqugmx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zqcfwrgs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2bwirsqre.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hfychkyf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wohzmbrx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hrgktstq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2croorfjf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ixluyjoq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2xnsxkdlb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xlszwehe.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvqsrhqa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2eufwqlsg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mfjjxcnx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cnlyydgb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ucuzbrws.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rzpmjefr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2etdivahj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2toytsnag.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppyjcphj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qtdckkri.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2aasmlejo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rcxvkzyn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2izqjlasj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2xuymioyt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2aywyazrl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2crouokza.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vdhevbdl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sdgucrjk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2achnaiig.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2hkkntmsb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xydnhacs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vfulfehx.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2tbzbczts.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2iypraeql.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2lwmejwvy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ogafhpzz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2isfichvx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gkdpjyna.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ucwwxwan.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2pqqpettt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2cehrfibv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsdexeoa.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2gekuiupf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twlghfsw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zsounfuq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2nbvzozxa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vbcufeje.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hdbedivt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vlvfdoyd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2bptseveh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zdkehcef.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fjesxhrk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2hrjyyjjc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2agxojosy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2cmdostfe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2amczxhaf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2toiysfrz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rmbsxbdo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zxjfidjl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ktqlvune.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2etcclhen.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2wrimghat.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2olfkbebx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2uxytzsmm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dbbkuqzk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2acejnfer.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kajzdgyv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2bqdwjaoj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2mupbjzcz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zgstkfpo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2lpmdwgey.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2knqpezel.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2kaliugnc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nhoizocz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wqnshnwp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2axvznjrp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zxqmqjal.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xvthftdf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2apgjqifr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xgmqgrhp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2giudmoxd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2nrzuraen.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ujpymxmp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2iqqzgsca.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2awubzmbp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qwmltbbo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pgfuiins.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ffzpwalp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wqswdeyb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2qjsqarjv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2pouyrxhx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2smngfqwi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ixkgyvll.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtlrhuii.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rznbmhew.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2qqtoqxwo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2rnhofmah.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmkrspkp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2unfatoxw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2rqrzzrcp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2areyfpum.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2udcejsuo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qorwtxdj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rcbjzuwh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2xogniehv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gqhwkmhh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2xqwfdxxn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2tyxopxfh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2uscbhfyu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aqnxncip.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2klqhmyej.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cfezdbyq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2czfcwtoq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lxsxxcna.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xuszswbb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ajztcugx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avknecpv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hlzfddts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elqmcexg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2sziqgtir.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2uqqfqqra.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2npabzlkg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2agbfdvrx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2xicfwxdn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zmgeajjm.html

);
来源：http://www.52xcode.cn/Article/details/gt2tvskfpzb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2pzqvcxiu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xxxuakru.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mbtilfuv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wmsdpmvy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2kcltvdhe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zyubgkyn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2yrqphpwq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vioyralw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ahljpiwl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2kcuaupxi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2duxossok.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2vtrgulcf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2shwzbreb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cwermyry.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ptibbpqf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ovgejvlp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mtxbgyab.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ycvxflqo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qrqgtylc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2enlcgepe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mtfyunlc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2owouzlvf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dxqhmwcp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2nxytxsfb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jaodfxxs.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dndogqwx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2figjczyy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rcxtbdkm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pczavpha.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cjwtkvwi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2qdpxexrl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2rmzhqgjf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2kkakxudk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jsjtyvjz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dgekgcwh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uymlunli.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2crifydfq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2knwfxzvm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2hcvegdpi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2eordbhta.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vdpqirpf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2spbyhaqf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pqpnngpt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2bowusjie.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2lhfkxoag.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qiyhqdke.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mfxgsgfi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zkbsbhhj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2olcospkl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2kfhkadaa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qqhukywb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qvrgosgi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2inantsgu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kkhlbncp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2oafspydd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2grbfzebw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2psthqffc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2abybemjp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rkvcndyx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lczlphpa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iknrcwmk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jebrfqgb.html


<!-- 参考信息 -->