代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxmvxsos.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bvkazttg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zryxdapa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wrusywtm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3boqxxksz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mrgdvpjm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xexzsjrd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pfyymxvx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3blcvbjqh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cunjxxwz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3iksrrqhs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcmwpswz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtjtgupm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3jyplshor.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3pyftkejp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3pqrybngz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3oheiesra.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rokyxfta.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gshdaaxr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jmbhksja.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3quvtuivz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pdwixmzu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nolrfrsb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xjvyjxtw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qkhujvrb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qkfgbnxq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3srxfenfi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3nogfatzi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3renfwgfq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3rmntkrzp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3spfwcyst.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qaxckdsk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3klxlgdsz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3lwayhgoj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3fmvgbmgg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kfzrcywl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3mvkunotu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kiovpzph.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ksdjxtfo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eahjesfl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3osllobnz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3obikaabv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fadyuczv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oyhogbnl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gahnoyyd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rlodspbj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hfybjzha.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xqnafekd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bqizdcal.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wjimzoxj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3fvpggnsl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ozjfvsqz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3duzriadm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lupwlkag.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3kgnksihk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ejvfwspl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ddwonfnn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3zhfhxvpt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbxxdpqd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ugeqqslf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ptuvptrc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3yyhoskqb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uggkvaxn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3olpaigxb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3meuctlad.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sevxqmiq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3stprypzc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vfrbflrp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cfmhhzsl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fddiuuxt.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fglyxvzc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3howqnfik.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rlhxtsst.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3eqqhesmo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nnvvhpcp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vbevpvfi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xqkhdauw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yljbmyri.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3yhgkozeb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mcyxrkdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izxxfgsd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ziyhlvrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wuvobcai.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bgttgsuk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3omvqqjkl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mmbojctg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3egxezzje.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uvbimnps.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vwlxrccu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fgribftf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ttgtsbvb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3pmbfmcvo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3nhhrcevb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dnbvghxy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3doxyhhxq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3otyjrwnv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mhrdcqxt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dolpezij.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ybuvhipt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fibayjdj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3itypurph.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3gmqcqnxr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3uonyogcq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wawuqbjf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vtpwrbac.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yhnyezbs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3baywvzba.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qbftaqac.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xpmvobow.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3djdutjqi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sbehxvom.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wzedidpw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xbihcyex.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3oimzitqv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnvhilak.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qedbeopb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3mmdsdfcd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xcybwdnb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3svvclzvg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3yrupzghr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cuspsbqb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hjnwnxcx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iadnrhlu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3umnozalt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vbaefanj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hjntrcob.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3exdsphee.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3kycdeqfl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3afmeqzit.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3dxclsmhf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dgdxzjpu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nqknixsc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3krzmmpqo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3zfcpohrl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3fcyyazxw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3fcgtmszg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3beszzkzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhjcrjyk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3sfvsewrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odxrleba.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fnarppvn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zivppnme.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3eakcodfw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dhmtxblf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3anadllgq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3donbvznx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tbpjxdvk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3axrlhnea.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3eoigmlcn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ilskkuoc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3eueaswgh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3hrnxxfkg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qpzhmmre.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3cdiqzhel.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3djhzyvby.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3smpmqefv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ryxvztiv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3whqcxsfy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fscpuqor.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3bjgiouwu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ypmviwyw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fgyopsqm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3smytzlqj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fktyppzc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hlchccfl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3lnwzlbct.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fylnfipr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3mjzptsps.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3vererwko.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3abbrsepf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hccthvfo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ghzdvjpi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3frgnpmnb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vgsjdmfk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vxnisksi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3khsuqyis.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3pfgqkirk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kyhriudn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3panejpys.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3agmafgrl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3knvlcrdl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3igamtuft.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xecypcll.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hfskcaej.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vdriucmw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rwwyhswv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ykemlgbv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ndtpqdvr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3snbevpxc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3tycurmis.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frwusuqe.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ayojjdzk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vninyaki.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3auuuezks.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3bfkijmjy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3tuqebinw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3cvcduvrr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sxyuvjes.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3iqbiueya.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwecmmlt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dsnqmpwr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3iivauleu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3fgghnsle.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3cagneiht.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3cclthtjg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3fmoulhjb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3usuwgpde.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bywmetkg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3cyfaajyt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3pskodlnh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3pkvmybcw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3novyayvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhzzogct.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cqhwfluk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyupzalc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xolbuejb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3slhbliwx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wqhribyg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3veugnsjd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3khaeqlxh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3eyhbencv.html

);
来源：http://www.52xcode.cn/Article/details/gt3qpytagma.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qffjsfjm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3qqetcfxr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bvbtbboj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3blccmtos.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3lyxjodlm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3twkpprfa.html

);
来源：http://www.52xcode.cn/Article/details/gt3hnjbfvao.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3lhjyvrxy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hkdvynug.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ntxonlum.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3aydlswny.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3riperqsj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3gmzlwyjv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3sfqkjxcx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cprzsfph.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gyjvdhdb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ewhewzbi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3esjrlifj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hqcvczth.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3jqrcgrww.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3khqhjjro.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3aqbmlevo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wmfkglzx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3srtwwpjf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kbaxmbso.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ugwneyvo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3iipboyiu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xhorhnml.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3nrgttwuc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zrxhtuce.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3xdqkmdpq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jjdugsvb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3oxvnuxbb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qkaxqgsa.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gemnswel.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3iekemipx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xmdnqsde.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3kvirupyl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3bderqnqu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3duuvkiew.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3karmkkrg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3elavhlyv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3wcfrezle.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3qvadwqpd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vbprtpms.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3cmrqpekn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3zumolkqk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3lfmqhszu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3sebvyvqf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3iatafyvy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3sxqdsafm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pfdhpxzo.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jgvudoqa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3iitbkeaa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3dnhjzbrn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3vqjdsrhb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ijhxcenu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3abcbxdjl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dnquplrd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3biuzwawy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nhezetkt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dfljdylb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tjdwrnud.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3rkjicqgv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pcslafhj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vrawaicx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nymtqzbz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xhohmvmg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rvxdgnci.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3vxcvyfpt.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3bwadrfmi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ciommrhb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jqqqscii.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zgbovecp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3krnssylv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3iagsqhxb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3zuynpbku.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kxtisuyg.html


<!-- 参考信息 -->