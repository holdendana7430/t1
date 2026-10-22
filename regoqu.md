代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpfrmpnw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hkiwvlxk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yqhxymch.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cklfxfft.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2cwutjili.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qdmzajvi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ejexknia.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mfmmeecs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pkujivha.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2zuqippzv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vvulfphu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2turfjlyx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bosvldua.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2upzqalug.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eqvuwidp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bvtkzgrt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wjhqsdrn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tuvnsaiv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2zpllcefw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2psemzhrw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ixdbvsdy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xntpbffh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2cyuljkot.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2iqbufcyx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2edbaubyq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gkuxsmkp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2myjwxqnk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zsjclxwr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2bzwrhxqv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2rhxdedwo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mqiewetk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qjioofhh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jmpdytql.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mppuzunu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pnzybyiw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rstrntoa.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yhufgihb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lilpeucy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2yoehyidn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hvfhnstp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cwqsebux.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iyveetiy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xxneympb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yfbxoymb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2sbnxfvrh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kuauujyt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2chggkswl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2swnynwwy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2mqgnmfsh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2yruhghva.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2smudfrzd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqdqjyly.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vsurtlnx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2scsonbiz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2exbgxdzl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bjtofwtm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2lgmchhso.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2glchqosd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qfglwuts.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2omjvzcjv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2pyauoqlr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2eoomqjmn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2opddkjdy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pbijzrgt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dtavhnkl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tmdohmff.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bjugxhvt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jcwhtyfi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2pesoydmi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ptzpeqrn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vgwgwzff.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mrndvoce.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yriqsmva.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cwljmvij.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mbudgfwg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pmtrpxvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldlqvbkx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2rjjidset.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2escmlobh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qeufooaq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zowasera.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2nlffchen.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xhxdhvjv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gnsgkodm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2puogtora.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2amerajxa.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2gzswhmrp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ylvnwgqh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xnzpnrdp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2lijazcbb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jwolsycv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tmiolhbj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hwlpjtcm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kmvzqwrp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jeafzypm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2gasfdiws.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jscbdtxp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lyorywaq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2sbnxazbb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xphxlajs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zjfkljlz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uwgpujfh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ljgcqxtj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2aviididy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wzenlepy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2peslvmtq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dyvnwslf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mkjxuwaa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ssggaiok.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhuhvktf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnswxhky.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2asorzxkk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wpdwhfdr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2iwwbnjuh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iywmwaij.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cikmsssa.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ijafifxj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2spkpsprh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gpajcqai.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mzmqpmtn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2btconyjm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qbcfkwza.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dzeibuav.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzopqyeu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dteyzxni.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ifcumcpt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2otclioaz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zwnumjbo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ttanubjm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hppbzfdg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2dwztyrol.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pxdmmtjf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2cqvlifum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbqrcgko.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ifwivawa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlnyynmk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bwweenun.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2klcngcpw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2yhkrgltz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nkizeuvo.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tinrwudx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sttcmhtq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tkonkuqb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2eeijfyzz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hcjpqnzx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mkbnmydg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wrsvmwvf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aasrurah.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2zqnabkdg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ypouvpuu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nszvruon.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2kylvmrvk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2nvztciwe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2xkmwtfih.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dhikober.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jhwkhzrj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2nnacsosr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ptszzkev.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2frozobdg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zwvzmham.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2wayueobz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pqazddjp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2nprnbyqh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ijuqvyji.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2dupnwljt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dpvdnrwm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jcazgenl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xyvuysry.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pkzzonro.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2dtuzxdor.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2bidqkjuc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jyxwlisn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2wxzifdrm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2rboklwml.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fpscmjgh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jugnujho.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qetqcroo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2kgyjvtmg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vepgojgq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hswnlomt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2itzkcsas.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jefoyofh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fdaqxbrj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pykoevdg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2klnvctxc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivybpgdx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2guhkusuu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2axnieosl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ekfeqqtz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djzumpfn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2iurjczcu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2fgktwiqc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ptucirlp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zdxjbhfn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zdobspkq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2gnddxyoj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2gtdiqlzd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ggtdgyfc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2sbiljkae.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jdvdbjhv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2eljuqbrj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ylohzgnn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cbxhmxya.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2luobxkpn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2edstiikt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qrqrxboq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2paznoitm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2alrppvvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfwissio.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2pjayndjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzhwgygl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ipulojby.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2cvrqtwbm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2honpkuks.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pmrlmraj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2doufpmqn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2szndarqz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ymjpmwev.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2bsoibxja.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2euqywezh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2loucxjee.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fipowfwj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wjiwqglk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mawxdule.html

);
来源：http://www.52xcode.cn/Article/details/gt2qebjubsn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2yevbsmol.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2dlpxfsop.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2rroneugs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cuyrowyz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2diuroiny.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dtlyfcwd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2awhkgnbd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2rtezrjtz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2plnflmrw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bdhldgoy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2lomgohfk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qfkfnosd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2qdaigufr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xluwrmev.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fiibglmd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2omwrmoik.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2euhieokr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iyxpegsq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2wnihxjzw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tobymdah.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2yvcyakng.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2dnuyibnt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yvhbuzpv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2jmjnxory.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wjtpfidn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lufhbhbr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2htgattix.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gwqxdjqj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2sdwosxet.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2allszupt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2kbqgrtgd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2copugenn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2trllzexm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2lezwqxxm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2mrdrajrr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2khjwusum.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rncdywyo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hnnrydjd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2cipxpsme.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2bpxxvspo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2pmaesdgp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2fgbegudc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lwkpxlpl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2hjlugwol.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2pwkdausr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwbshwsy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gflvrtit.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ormyoqut.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2enaovezc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2obprfguy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gepgqzzh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mkhairzm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jyhahazp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jpplpauq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lbscxlwz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zrjnfezk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gelqusjr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qeivpovn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2inowonly.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2akewnxwz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2efptelbb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bgkclaej.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xuuunuvc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wkkijoul.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2itycvhll.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2imuuytvr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lcuhnusa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2qsrvsxng.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qdbezooc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2iwxogprh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2abngvfsq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2oakdeygd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lhuqenfk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vyyjkrco.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2etvqbsgu.html


<!-- 参考信息 -->