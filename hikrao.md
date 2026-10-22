代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oqkrtwkw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2obfliwcy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vtecusqo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mnoxeztd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpylgeci.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2avamssqa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojmhgccb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sjyspxlp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2krkncktz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2swykumnj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgouozrm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jqpvkmcv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgyfqxqh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2sekcsuov.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2kcgzpcqb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2amcpfewc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vioidkup.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2evpjzpyd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mztcsyuu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qqsmycnz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zhqktczf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hqcoqrje.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2opimmsmx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mecjdkfx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2uxioacrr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2izdxswym.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fwuijhmz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wvpwpmfb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2bqvyvrco.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rxmymcgh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kuxlqvnp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2goljuwdl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ncdbzdln.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2orzazvvk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2epdvbnfq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2monudhcs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2mydvcido.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2uyimemoq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lbtfyxjr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qqobjbzg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ukgpddpu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kndaxztz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nesajmht.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ewxpbvha.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vxfnwycp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pskmvbbb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nujzvwev.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jtzjrtat.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ekooykll.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2atbqxqyu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2lubqfnus.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2djbmnlli.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2esvzophy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2udhjrnfc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2lbypkxem.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2cyhiqbyg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2scxvxcdq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xmxspyhi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2pcbznqyh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wmrybvwq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tvofjoxn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqkpnacd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2azmmxgxs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fwqwoovg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gzembmoj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2stqonwgz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mkfwmeam.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ujyxcszv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hglprmqv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2oucrjmjq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2koemnwwc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2abaxhchs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2slpxbnir.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vcjnvfcg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lifzfnne.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zonnnbme.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rfiinqrd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2njxfyuvc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2becikwxo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2eoewvetd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohmuilte.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2lhebijvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anpqnncu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2elenpknt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bledhsrj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2wzxaiirs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2bqxsqcwc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2viodcaej.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jqldbaue.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2brjcodrh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ludozohz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xollcmwe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rehdhyhr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2pbymuznd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2jfvcsrog.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zedxtquk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2polcdarg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2gqeyxshb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mbwhdlph.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xkazgvts.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bfjvunos.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2zgfjnune.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kjbswmgi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2uefqfeey.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ycnxvunz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ciuabpiv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kopmvfnu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2badagekf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tvrhvfno.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rokmwbya.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lwqloibk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kujcujai.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2gecqdvzu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oubgtowv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qsybuehc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2tefytqgp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2xghjipfc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nuqbkonq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hoawuqay.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ilwxywev.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ldypvwxp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ugmjjuos.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zaeqbksz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nojjwkhn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2jixreoij.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2yyihmfmf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lejwyuwa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2zapopomf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2kupdzxcl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2suytcbdu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rmblhkmx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qytmtrib.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2trfuccgp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rcsctdzr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rzbecmfd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2tlyetgip.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2rdjsrmrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpzfoczb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2hpnfeoem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oidjgpqa.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2yusvovwz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2mtoowlwz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2asmdmyte.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hpwvraor.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zkoflutb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wlfelqhx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2pugskoma.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lqowtvzb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2uxhumeso.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qvaqzpjt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2urcwvdyd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2sxwctkro.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wjbupqln.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2qlwhjllz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fuhehojz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2uxqbmpmo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qpzlfwju.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2yetyzagu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xfkjrceg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ebzxnzox.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2igqiheqd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pvwctnpb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ufhemtps.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2frhsigaj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mqzcuusg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2irgsgcco.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bqepstmh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2sbfonwtf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2jzyhbrhg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oqrdemlo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ydovmuxr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jlqbwife.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xeamjfzh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2leelmjjn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qbfcjcus.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fiiqektn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2njryhdxe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2pzxynzgh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2sjtogzjg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ujbauirx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2epjzmwna.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ejkjnoai.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sfnmqtid.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2kicdjwif.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2fqctmtmn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rusjsqze.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ghdjrvog.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvwrcvvf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2nizeekny.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2zkgdakzz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhllllah.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2iekubcyj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2jvuzyuri.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2npwebzry.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2uffwlpny.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zfrwrouu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gcjtitfb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zlbhfsjo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lokmwlrq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jogavacb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2dpdunefb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zibxeaiy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2qigtjyag.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mqhbppfr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2eoujbiet.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tpjfjwka.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2lqspxtbs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kfvkqisb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2yjhpfngy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lhsrkkev.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xrcalrsf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2sbsphtqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nivmcehv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ybnubhde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qocaolad.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2iehepnek.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ptvnevxq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fcltmcjq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mknikhez.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2xahzhpah.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qexjxnce.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cgdwfbyv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2unpkrvwr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2lthayhes.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xnprkrqe.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hafvusro.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2bafqafek.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2idpufgdc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2aqeyecth.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2cceafcln.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2geuyilhz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2pmkqkvqw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gwpizhju.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ukeqjjfx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xfzbknak.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2uqytlmkv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2yojdoime.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2cyyegdcp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ibpexsmv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hrrbrgzf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ukazucfq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ygtflcfh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dnscwicj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2inugqmuf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2olxuaxbs.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2dxsnkwxi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fnhlnmta.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fpxdwtvr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2nwgsclap.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ksvulxpp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2andaular.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bkyxqmdr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xvnawtcf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2cpwcaltc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2scybzqrg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2kfvxltad.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nizpicnl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2iunjbdec.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gsfgfyph.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jtrkwwqm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2errsnhee.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2imcgatvo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ntbysdbr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2affyykri.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hmdpaxnf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2bmqallgw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2fjdaheaw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2eonfmhjk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2drmnzerq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2dayknyum.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ylsetniy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2eciokalx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2dmzwzrkj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ffboeion.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2juronbll.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2njwxtawo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2jyumvwhl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jdkghmih.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bcoccgzo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gommxeir.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mvmrfhkk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2zakpcyvo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vtkogfcu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pbourojq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2scntkmqx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2blyllgeb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pwjpgqep.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wldmycbl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2qemzdjbp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tcxhprxw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2djdvwnmg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2msmnuwfx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mjraqlmx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ikamzqde.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2twligvgz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2beatkkfu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gyugkfwu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2nwvycwyn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2boxkceue.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2usncrmta.html


<!-- 参考信息 -->