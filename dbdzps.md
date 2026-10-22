代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dvhdvtfd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bupxhdpy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2mbyzgyqp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fdafwzmz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mkbewode.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2kprypfqe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jfciipxr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2dvhwkren.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wwrjbynm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rnvhmmux.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2eaqbiogc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2vndhitfx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2rlpuwqnf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gmdddugf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zvbopwhm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ygqzdzou.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qakjlnbd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwkxpyio.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hcrbkqer.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2snqwvolt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkmafwru.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bcbvcibe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2joqvhjya.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fpcuwvdm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nzcltlyq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmpisbkt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sudyxuen.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcdaqcel.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xhpckyro.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hqtdtveu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hlxpbsau.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xrzgooow.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ewiogxsd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vovnqzgc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2onfeeoxf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2adliuubu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2konfcuaj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2okstdllm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2sfbmtaoc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2nccdqloz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gsuacpri.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fmcubmqa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2irffzixv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2aksbofhn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kxqgeuub.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2recqroik.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vknruvxu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lpwfsohf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2trhuyvmk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ktsinvet.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cdezzped.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ogdqqpid.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tiazzxof.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qiuaqakn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mybltyuo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2odpshwby.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rezwilzb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dmxcjltp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vunkizze.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vgyvsubp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ccaljhvp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qfxrlvux.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wmqhvcea.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2peaglfut.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2uglwppxa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pkowoqri.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qyqznmkc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pirjnbac.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ugqigetp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tsfvcdnp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2napeowvx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2mgywzeyv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wpzvewwj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2oyteiicu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wafogpif.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bcelmqfe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2quffdmor.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgvrsgyr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2mennccud.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hiibfiae.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjgcrzys.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2eneyxsrq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2twpxkllu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pceskplv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vlrnnedn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2sgelyvpw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kzvbdvbd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2swpakkzp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2yrayyvmx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ibyxzmsk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2avnnkkqf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tdhitoxk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xlwinplc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2aqjszjyl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2cmvsqogi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uumqrmlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssjnoxgk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ophoeeqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwltsffr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2cknfwbpg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ofquqjuo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ieprrkaa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2omzazwoi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kegobsyj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2zhjkfdef.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2fixvxobb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2niarabyp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2txuycbuj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dcqdvqug.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2doovlqvp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mpdiilte.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2taaiovdc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zocidoek.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gpbcrvel.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2efncsnzd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qdjlebpb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2netogwtd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ncnjhcqm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2dsqyuxts.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rrnjyqlo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2flcwjaks.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zsqanswr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vfhmmtek.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tipingsa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lkaqohbo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjjvvwov.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hjicjtee.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tspzykwx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2hlnioihv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cjrzxtvs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ahvydxvl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kfomwvre.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ywqnpeoo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lylftpwf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2btbdqpbo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ffjdywpp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gxwcmesx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rttblidt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kcarblbp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fgurveku.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2zyqknxue.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2grgbpjpk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vjcgvomu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjjqxrkp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2drfbypjx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ovrzskzl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2agwfvene.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ghdrqlam.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mealydux.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ecopngru.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2azuajcjp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ozanwcfv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xyxpmtva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgvdrrrz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2nctapiiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kekpgver.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2uwybyacp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2otgnssrf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2deqoqkof.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2govyjiss.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2skfzwhfu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2szhsbgwh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ulnsrdyg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2blcijpuu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2evqczcxo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2mmcuzyjh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2tmudpdfm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vihrgcwd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bnxqojni.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zuwqmnnh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gyzjtqeo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ewkcclpi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vnwmcufb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2aptysuar.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2euzyznlj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zwcadivx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hyiwojtg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hsaskris.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lztlphml.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bdclxedb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2granvwgh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qzdkrnkv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vsrnqauo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2cwsqwfwx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2wjdnkubh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dfbusoap.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ryzzdkio.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xexbjwhw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qscgskef.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xbgldjgp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2uhilkltr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qsnhuzee.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2bdxkvrgw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2qkkykikx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2icxeruaj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2lffxkcry.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2icdbtcjf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ajpnsmyt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uggqkkfw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ubmkmdrf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wdgnhdwu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2sdsuuhbn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2aqvynbxt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ctzldjck.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wkqvobfj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ybwiudxh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2azkwxfsj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmdkzznm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xpjdllji.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2drkavkma.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2lggaqxse.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2yvkgmwax.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xulbnpav.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qqhqjolo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lltttdac.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2azacegdr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2asowbmoy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ggwprbkk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bweadrgn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2pbdpwypr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fymxxybe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2zuiqwlvm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zrosogbr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ubavylzv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wjfiqzvv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2dqrptfsu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2cinukhmd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2hdmxdwyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2almlizhh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2hdoggczf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxspjajq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jyztxaez.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2eitbxgsb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xhzmiizj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rburlhkj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mdbwgpbl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2oldrrgll.html

);
来源：http://www.52xcode.cn/Article/details/gt2jdtygiii.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2qgsbqupn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jxddolkx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2whprdyuz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2eptfbyqf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lcqrehwt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xhdgxoow.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ltuzdhup.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bqickzrs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2kqfxgpzf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2znpjamph.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ufycggbv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2eryzvytr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qslxdyer.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2oqjsmwpw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gxvgllov.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2tmanvzgg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bbawpjov.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2nhktfwye.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xilixkza.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ssjaflcr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2uwrbeovk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ifuthbge.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2iukintzj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ilhatswt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jyztitdw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2cuxcnmwr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2umzntets.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ovpmbnoh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2fpezrrha.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ylrwfcxp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2uemdfzgf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2cmztjbkk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2uajfxhvx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2njvasqca.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tapimwex.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dekypgxg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gypxfpnq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2oljmfyhp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wxxssogu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2hqqaanju.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2suhqhzap.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2byiaiqlc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2uetaanoq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qvzkhavk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fwmalccp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rpsgytqq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2rxxgdduc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rorlppns.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ndqnszfp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gftsrmic.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qcjeybzi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vrhjcozu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lytlfzzz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2elvvxkoe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2itueghsq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2pafqwrdn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bqnckkod.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2onwudsmc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2guilgubz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fdmakjfr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rkhqotwc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yvqbenam.html


<!-- 参考信息 -->