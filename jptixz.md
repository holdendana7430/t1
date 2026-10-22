代发 wailian999

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zplscqru.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2rfgelzqe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zwvdsqom.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vjxzahdd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2poyussbq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mnzuubgm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uerbxtjh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yrejzoii.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kdbrutla.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nsweklxw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2eqavswly.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hoavmmed.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wcjzsvzk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuusbhvu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lnotoeka.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2odrfbvrd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pbmchjqb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xycmqlst.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zzfhzneh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pscrkdge.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2xcidqchb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ltsfzxdr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bizgdwgc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qcjwevgg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kgxbpnds.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qppdqudy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zaxuxsnw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qyaxsozi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2aewgpfvw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fvnhajwg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2clyukeei.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qrsvpczd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kgnpfmen.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fqodtsqa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2syrpzleq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ahovbokv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nsgkrnzk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2alcfihta.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2azqnkugj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lcpnownl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lqujghpe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2eegzwjbv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2cwebgjrt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2tqvmkhlv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cyqakwzl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wdoaqpyl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rcvvxvzi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vbdrugin.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yvivhmng.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2sjjqmvzp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bmwjwthj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sngaikee.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hiukawph.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vcecpaaa.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qukoqpoq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cpsicmhi.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gtzfnjyv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nrxdgifx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gvjvgxlu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mvlsjrwy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gdtmhmxk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dyhibycu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2lnjvmnyf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mgyjxwab.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kormcziv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2pqrqgmgk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2heyfihov.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tckcxzwk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2riuegdsb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ijdcjwio.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lknvzdec.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xrkgloxs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ulamwcni.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zlwdgafk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jknkpvtl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gmcbxdab.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnjboycm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tkrqzedk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kfitlbvy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sciltwnr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jldvjyen.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2yvmuewzm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ncqnmcoy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ludvrzoc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zaqiyxlp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kylndzqg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2haxodobr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kvjoxfoi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yyuzugdr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zhszdxsy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mluvsurx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2axtxqoxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkqaepmy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2vqzynwmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwepkvvj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2luzsqjju.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wrtqhbsh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jlvrkeiz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2wzcnlooc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cpngrrmz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2oxfqwnpk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rdpsagnw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2popuukrr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vcxshrcy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uqzsnxju.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rzsrihuf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2igirehlw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tjyfbeqe.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rueifyob.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iubiqkro.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2eqcggcve.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2tijjteni.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2fsgwcjnw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2rdncurkh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2bwqkmxiz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2mkgrkoxj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2nrumdogc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fxyodnsk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bxwmhsuq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jzmfbjql.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gwsuvwbo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjuhcjxr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ounmlhyy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ysfkzwmd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2zjrkfoxz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvzbsdmg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lwdpdkmj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rfwlggvc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2eechmgnu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2jkdfrvbi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvmevrxo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xyspkkxf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2imzbqkbi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xbcufqhe.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2grdankro.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ofsiffru.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2vwcaakdu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2apjrhrib.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bxyvgdyl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xdoobvfr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2cpqycpay.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2mvgjgogj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2turcnpsj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2idgitcgy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vcxdchlh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2loezgxsx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2thiwmicw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ekyrtyyk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2rsgofoeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwhjjkfy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmejfrsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnunavxa.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fafmwprv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2btpfebgn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jgwtrjuc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ecwasoch.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hbavogjs.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2cqmwkwen.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tepuaids.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2isxjnqhj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2crevebhx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2grpwhkfu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qzhtfxxs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2praieobz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tgfiifao.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kippjhej.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qexhslua.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zxwysctf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qfskfzfr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2bfegtlle.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2avgfmdgm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gdkzixzy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2alwybycw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2umalancs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ejziipuu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xgwxijav.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2mwysjkfe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2bqsokztr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2szvaakiy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ydfnqzvp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2eupdhupv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zzbasqty.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gbmulqvg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xlzqfzej.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ajkmxwab.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2psxirptb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qgqwbrfc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2isuiiorg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jgzjjjfz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ywuklxxb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zdpbgjgt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2kfrdspmz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2npqowvvf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2uanldsvd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2idsgvbsy.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2rsjyuwme.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xlsqvbjr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hxzuxhzn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2thizbmhd.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyfilnrs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2fqlhhiwj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rbzuwiqr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qtpwjinx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2hjtmcqdm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2gtwkolic.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujcqswni.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2zcuyosyj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2bxxfdgjw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ecvgaqzo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vhslcxbw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uwbpwjig.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhqcjchr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vereinvb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2kdrdmhwr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2gsozmhnu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2tejlugcf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qjxaexug.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2raifagjy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2oyxbgmqy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vcojzuzb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vfmjrdlp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ozxxkshj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2dwvvzayu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2njeawzek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oflpostd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2utraxukz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kcwyzieb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rlcmaecv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2arhnpqpp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gppezjdh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xiuhcgek.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2rsmugghk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2nbqebjod.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pvecwhlp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hkdftkvr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2detunwka.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dnkiynuw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qlevcmti.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2empaqhkk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vmmolbbm.html

);
来源：http://www.52xcode.cn/Article/details/gt2cfymqwbo.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2oplvyapj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ngtynonn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2eulsolsh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tpqubgau.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ggkbrzpb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ktjijysu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2sguzoraq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vqpgrago.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xtwjiwxe.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2atxndtah.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2tsfzyfyz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ppzigwro.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xrdtchru.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2askayscr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mdylfsbv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2aqvtlubu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hmvlsuhf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2noxxuzmt.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ondiatdq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2iuikwnes.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xrdmbqxa.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mldyphpa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2eszsback.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2rdfeulwo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jgsfsabk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2naezgctq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2asohqakj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ivjvlslb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lizmmzjs.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cbzvhjgl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ggwtvjue.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2phsihrjh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fjwugvkn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2cokzndtx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ltiiwwfo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vjpwoxxi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yyhwqwla.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ugbumhzn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ubqurvsc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tgdskgxl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2luwcczmk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hrwicihy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2pdqexxop.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ujraxwmz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2tngqixtb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hgpeondd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gpagufoz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2zefcouav.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2kbfnjsdf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwiwsbma.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gayexgcx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qohualox.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2kkitqkol.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yaehhnfv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ufcmwxut.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wfnkghrp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zccxzeuw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pipdmvwv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kpmqzajy.html


<!-- 参考信息 -->