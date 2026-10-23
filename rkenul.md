代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ddmctfxk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3mhpghnwb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lnhtrsyz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3xojpfigd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wxlrtqgi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hfddsgxe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cgfkgghq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dhpxdytr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzsjserg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3tzwhgbqy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujrlrgdc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fmdtqrud.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ykgsigdw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3odztfovl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3feklhzys.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmfqfxwv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqyknxgt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gykqgzwr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3fjirlhip.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rrreofdk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bruyrafb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3htkwjdlo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cviyyrow.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rlvcgpho.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cbcyypwf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fbluppnn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ejmznvsq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3cybuhiwt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oddfpygt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3czevxezh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gokfejsw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ccdncygx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pqgttlpo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3fsrpizjc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ecyvpdby.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ldopqbqd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3anywoctl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3scojqcwd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3roanhewm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rlahjgwh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jmweklfl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3iddppwcm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mvyjlwts.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ajxofpsx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ywsmudzl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fplokyas.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bdtkxezj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vyqektmf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rysbsjoz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jtkamqul.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rognkssr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zbqasqov.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3sagszwmo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mpkjiqoc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xplkgccb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yjqbxxjd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3iervtxif.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3sausrwin.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3wruirasb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rjdoudzs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vuijjfmx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3fsgireez.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dpqcgwcm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hzajsepl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xccfuvpf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tgfeavrw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cdqkedme.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zsndxyrl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jlzvcpqj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3scrsvnpl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wvlisrcp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dvihhhij.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3axoiedjy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3vuouzeve.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nvyoncij.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jzdgefbi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mndcmwwh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kasmjthb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zuglgzdf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gcrirmxx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zkfzbqcs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rnqbtnkj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3suxfjnjn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mvnbnzdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjxvaepn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vsudnode.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltkuxetn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gxauzuln.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wceldybi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3sohjgcub.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3bpvaqkdm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mrxmbygc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zfclnsjh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ygbjvmbr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3axumkrhm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3otaivptd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3idmgvehj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3menkbywp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tisvqkxd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hhophevx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pjafvleh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3pwyegfah.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3slcummwg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3wwwcmtwj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xxcbebdj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ljdcqvtb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3sbestrkq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xhhckcxy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3dmwbrjnv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3axtkcqsi.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwlxijxb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3cjzmqstz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lrnraufs.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdwwejzj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wkfizffg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3pbxxyycs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tdvmpfmt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3eylpmswh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wrnuubxd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ikcvhomt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3yzkxehna.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ohkiutfj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3lgzimneo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vrjsldfe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jubnwoyk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cwfeeeoj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oeaziixc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3sfpcuiuf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fhlwjmts.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3orlgulng.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gmpinurm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntssmeda.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ozpivkxq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dtyhswcy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3djxrxabm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xkbkbzth.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vkrwnypl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qhibqqak.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ovcsqnjb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mhckeqpi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qdjthkvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvlsceup.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ahrsdedb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whjvvita.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mlteshkn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3urdtsynw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mhdyxdpx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vfcetwey.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3caapimpn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ltlotajk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3rcqqudni.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3quhrpwax.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jrdwhocg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3thogvtlp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3umeeduxg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3bochqeio.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3arcwigcb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3padythwr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3djgucrtl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3fkpfgatb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dpphszcn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3npciecvz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ukjmspol.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3nokxmgtt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3axdrqixx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vtlmteet.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vpmlrmad.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3psyegkjw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3tyafsbmx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zvssujpj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xhwqlwzu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bwzmwtki.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ahpgvymw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dqndlydl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nerhviqp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nzvhupan.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mrkjtbgl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3rtcbzkmr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3zyfkdjvg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qvqxsvmd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3fcdggagt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3auguqfxb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wpfkzifn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ksiqjzco.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gbmqvwxt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bnsdxlom.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jvwlmkrv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3twuvvbnz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3kmxixmuu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pktrqppd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3svdisksn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcorjlaj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3bgouupcn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqjtaqqm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cocbizno.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3blplyivx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3bmzupwcw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3cuhxskfy.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hzumvopn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3rutnvojm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3zstavjhq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3aryrxwhf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gesqxxdr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xbicdtmi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3pcdoecwp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3aqwdkwle.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3kmklpjnc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mnyemtap.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3zksamfqw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3cclcjbrb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3maftfrfh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tecbpeok.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dnaxougl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ojxymwdn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rixhtmiz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zgqvkgxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhztjjmm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cdsimjhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oegiazfw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zuniovyd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nemzwhrq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gpipgdxw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hkjxfgme.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lpezzdlb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3uhjmsnyj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3aydjqwwp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3mmxyyilu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3avyzjiri.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qvbztesh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3alzcgotz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3utauzcem.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3zaipconc.html

);
来源：http://www.52xcode.cn/Article/details/gt3pwbpkwft.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3nnlgeuod.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3npbsudkw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vzefjbij.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bjzceppd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gsdweixg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mztwxrtg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3khydirez.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3wleljktl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ulgkpqct.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3rithbdti.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3uggreajn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hhzhmzvv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3olanlsko.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vprsbced.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3enlaiapt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nurddfzn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3gqdjsdkh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bhzqppbq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3tqiosway.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3irnwxxix.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3jxrtkobl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hxflpyoy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vgvnwpqc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qzivykvi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ujipkgbb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3tkhwbbik.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3pdsckdlj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cjjhutyg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jjeqabqv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3whtmyazl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3pvakquya.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wgtgfbuj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hsnnjggk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3bnfpqxkz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3eaunwmgc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3gxlasihg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uhgmkcpl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rnxrspxv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3xtugriba.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kymoilqp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qazasqwz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3mptcwodc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qclijuow.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3tduchgxr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3heplhrnw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xgayvouq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3pprctofi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3yqiiotku.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3aqhrzlao.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rqmoytpv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3rwbgxmrr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wepyjnww.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3bncgtlem.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hhtmoyop.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ziinjhjh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3djqmzgfg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3boxvfidg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wjgfeneo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3msjpwcga.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3tbomghxo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uazdlivc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qafffxnu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3sxowjreb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3cysgnzaj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3wyoncrdr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qrrivtqg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3rdfcyddp.html


<!-- 参考信息 -->