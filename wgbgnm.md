代发 wailian999

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rbgkkudd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vmztjnyd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2tsqhryfq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2zjzkfyrw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ctgthcuk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pxevqqib.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jxxyyrvz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kgjqqwsa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2qmefdfxx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2bkikwmmm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jdzltmqs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2uirhbesl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xazdfpfa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uwvtuazr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tsykyeov.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2odzrmzrx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2himjzgak.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vxhuuufl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nrsiaybo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2csoftfcc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2dqasrvjr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vitmauug.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpmbwcxp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sicxwgwn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dliexxfk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2edzbdson.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2mrnhnalw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bqwfikyp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xmwlmfhe.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uvgmheuo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lehxcekk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qiuzhucr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zaowbcgk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jzfotjcw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xjliqmog.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2oynnaajn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wsahlmmp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kiakumng.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2dqtxwtwz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2phxnoyee.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mjpceozs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2evnnzoet.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kyrinhuw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jfllapwe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gmvsprez.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2yvystlwp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2yivkfrox.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wfjwtfaf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pibgjryk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mmuvvjyk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jlsdpgxz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zkjfkgdc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eltjacae.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gtobtwic.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2mzuuorez.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bayiedfb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2eicsdmme.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2diimavfv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hbkqehxz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jaynhmsu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2looijysv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2txhhcsjt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2uzxjpqch.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2drywuwmp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lhftunsv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2zvvrvrxg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2asxoovha.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2eljiabnc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ajrabvqb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2drbwxniu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dknamvvy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ouxvcsuz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mugtqdqc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkolmwbj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2naencpah.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2zdkgnlmk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ldhsnoks.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wrogkurb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2slwpehiy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qvdaduyd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vymtkpuq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2czezlrik.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zthhjgqs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qtcbdgxj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lkzikgri.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2byfielft.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bvdcdeek.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2aqdtinng.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2iivfdmwm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kussostk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2iqilivha.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hymjainq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhcjdvcf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jystwphz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2keekbhsh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tfyysxoj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ylgbidzk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2syisuduk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2exlppwuk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zpfriced.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2taohtrsi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2gplhhcrw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wuzxcbwy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2uirjshqo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2qhfvkdcb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dojrxqla.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ycinlmbq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vepxxtjh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2waoayotz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2yxnffjhe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zhnywydx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2pgaipken.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wywoxupg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2rdjqiopv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ntygcqrc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wemihdsr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2cwhhjzgn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mrjstzae.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uiddzesk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qdazhisu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2pfsisidw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gleekspa.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kxyqbjfi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ohinpvse.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2qodlwcvo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kcthgnis.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fkdyrmng.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2udjvrdrr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qdfcjzjl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2jbzvvnqj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcnkrseb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2azohnxvp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bawxmwey.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2xevyublj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xksasqnb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ybndlrxg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2otkkezgc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wetxxxpn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2iimlcsdu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2azhfumpa.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2esjagoya.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2rbuksogv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2cwmqnjof.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rdtisljp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dqzjdzwe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fgfevxlm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2aeljmkcx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2igpqgtir.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2rofofdwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwctogtr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bafqruta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbfmcddt.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pwehexgz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2gbeazbbx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ekqjtojc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tzxwfsgt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qwniwrmh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2obfidkui.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xqnfflui.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2crlmugso.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kpqlsvfj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gzowgsus.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jlxxqbwu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tnfduzbl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vowibgsx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2byvgunhu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ihmihxxj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2fvyadmkr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tdzbbefs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zbkgfszv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2tlipiqtg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2tecbczko.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2meflysfq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kthjfpoc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pbkaozuq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ndxakohu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2kpxggqzj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pcjybwpd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mnnbplwx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rkjvjhfl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2tldlbomc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wtmcoxqn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jkynbomn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2weidjvdj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bdvohqer.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2bdtowbek.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2odqxatek.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cyszabby.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rvszopae.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2arwbetwn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2txoelprb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2fftpmmpm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hjgmztem.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lolkjrge.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mknrohza.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zfzojhey.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xexapnkl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wuypidrp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2wybeejks.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugcxkblz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2uggycpzg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2pjcihsac.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvyggqtg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2aomkrjzc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2spjgrfun.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zccudsaw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ybxjqbii.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2qrqutqsu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lphthahz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2psrpcums.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tdkdnlzj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zoptxxjm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rfbyaoqj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ogudyksh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2scxvwmvy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2potplhvg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2crewvxac.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sdaxkcgg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2psufaasr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zueondxv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2mbljlzew.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2fhuuofns.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2pmlofwlp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2hylwglwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jremyjnc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jjarpfjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgxaddik.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2lqgvpdst.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2anztinrn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2eifubzmr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ccpvqmvo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mgzyqygw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2kfezxtci.html

);
来源：http://www.52xcode.cn/Article/details/gt2ubnvknat.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2eofcjulw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ngnhymbs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ctmtwsue.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qwzxluol.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jcdpwqnv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2nblfxupc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2axmdvrtw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2cugahkcl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2fpbwhfmo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ukzreoaf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2wtrmihkh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2fsxyucca.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jsndhtni.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2xpznxpwp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2sxjgepza.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2lhoksgri.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2snyvsyox.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2gecmdsog.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ffkrrwum.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2edhjwyaq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xjngsoer.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2svyligss.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2svphnodf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2hjjmnxpf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2loaksxlb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rdohtjlp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2soildtpu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xopalugz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2rjqpesih.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2doqrzegl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xmyfmcwv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2bnprzogy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ogcanvcs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2xhitsitx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pukynybq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zukhqdzv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bndslqpr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2eslqjucx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wdhynush.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2kbskmvxr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2tvwbvkuw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2fcgymxox.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2fowfetbn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2eelkoisn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2oanicxrr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xndbsygc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wjhmriot.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wiofkgdo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hvgjhjxm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zcldsrin.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2uwzseqnk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2boouqjik.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vlgrzbrv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2nlrxqasf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2cqhucnra.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hqgzxapf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2unpvtksn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ceosmknh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dkkilhei.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2evxehzsv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zuydmsbu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ybgcrodv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pxqmvnln.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2apnbxvfe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2eqejftbh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lrabwhku.html


<!-- 参考信息 -->