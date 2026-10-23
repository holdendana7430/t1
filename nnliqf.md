代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3epdupvzr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3guiccskc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3spynxxtv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3pgnnkidk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vlxrfurf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dzyjsewt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tjqhqjti.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mezsiujk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvselxwk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ppiejhus.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rikvoovd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ewwkrtjq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3smblsfme.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wowibblh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ycsbarfv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wwbuwprj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3stmobfkg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3regdyupv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ugabzmbx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvqhiubs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozxbzxus.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qshhdsop.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3varcwkwr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wfiqmqhz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3omafabyl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oegsbflf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3tuqqloct.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bkyudukj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gesjvzva.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mortzsvh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qjcxprxp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3sxicctqd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3kiztdklr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3rhghiwnp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3yemeocbf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3wjwrjggs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3uopqdaqy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3owcsgcjc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3shitwpti.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bqaotpgt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xvvvmftd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3frpauuyl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3obsxzmds.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yhuikrfz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3isimjybv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lajtpwsi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gkpeqozf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dpzznhjh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3giijybug.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3aasbvqfg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vfnqniql.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3afjtkixz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dsenxbxq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3iaosptbh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3qqomucar.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mizdlcrl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jrjxtluh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3guiaockz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3rmfpgdru.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3iphdntdt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ufvoitnv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3himpdurc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3okigeowj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ictuzymu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3kbxpuavd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zfaxlypw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ksybjlcl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xfezccrc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hbcvthqk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vdmmaxbj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dvqirzoa.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xhyouwvo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uwgmcomh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3wynikmpy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ngapykon.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3sjsnpxft.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gvjzsema.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3uzxuqxqn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3soikeqdx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jkfqdnoi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rbgsljgb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3onbcynwl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3geanabot.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vfuoytgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3votfcxeg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zoplagku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upuvdgpv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3akfkoymy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hzuzaaiu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3unsaaruq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3sesntbpt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xvezepba.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3szdxghhu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jvizujes.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3glprtxch.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3bsvqxqhb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mnmylthp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xodbgxfs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3myaivijc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eqkmdtmb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3potjfvld.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rzrnrnvm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bexdlehx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jyjqhowt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3tywzgqqe.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ascvpsnw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3yiznkefb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3oqgdgycp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kgaabqml.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xphyyhoi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gjirroat.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3iyzlenrh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3kavccdcc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jvuzulqa.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pmwoewfk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ddmcmhnr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ofiiudqa.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwgtjweh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3elmwwwlo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3fkkcwfyv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jmlswgzn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pqvikuff.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3dcnncucs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3esofwzyk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kgyxehap.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tcjcyvmf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hokvekra.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dwvsuwkg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3sdocttrt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vvxvyxbv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wdpjfixk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwfoplra.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3libxsegc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cboatkbs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ktjjndov.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xmyrwxza.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3oycmnbhu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uhpfusgm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3slnzagsm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3izctnnvc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3sjimjkmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbutawmd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3msomrnmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aovxinmp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gngzaxul.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3invzlhug.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ftaswyql.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dheyblih.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3apntrxoq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bctmzwmp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kklorlla.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mziafkgf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3udcpzecw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wqlevkvl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yyruntbo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mcbhycoi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3xzaejbwv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3covlnnjj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gyhjlptt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3yqdtncjz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3przuclpz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qpdkrsqb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ybmpunpq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3qhqtzhem.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3bsznspjm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hrrwkzdx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kimyrqsl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3eabksjry.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xarqatqo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kcgpmpta.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3utilljmi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3yqhfjrwa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3zrijvtgd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3igjwfdta.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fymqhgwm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kgaqblsp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jpbjlvqv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3izpifzos.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3vivhwxme.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3walttxdv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vnaxcaav.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3klldvich.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ffpwehvo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3xvnebzcx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ftergrbj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3nsxwnrjf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yqtvwvkh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jhitekcw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3zemgkzbv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mnsgflzt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vpniijol.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntfhkzen.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3bpjnqwcy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hceqrrul.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3eedqxovj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dutocsbt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ddaduqjd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mzvbgajh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3tnthjdju.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3wynzwilk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3tmzxzavj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rriqtgwq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3roztkeph.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjgotlpn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ujpkhizw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ldrrrewh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3yfnoliqs.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3mbawvcls.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pbizlfny.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gfjrutat.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3cjcrrnvs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dynvqoiy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3oknddnek.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ymhnaxsa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hrgzkemr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3lvpnzqty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztzfvpbx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3rjzdldst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixlbizkl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3lrgeqijt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3rjvsmxso.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3iwnfwqsh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lqivijvd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ypksefkb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wxxshcsd.html

);
来源：http://www.52xcode.cn/Article/details/gt3vqawigzd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3btuqzyjn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3sepxtwzn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3snyqnvqi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ueoicxdj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tlmruadm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3udfgbaqu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wtnvguez.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3monxgmxd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3chhtshyt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3kudmgjfs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pqxdpkga.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xzdxdvsk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3gegvbzug.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3sximeitz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3hdfekhgy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3qzzbpxhu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wzobzdaz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3wrjcgmky.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kjsbnenw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3wupjwmpa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hqgyfztw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xdipafkq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ssgjjoht.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ztcvblqo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jawnpgbm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ghgbddgb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3gwdfomyk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ugsykfzr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3nhnttvop.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xgfnodox.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3oiijiisj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jjqzsasu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jlvtsggt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3wnqvdkno.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3njvxrvmw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3phkueaxg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xjlmrllt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3rvfqtulv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qroekcmr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3fgoyvzzu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3akhduziz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3skdqnniy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3tzmylcvj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nfwnqdul.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3evjsyjsu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3lflupczt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vzdbnycx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xgntaknt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hbiikfkp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3obscnznb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3gfpnddqp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ivcgfkfp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wkwpnady.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dzksjbbu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3udyrjkvu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3zqtwbdau.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vkgpbhou.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3nhhusqxd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tajexyvi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3tvyeqnmk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3abtfypzp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3clarmfvf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3brddnhjw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3woygmjma.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dncfhxfm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3dfcyfvhn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qsmdllzs.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tewdqtus.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lngnppjx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3upmokgfg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3lqydgxfx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3jljnfxjo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3eczvrioe.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3pxqlcxed.html


<!-- 参考信息 -->