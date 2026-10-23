代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kbuquvdk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zpyaxphx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3laggwmnu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xrlfpplh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3brsasszr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sflhywft.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hccxbqco.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jskusped.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdzrwpsg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tyonoasg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3nncrubhq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3mgulhurj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kgudntod.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qpgauasp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cdhdvifp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3miemcjkp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ufuiodkb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3colvhwqw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ngyiljwo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3oxffzmkk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zwberovm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uowbihic.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jwdqoujx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ccnvqzgd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3catiswyg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3yzbupwai.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3skkklesj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3kakegbhu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tdgtzqan.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3sbphfpvl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qrcoeers.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hkmknmwc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fhqkkgqp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3hcaewcgx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cmtbfuzv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nwvsbtxj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fowldico.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xkdigfai.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uawqtmbc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wsemphrd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3iewpihfj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3gyaqyyjb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fpasdyno.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mmwsgdlz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ftcxsfeb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vsbtaatj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3igkpqwkw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3iyndpsnt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wqvifrnm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qowherat.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3thalggqi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3cetqkiep.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tsxawvep.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cilbridm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zkhneklv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3shnwhnug.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3blcizvpd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3elcfvdqg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3shkboxam.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3aouhhsnl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jvbiroem.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nzrsicet.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lrmchgxk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bmllvaex.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dsptyybn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3yidnbxra.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3auuwznis.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ogcwdmuq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hbjzbpgr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3cdaqrwhk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dzgwppqr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xcyvwyyf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ocsoykbq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3caopytwj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ryxpqrda.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3viwmcjje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ogwlnjiy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xuneecgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnqqhrxl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hftmvqdu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qoyopbin.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ynkklrzx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3zxulxgks.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3legivsqk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qaepwcpi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3dmkwqjxb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3vwizkjvn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3rmkecsuw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cvzcepgu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3jvkwxhre.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3djnnoxrh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gdbgjflv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jkxagknk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3eolcofba.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3kabavrpc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3bsinreij.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3pbynvtcs.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3grnbvkyk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mxqqxlsr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3fahyrlpi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vurbtpfe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zqrgziim.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oljnjhat.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pphcwovy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qbbvqmte.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qigmaraa.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xoaapdxn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3wpbimusa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wjbvgfrm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwkmlqdb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlwutgqf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ngocdaei.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3zbabsbzr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rhjzoqvq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3sqtcezmv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3oguaskdf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ldnbjhpu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jbxgbvmr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3sxhdtmjh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zvujwymx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3movsvvlk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zmsaevkl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3euovvfiw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3mnfnhniq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yrjwwrbt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3fvfqirlg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xcowctyq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mfcfzfez.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qglwmdni.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3iayxzxor.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3nesoqhby.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3syvrupku.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3hubunmkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnhfnqdk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3aktnypze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzivbtmv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pxgcmald.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3yamtglhr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dvygcrhv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3daqlipye.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3udhgcqkc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3khttcnhm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gyyzowji.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rhjfwhym.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3yoxytutb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3tykrjwqj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3crsjzjjb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hwpksmov.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3yzfexkwl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3rabvvapz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3crodomgr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3kbzghxpr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uxljafst.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3fwblrzcu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3xatmmphb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kkgezvjc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gnouaclj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xdyobjoq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zqvjuakm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3zhvoclaj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3cdevekuk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3hebhqmnp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mtehhtzf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3pzzmfajw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ejeqozsn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3erspvmld.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cvkrqxyi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ufsyshwy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vjnbyhmu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3cymnrdca.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ofqgefyf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fkouqjoi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3rlowqczr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nfwqcfhv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3quwdtmzd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wupiczjk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gfgvaqkp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bgutmbuz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bgvpuhzg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3unfugaxz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hqfcitzz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3dgznellp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3xnveyzgj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hpoxmiwk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fdrkever.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxjeamsu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfehqcyu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbdkpwqc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3fcebjnvm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3yqkfmlih.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3rjikgfpf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3bssbphfe.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3utilrsuh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xhfddtxt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dwxybwgd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wukwcvgl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3grvwxkrr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jgiqsomm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3olecvjzp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gercvtyl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3dxwcrqdy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tfprhyaq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3xrufludc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sfnmutcg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3pofpqtbe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3woetmiwv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ducdyusl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gankscib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xjfckddh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lgzzpdsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmwtdcdk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yyyfspuk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3pkeohfeg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3avmtpojv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3exifjniu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vqflkjsa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3uskbuhcg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pmraffls.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3lipjxwon.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mczyndrk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3brdrjcej.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3digjkspa.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3owvkqzml.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gvrabskb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pbznfunc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jgkugdxp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zjsefima.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bsxdyjqo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lgspmhnu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3bxnvgtyl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3wfqmhyep.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3qenxslqi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3npyeuqxw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3uzsjxugj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ynaltjlr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jyvkqaza.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3oafoyvwg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ymfkhrkl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fijiuaic.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3tffdqehy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rbdmmcsm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bvxzuevm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3etiaqsno.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vpoysalp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3eqcqhowc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3mlmxonrx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3lcryekaf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3taciflak.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3fxytmaoh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3asxumfcd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3njkmjfww.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ibyduuxa.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tesrxity.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3yrhwdouh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nvrjchcx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zmafdktq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wgxxluer.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wodzauoi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3gmmapmwu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zhptvkke.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jfublvbt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3oquoqfdk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ixazfuxm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3knlpnbua.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3atkzlifg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3fjuoaiwx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3sdknuwvj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3dpezqegd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3oazteazi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3srkadygt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fovptphc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lpvoszhz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3eifugwjf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3dejwolai.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fxtnlmot.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3onhwcoqn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xyryrzse.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3nqlgbplv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3josdwjqi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xwwtakzb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3becuoapo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pkhxixfl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3awnfsziv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ngiogwum.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3jzaumlhi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3evotiulc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eidgmuki.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xrmaralh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3oiamtjpo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qjzdbuzj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3yowvblsf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3mkbnetfy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3yvdzaomw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wcisxrac.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3dhnmubcy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hcurkbgt.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3zlmeeoro.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ilbdiujk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vwngqbzs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3vgvteswe.html


<!-- 参考信息 -->