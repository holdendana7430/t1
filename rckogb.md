代发 wailian999

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uaptuxcs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cqnopipz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jnyhaqzs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3zjqvacby.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rglywkrm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ibttaxte.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3felrgcxz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jbffuipi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3baytbqmb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3pivtcebx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3dchhmbaz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vbdcmsbo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mjkmetvj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxwehrio.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fpkgvfxh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gsabpbzt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3obywrbzj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kuupqsan.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vbqkaihm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dudmzwxk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3esiddktf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nsftjgvm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3mvresdtd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vnxvnpcc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3caxgwwol.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3pjtcmkqg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3gxsoailn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oagouiev.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqlnxrrr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3pmnomthz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nsloqjcl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rztekbjm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3urnxezbz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mqzdgidh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xpkhygwh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3waujgwle.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3efuuttkm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bcdjsapd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tsogjvrr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cvxksrsc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3bgiqxzws.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3tbfweeak.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nqgzgrug.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jojvjzsa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3atspmvtp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3rqcjaifz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3jnlnzblu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rkfqqlrb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vawpwbxi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ojixcvaw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aycurwze.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ixksyzct.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bwbtpcxc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ptohlbhy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mkslrgul.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fafbjwgt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3sajxtvkj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rcnfsqei.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3brtcpjhm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yczpjlfl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3qhzgvbwa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3edbrdhlc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mxkgmdao.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3drghyukl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fdjdayvu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3mossibpb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3pqjgmnwz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3alhzkgnp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ujmkjvdi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3vmnxkslj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sklqlitg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ndhrfrni.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3pshycoby.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3bkysfdzc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kpvxajak.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ngofzhpx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3sunkdvuv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ehuyjcdi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gpxdnqcj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wpclfzqm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3owmmjtaw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3afpjgkcl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fysevhtg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3uvtagifp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fgyvxmdb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dfzsdyrh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dptlxajx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pvkpqzjm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3aduligfo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3mwmbrhon.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vtourjgk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gbhxvqom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwudhpmn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3kqfodruu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcyxzayx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lgfqkdpg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3nvpqgnzx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3tuqprnwc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3fvqpfxxt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kazelxql.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rpyfcmkm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3qfchjszx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dhfkesgr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3npbcqref.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ncqqrxyo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3prasyftf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3cmnlased.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kfikwfzh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ylurcyrc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kfemhtau.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zkgmtfoz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fwakahdk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wcuiyyaf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3umlmqaqn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ltclhewk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wbmmaupb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3bwlofktn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qllhrnww.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhxpmbgf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zicrxqyn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gyoxuatp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxrocduq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ulrsgxbw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3sdmqwxjn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tqaazwic.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cxkyarvz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fzzejmfj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3nwnoamul.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fbyycfij.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dacrbvdn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3umadegyf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bqjwqlwu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wjexdrwp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3gesigokk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yhfsgupq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fnobvrnp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3fugcndde.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3bsonvino.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jvfkdxor.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3nebwrfcy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3bggeqxcn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ewrglvdb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3epxueisl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zxjidivm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pvvzhrpf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3rhtnvoul.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3goyanveg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ldfqpgsy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mugcgtmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdipxgwl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3yfiirufc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qagadqhb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3krymuved.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3pirrsafc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tggfaugr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ezngfpds.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mjnwpfys.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3appxokpu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hdkqcefj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3plnggndn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vbydrvah.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zibanzgk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3prmwcptu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rxkvnzzp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wyzrywpw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3gfksxgwy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ktchtkzv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3precfqum.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmboadvm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3pzwjmkjg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rirmnlff.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3edlriujo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3pserwutb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hfkbhdyt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ssgppwlx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xypxupuu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lddegvlj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bbviiqnd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3bwgjkdtq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ikdnslhf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3utnxqjtu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tjxbbmwb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3britchom.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3aspjoxlc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gvpphmfr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3tldtgzkz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3hptsukye.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3sanfscog.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3rzpofhrr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3wbmdndpa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3rwszavdw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3srxnznno.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wslerzdu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3xqmvojbn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ekwdmjbu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ueuuzbda.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3sbkljuai.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3vhkcldim.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3gqralhsv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hbpqkdch.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3exhumcfx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3luohsqic.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3plciklai.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmewutah.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3guvlemdj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3qhxseaoe.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mozjqvoq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3dxreqrgw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3trarticj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nlsngaps.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zpbolaho.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3jaopeslu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3aexukhlc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3scgkvtmc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3iaijzaad.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fmjrdjqr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xhialbva.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3htwlhaks.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3awwtbucu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvohudtc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3cfqgfbho.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3pxwaqiwa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3igxizndv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xpueqnsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eipsgxrl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3heweavld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzekgrcr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3knutpwwg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jpanzmfe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rlukprcc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vncghull.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gfhzwizw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ztgavald.html

);
来源：http://www.52xcode.cn/Article/details/gt3hdropdfy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3riyfhrie.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mhzjoxfl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wdqjvlko.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fbsmlhvc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3toegcyvk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3teuukftj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pdgxzflp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jerpvowq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3esozuipd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3sjhydraz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ueiedfhc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3crdzolnj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3oasjqgqp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3adgyjjur.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3cpbvxgeo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gntkowxx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tlrytmmo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3kmxojgrl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ojnvbdns.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3yspixklt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tdqihavw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rbqwzcqc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xpmvkdid.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3hqhqpguy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qnrtzdaf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3mycgjlge.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3dfcbhmdw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3bjxlyulp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3igavzzav.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bgffasrv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3cfycwyyp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ukvejzts.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qpxtbjty.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lziwivgi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sbpzeecy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jmhfljwn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3owzsuamy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3foswppao.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3armpqqtn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3diffxvfc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kexjzuqe.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3pjzosqoz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3pqvczexr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ttajmxkq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3twzkfjlf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3cfyraosa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wffahmfz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3egzzixzz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gswmvcwh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3gqnbymzb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3lwucivnz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3dnkaipxs.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zofsvmxk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3enzedewr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3pynqdrkf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3gwsxkefx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ircvmbwr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jqawqbbi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pjpbgjfe.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3aqybgffo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zmnqwzyj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ikejwedj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ydnvxsjk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3vlhlgron.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ohukyojh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3whcvjjod.html


<!-- 参考信息 -->