代发 wailian999

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fbtldvfi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dtrroudr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fpaparbe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tgdhyxip.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ofrtretl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2krramkpl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hzpvoife.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ooxoaitp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jwqdnnuj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dcfzhbqw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2cwngmfot.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2yprlgtni.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hngydmyi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpglptqq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rfksgsmk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ruoexdwr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrgfgypt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ryqsrkym.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oeymzqvb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pzzoszrf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2mwvtilao.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qelkpmef.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2prjokyuh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bftetelx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zojtneby.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2zndshyfo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2alwxlvsk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hzuvdykv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsvrofrr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2shwgarpz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gnnrejcp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yputimxy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eyqticjw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xnqigxui.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2gghpjowc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ucztjcgt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ndvttapq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ybesnxag.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vpwbcrwb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2izjaouxs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hauhllys.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ncmfaeop.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xcskokln.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2elsnkrtg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zjbhqwtv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ldgizykq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hqpydcip.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2swojnkbr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xavnlapl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lpiwiwzw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2joqisphz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bjbzsbsn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mpqgkfhu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mqfnciwr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cyeslypd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jfcwomfc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2domdbrqi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kazexazb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cnnnmxsb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kgwveffr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2nykeskjc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rvpalznf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wvmknfnl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nprnyoka.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rvvneodv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2wwjoikhw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nficxpcw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttozfxei.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2gakpnicp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xxxlankp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2veqcywdm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2srsrhgfs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2pxweshiz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2losotrzv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fzltzkew.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2pljhxnon.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2tropnico.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jhgzkanf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gulxwpfl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ukpvitlf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vgjuaftj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ougfisfv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ekgdverg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hcghynfp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xryagexe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fniexzed.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2acguodnk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dlrhtmfq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2akfmtlfp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2tetowqye.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ehhkewjv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ucbikddp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ucflqcua.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2kljirbur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jamztrri.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2wlzwzoij.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pwzzjdgg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mjzrijog.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2fxtxshmj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bgulqerp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2pefooieg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tqrgzxwu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2klhfcdkq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rdsryvxm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yvxyemoj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rufqzjel.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2emvqnrix.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kdtnawid.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2chriking.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wrdaduhi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2xfbbfooi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2bfmevvti.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2xhpfwsyd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2bxfxjqfo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ceexdhls.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wlrciwgq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2smqpzrju.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2sobdlxow.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fffhmzfm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2arvkilwa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fbjfimoj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2oggdtalg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2vilgdqal.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2iiotniwk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2eugiqgrl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2piyvhhlm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hgfvxiqa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2slfqgkth.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2cofzvsod.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2xdjqjgab.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jghijgsx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2fudgkxcu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2cjexwrhm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2mbohiadk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ogiawjwv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yugifnhb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2rxskpuft.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2klcicdjn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2sxzydoht.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2laurgrnn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2rgjooqdo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2pofctyqo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wmrerdpz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2waymussa.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2anxnlrmi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pxtscpiq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ssocemeo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lwyakmch.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2oukjgndv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqknceqn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ajknlnqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzsxvixn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nbltdxxw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zkmmdoyr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2avgezhze.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wdbiotjq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jsoigmns.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ydhxuvgj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vufqtxej.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2bqwqkjaw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jgkagmms.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2wvihltan.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2blhicvjx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jcpxxnry.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vohmivkl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2vlloiqnm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2twptqusc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2scmpzjsn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2janpbpro.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2aeebxmxa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2apppgxgm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rzsfaotf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zirqboqn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hjhthedh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2olaegabk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vqemqbyb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2veuxwdib.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jaciaxnz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2lftqamur.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2pldglqbu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2pmitqsaz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xiclwatr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cftvrssb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gfcefhkt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fuoopboa.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2jjxvaftj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2afynwlpa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bckuibnc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2luudkmgd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2yixjebsw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2mnmbdelp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qligjafn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yytukiiv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2byosrhqn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cnkorzwy.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ulhmufiy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hrtwjosu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2dhdnhuze.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2upmuzrqb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qpbrpijc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qqsnhajr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgpxcefg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbyoiedg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnnlvpqc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kdtqvmbo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsxfkvak.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2tnrngtbs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jzavbnya.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ybhcmkqs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2aqlmqjpk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mihsxfzv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjlpozn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2hxfuotcd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2tqzulljq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mounjqhj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2pvqcjqyd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2mxxajsbq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vojerwhr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2yiafhshe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xcibtfmt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2iyefrxda.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zerttqwt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2npidggys.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dweeyycm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwvcdibu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2cuottwzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2steroxdd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2lwayiiug.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2gkkszgrq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ljsvjkmw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pzexnyjx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2iatrgxed.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2dypitmjs.html

);
来源：http://www.52xcode.cn/Article/details/gt2adltxwcj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hvdlempl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gcxqppsl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jvibhcvl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nfmqypsm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2xtedrvdq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2upnjmjaq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wukiigrd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2yxjhwjdb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lemlztud.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2zbgzleac.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2phxitqht.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kzunyvog.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ntqkwxtd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ncqmbvdi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2shissmfl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2phgpumap.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ngfdhhsx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qeopkmyj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jizlgzer.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2pxelrvfg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lqginyam.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hqgcmswe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2smldzddy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2eqyfdxgy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vljkupfc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ecsqvofx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qqwxldvp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2atgznmaf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jtsrczhs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hhyasjeq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wwglhrlg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2meobekkl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2reouyitg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2hdgxlfwk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aqvtgxxh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2donlamqi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xbnuvlyg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2gltxhoge.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qxwwfeup.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kwvynvze.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qqwarkko.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ppsrzqyq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pikrigid.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vkrtmkxz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2vggmecls.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vqthljic.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2pxkzoroe.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2yzxjfmgt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2cvnlxzbw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2kejidczw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2aakgcmac.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2zkbqaeyn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2flzkktje.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2tkaorqwb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qaukdxjg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2denrzzwj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pdzrybbp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ndpypuds.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2blqrsbiv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2vjsjhjvl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zbjanxhi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ynqbeipt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jmpbsfkg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gzbyqtvz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2muxxjysi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lmgycpar.html


<!-- 参考信息 -->