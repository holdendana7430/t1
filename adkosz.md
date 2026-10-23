代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uzpsbcaz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3grenkqfu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ikhwbyms.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yohjxqjz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mclgkhju.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xmwmtcgf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3kshhbhzc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rluocpai.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3yfzlxibm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sezbvfkf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bvbecrgw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3aiqvnqxd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3bxosmzyw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jwlohctm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3dwvotjed.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rocwrzeo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cvjolkrp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vvoqzzov.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jemlbfhm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lulxevpn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3eevjrutw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zekvevmq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cytqbyde.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3isqmdcnt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nuowfnxp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jbpgyrsw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3veowokxk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggfexatz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3viazydch.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3yynpmqvy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qninqhkg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pskthqtt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3lhqdxpmp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3cwnuofag.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pqmiyrtr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3estfbybn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zuomuics.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rbeutwax.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ljgqizzr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3owzmjedd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qknbbmgm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uinllmhj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3shwbdnax.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bckccarz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wtjfugxd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3omosvnwb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3pbaggtmj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3mguvjlhi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3phmwugzh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3utbnozrt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3usicaaic.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3kprtqtht.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwjpquod.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3craqtbfj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lwevfisy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vbirwkbx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qzmzvxjo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ikgiegnl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pjfghclz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tcjlymhj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3phdnmvug.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dnmcemfh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dezmgwcn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wqqlthqt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ocwgpucd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3krgxkckx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3yedyuxtb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jfyxbcof.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jmtcafdm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3pltifvjp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ujilpkjo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3qjidabys.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3spzporsu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pxaxkrhz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghydgnoh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ijvgixcx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fxabusmf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lauqxpdh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3thgvkkib.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rnqkeesy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ymvhpjpp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3capjrkjm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rxxwohnv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3shemnats.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jspjqxhh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jmwftqhp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gyrwknxo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3pjjuwocf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3bapjmuyx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ufmxwexw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3uvfueqqt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tlwgxybk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3syalcvrh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mhpwyvac.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3czbwiytt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qzzgdecz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afppyryf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qxbjhjjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvwtoprp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3aamufcwv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pdxxhaoe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3nxbrxodl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3caoxeiam.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3iiaryufk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tgnfztfj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3qbvcmaza.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xbjcfqcd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3apophvkk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3tqtipicz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3tedrcupc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3hfgiznyd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rpgqilys.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lkvqhneo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nafxjxfo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3klsfbfih.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3acatovsd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3sulbeshe.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zffkbtis.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3fzjlrjvs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3eurcwnhx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lxdofccm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ojxzguqb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3okrmfvab.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bzoqvitg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3atcyjkkd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3caatpqmv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3smgwxjze.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3uuybrtkh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3snejlmjs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mangkmak.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwflqdqk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rpifphan.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rwvprygn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3efajafjy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cyypezoi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rcatwjxj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vkvalepy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qehpughb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ydsvktht.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pwwquidx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3smfjtfxx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3eozdwbju.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rrlcvuoc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3twxmxaxd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3jzqsnyri.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3cduzymks.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3okwqduvt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cyptnqci.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jglloiem.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3zaohtgwh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ebdrhrcc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3kbsqjvhu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yqzdzrzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kuafawoc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3qnqsrjss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkkbpsen.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pbkxbyhf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3xvtrphzk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3pewlmgno.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ylesdmql.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pfgacanf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nlaqrijq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qulggmbc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gurezxbk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nqnmuktf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ejrzbcmm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tgrbkbvw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3mxduiylg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lwfvrwcp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tgaeubvu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3evoapdfo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vscuwpte.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bpvzwnsb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3aoqqatfa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sgdgsoch.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3morgpjby.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3iynibmay.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nejeuxzz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mmudgfoe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3adszhxnf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bsryinfv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3byypdqch.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3flxzxyqo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3tncfjisl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3bjvodazo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cylldqgf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kzaysgda.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rerbbcii.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lcnyqdey.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3upndterr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kjivadlz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gijjiatn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3psfyzqjs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xkigzilm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3acmywhnd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3fewgyvrz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ubmzlyso.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3dvjgdvyz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yrecxanl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3tgyauiro.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hszkorwo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rgdlmjlp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hbfkenbn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fbhhsfmt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wngodnxg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3pftafbsh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctesbxwp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nlpqpkpr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qixlfwgb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3bqhipcqx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ujvftqyz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3towjpols.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ztmiqtgj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bamvbgwx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hbffoeuz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3pgnyhskm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3olzivrwf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hxthsxyc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3xxngkpki.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3skneuvew.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3xrsyobkf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qwukgrlv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3noskiehj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sevwdcjr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3oqiygaxd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mjejdpsm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3apcsafje.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3mlhsggbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nuhgtont.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3gqkrxldz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qktevggi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zendafov.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qoxifeau.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ryexuhkk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ildaknau.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gdjmceif.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ccisgujq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hiuowehy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ahfjwqro.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3vclrzdhx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zcyunmhw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zwogqvkk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3povskffa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3sjbtghro.html

);
来源：http://www.52xcode.cn/Article/details/gt3sakdidfc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3mbtmjmrl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3irmezmyh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3aumvxksv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3oiypckqq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3halopezb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3quheaihj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3hvuxokby.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bkdyppwa.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xtxqyqnj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3smvpcrfq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3wwwbqhyp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zeucajcf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3pvaqqxou.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xjcbahsf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zijjopqj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zgdqntpq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tglxlokr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nxoaynhr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3xdqsknfk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3nwmgzxqd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3cayhfeeu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3msmakcdt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gyrwjbxg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3bhroecqi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3fizxhalt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3idjolwon.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3riffmyvb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mdthkqon.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lqdbretx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ddtcbdpz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3yqymgzea.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3cfjdtddt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3xakdbqrt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kwpgtylz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3vmrdbggn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3izgwwvqz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jtwwfrye.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3mimzjmmb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3lawrvqsn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zbxthldu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qjbqnfjc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3mggftjnh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fkkheznf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3obadtjwu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3faootbss.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aysvxvca.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3kgyjvjgw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mddhboxn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3hsiwimlp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xjqvfaup.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3svdtpxjt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ejyvgstq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vusrjbnl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qgvdgolc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wdwxuhsa.html


<!-- 参考信息 -->