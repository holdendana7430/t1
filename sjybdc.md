代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2nmsftfax.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2oykugvki.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2pczeohyy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gifbxrpc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fdldcysw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ovvsfnfz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tsgbrzhw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2spamyfvr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2spqhnvsl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lybybcmd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqrbcoph.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bndrzkwm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wywkywyf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jgffquns.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2knscocxd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wozoyaqj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2urbqhwhd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2wooltukv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2epjdzzkk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2cqrucaqw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ujayffvv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2vsawpahw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rgrmgilf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vtxrwmjj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qxxbhbjx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pvshjllv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2radpntto.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kytpixfx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2uspvboyp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cfpyqanf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2awdaqtys.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2kwknfimg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ipnntixw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2noebdkxd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2jdcnhltd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ypwgcgxe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2uwiwhnhk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2yoxhwpzp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ncpjytrw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2uprscpci.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2qyfgpvwk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2tprijlhi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xzjvagyp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vkegknfl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mapvhrpe.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2srzjyqja.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dofwkovg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2trphlxyf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bktxwwcx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2srawfrpm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hihftcir.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pialgxar.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qdxacohs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bymeoiul.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ouruampp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dokebhnz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2gxtpjlox.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zjuqrbjm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2jvojhtii.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2gehvzrag.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ktixmqvu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rmjafkio.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2frlcaksr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2yaeucsrb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2bftawxec.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrdioqry.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2shgetrmq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2adhuipmu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2pkvgrnwh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xijihziz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dsqpguil.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iojscynx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iqmkmcub.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vdswvxvv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mknqhtth.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2srzrhfaw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2tmwnvapo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ybqbtqxs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jfgmnyvs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qbgshylw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mwvcwfic.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rpnufvnz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2eykmoohz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2keeoxpaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajkyzcyc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2shqskcnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efzlrwyr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bfvktumg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bhczmpmd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2dyhjswxk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2boihzufc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2stqeyqhu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2errlpjsw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2bsxpqazu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2pknidfyc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2oefzrjgo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2enrfdxhb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jawdfpgp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dgypklfj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ippcszeq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qkzhuxsh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ckdpttli.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2cxarrpaz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2yqssodcj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2pmqjisio.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2pjuwgddr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2adutgfjv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hvcvjsfd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2sugfyaol.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2teugbkqe.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhhdoymq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2axawypbh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ilghnhyt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcqhkopb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ekwxtkid.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ofehabmm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2oiueelhs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfilltkt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lonoquif.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ctxitmgs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2mfotuzuj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2bmplemve.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2skunqoet.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2pciebdql.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xybtssra.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2aielgxtu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tgfnrbcc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jcszslae.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2kxvteacv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2srcgqxpu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2syijpwaq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2judzjovd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ddoupxex.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2gtqcgtzr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ycryhmrj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kzvjtetq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gfzlulmm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2euolhaan.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xexwrpkd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rmuhqpzg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ymlcatkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdbdybqo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kswvnmls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frodhqma.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2sirkhely.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2xwnszffg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dqvehccd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qtdcvorf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bsossijr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rgeptasr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rbmouygz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vqnxmehl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jvymwknf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qgvsrshj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ycremcgy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iauspknn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wajtiihp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kumgvvec.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2venbqjhz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2cajimuwl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2fufplxht.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ejjoswaw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dlesyish.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2uycpttjd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2chhqxyrk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pjoacrzi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jzqfmqvr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uekodmda.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2iznocobq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pyjqcfpk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2zqctnrvx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2msluvurn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2gfkvbiha.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eeldtcke.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2svayopwg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2luybmugq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zmnfmcwn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zwyeluci.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hojixqss.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bxcphiwv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ulukenfs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rljpdfje.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2iqqqnzbh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ytyfozqs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pyphzuat.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2gynkwxde.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zvarsagt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vchlbryr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bxsjxyeu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2bypdwtwd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xyleztlb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ssnlhihh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2weetwrla.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ktysifmm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzovjzcm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2cvumpars.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ravvbmgk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbfluxwt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2msbntclz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gopxkknz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2acyucoli.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2suszwafc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uxirfbcr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wobcsdnu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2dueotsnw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ujsvthmv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fktdicvv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2byacjafd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2wbpbzlah.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2etwdeznv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2qgiekake.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hmwezdfp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2oazfmiun.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2mwsalkhf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zptigagl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ffdsrngw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwvhnzox.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ttwnwgip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sagcylmr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2mlobpric.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2salruoml.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2djitssmw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2puxarxdm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2inidxurl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2mrlibhjp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2syicoong.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2asiinlst.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ucclfmqs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jgcjusxh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ldzztzmi.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hwiuppdn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lhasngoc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2koqgpvya.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2eanrsgss.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2yougjtvt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2kgbmscxh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2onnmlncu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2euwhqsfg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2yrzmcbjy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2hnqzqhro.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2pftozvpb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ljlwcqnv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jbwzkati.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vvojfuwn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gjqsqvhb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2zrmviypp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dyreqdgp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2nzehexqc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ylkgcarp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2daayrodo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yxmbdtze.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2tdyeewqw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2zljsuwpu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lqmbeaby.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2tnhrxgfa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hncjvrlk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2aivojtdl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ignypoin.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2yspcdvgy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2nfrukuaj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lqrnlcgq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ontotrfa.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cpfvsjtd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2plqvxzol.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qnbkewba.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2uphmacvl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zcrbccam.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2pmzlvvpr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vrdgmblq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hoiozinn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2quazmlai.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2opejuekl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2sjzvtrzr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2nbqceusw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2uznixowc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2lytkhrca.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kosgbchy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2itwnwtjw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lkkdbjxz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ogbtsyws.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2pwdhpugc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2pexapoxc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nnlqtxls.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ffeubxnq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2otbzivht.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gisldhnc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lcmjqopc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kkxejdbb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hwdmaguk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ohpjwtua.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jfyizuih.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2onwepbbh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lxyktrxq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2inarvmby.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qcqynspv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ymzcbmvp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2dygottea.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ivaatxrd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2fsggncsh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vyplvybd.html


<!-- 参考信息 -->