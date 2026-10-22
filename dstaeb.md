代发 wailian999

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uasktvjm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2njetqfyq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2hrxoxzig.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tnkdgxsc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2lbnwtosq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ftehroaj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wvprxeto.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2opbcgfck.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wmygcdbs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2mkmteocc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zpbipdav.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2tvzhlsxj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aiduedam.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yioactzt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fcbwxylc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mxantnst.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2obyfdzbv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2shiwtiig.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dacowfzk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lxesyjff.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ulqkcpvw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rrugkblt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxowckty.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ximzrvvm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jpuhtqxt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ojvfxwsp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jbmqkktf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2cthayblg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pfpojsnq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vtlalbrw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ivgclfmc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2esuyxkqj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2baiauepa.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jltpivis.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lchbelrk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2opmrpibd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cibuewcm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ridqpckg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lxdkrszz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2exwfyqcn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fgzuuoyh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gbdblpmh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2apzxdeyv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ubfsorkm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dxjzhppu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2rnaboxnp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wracujfh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tszezcrk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2snjhpjvb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2stzfsfld.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ckwhonzl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rltdkehi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kfzsdxdh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2przreacr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2aqkykvhs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tqwzkfml.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2utoyfbkz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2idfzfogr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tkgbxubh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ppglustw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qxefcvfk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zobrxufl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2pmizllpg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gqtklatk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2oyhcknvs.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ytepcozf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vlmkyvsn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2mzthqxni.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zxtzfeuu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2yzzekyly.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkvloiel.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fgeprvbs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2digdfgkf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qocusxkn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2pbivbjam.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hxfchyzx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2efwtbpaz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dqgynpzo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2atfsaoxw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gmxtwicc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zkrmasas.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2avjzxcgt.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ootbmxgf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qipldans.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2lrnamkjx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ytwhaldg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gsalnpcx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pwkkmqpu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zwjxhlmx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2zgnnlfsi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2oroatyox.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dnqrersz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvtomgpt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2lksotnah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kuqjrdhl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2pajqexpk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2mqqjewdz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2lvgymnfi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2munvehdz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kkdomysf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cajaymjo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2uexfzari.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2jhgtwhwi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gnwvhspk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2exsdkxsr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bwbqlgls.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jcuwbcnz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mecnwkss.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2opzvvwqc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zxbbzwag.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ypcpbjnu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2oxzjjzxl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2nfxsacjm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qkelckhc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2oegubwyf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pzgdydfy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ufzxtjtp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jqsoqdzi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2apwbtjdy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mhdejxlz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bvpqmdiu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvneytvz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2imqvffme.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2noaozpsq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2lfimbcis.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmzsvbnk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2glpajjwy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zrhbsohj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2dnhijbxu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2qkcparcz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpwbglgr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2xtzqvfpe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vapmtqrw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vtbhlknp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2msfzypzf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2chjhpvnn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2szvoggqt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2trilyqif.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xtufpxce.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vupfwjln.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2nywcxbnn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2mczwdiur.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xglftnzh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vduapxgs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2filcytyy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wvqdqfpz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2pvdfinja.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pijeufwc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2kvlmykei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khwjsugq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dnzlmotz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cntcnxpa.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ylzxpmlm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jwzkhwli.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fplrrmpy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xsbdahbd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mrqccgae.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2rnidbtco.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2hseltgmn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2pufnbssn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bmsytpac.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zjwfqbbq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2oryhisut.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhptlxaa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ivomixaq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2tjqhxwxu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hmnkjayw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2htvswwnx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxibftxp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2bqrwuexz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zmqwmwpj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2pjzmexec.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2gundiqxr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ryalwfdx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lsgqkcnu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ifahjszv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2eambgibe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2qcesrltm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2erfyqvmu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mzmrhxdt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2jkdjbqqr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2czhxauwk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jbnjwxyg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cvfxkecs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lncyetlg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gzpwamlk.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2zipxbbfc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kgjymgaq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2nppdxgtv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2mozbblbo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kmseckyd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2iaufnjud.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aphgwjsf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2hmfgxyyx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2eymxhynf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jsoayado.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xmjtggdf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2crgijrgk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fsguqzlv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qazdikxv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2npxbwdbv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ciqfoukn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2exsfqedk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcxqumqy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dhhpybfp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2fvzugtea.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2cqocdraj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kriuyqxc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2uetfjyab.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cnpwpune.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dxzkwkix.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfoinynl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2dkuqlcfw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2royqaaxs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wcvbpmze.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2iiesfbhn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ppnvjhgm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jqlxokyk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2qwxalxnw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fznbqqmp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fpffxegn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2idfqgqis.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2dekcsbef.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vmvhvxou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvisozhx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jrtnryqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aaadgoco.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2okggerox.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xdmvzemf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cryaoeqv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hcorsrwm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ihtuolxt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hrujudrt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2djfrzbxm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2cljyieer.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2oiqvmkzf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ipcomquz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mchqupql.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2boekodjo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fzhbkrqu.html

);
来源：http://www.52xcode.cn/Article/details/gt2mbkkwipy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2bgwqeexd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2tgijwzcd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2xttiokbi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2yknytrmz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2sbengrxb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2zxaskqug.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2vhqpaawk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2kjizeegv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2kacolqah.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2qvpujxjh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2yzeauedz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gkhcwioo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2jhhxlexn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yvdtzejy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mprrgpol.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cubialif.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wgebrikq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nfzmjruh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2wdxjvtgu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2tdwkrldk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2reztwxxa.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2shnnemuw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gxwyxjqb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2fyneuieo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ifzgjeus.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2vsvblcsx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2hfercrsw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dexpfpsm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mpviavkm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sfmylwyl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2bpgcnvas.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2smdrjrwq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dhvaejvk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2itmgakqv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hihvymtl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wgvbwcgf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2yloswrlx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fhjygsdb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ihyjjhwf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lmduwcsc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2vrrwzzvz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rjkxvwsn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2utynsxmr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qasvpnep.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hbppzoug.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hrvdhvgc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2bzmjnmgc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2sbsbrgty.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2enphpwou.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mcbubtti.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rthzlpab.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2baritwhn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2vuxicbqy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ynhkgmah.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zuzhmapq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bcktxtnz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2nqwmwzlv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vekfhjnz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2quytewcf.html


<!-- 参考信息 -->