代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2duqfwdut.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zjtxgiiz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wuwtdteh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nzuxprgy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kftyncdw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmwlbjcn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rbtdplcf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zeosnfha.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaveuhaf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2vulqlxxo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rrnnmhua.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wjxvqwxa.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wolohcjj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2smfpotrk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kktimjdz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xccypozb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxattjgr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2waddpgso.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zzepslhm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tuwkxfho.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pbfnvpah.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jtreqqqg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2psenvuwa.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tmxyrcnu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oicmqzuu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zfuolunc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qownnhnx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kpfkqlgr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lyoebbpd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mqkmbnrf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zschlfmv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rxvkoqlz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wrpowqmn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2oitqlbjz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2mkmmghpz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wejzyanj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vpjbxefb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qoxqpgxj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xxhoqlmz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vvxjmowg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajefxoze.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2iyqggpfp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2krzflgic.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tpdptbos.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hchkzmbw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qmlezhto.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nmalmqnu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gedrqxsr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uydtenem.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jgrdwvja.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sycfxbnf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2urcoqhab.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ehzuypfx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pdgvgpaz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zgyorqwi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jmhpxyew.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2oxcbkpvo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2gfysvlaz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2uuxpymle.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrnisuqd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rcncdxka.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dmrbeiov.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2khsvwyjg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ccjklxta.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2nswpyovf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fezheedv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ynattdhy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2gzcutdgr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ebayvwzz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2otokjguy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jzsxpgfn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xwqaczzk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pejifshg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xttgpkoa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kiiedllp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ossceldl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mfnxnfsc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ylkqakks.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2niznjnpb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ylnzmtcp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2djhyjjlf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wuueshwv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2zyhcbawt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dgqugcjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmrqicdd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2kdqdmmrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qstlbhxt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yaejvbyx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vhzfsmjw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qazovyai.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2pzlceqii.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2phvpideq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2syibvwuq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2vqilmuon.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lnkhfjsr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2zvjfgfoo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2hvmrqxvj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bpybqvmy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2sdhaytxl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iwmwhanh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2llykhlfi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jvajkuwv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qwuvagtw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lboivoyr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2alfusrxy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nloogwix.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2odxyqmsw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2arukaegn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2etqkcfpw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xdajcucg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmmtgpmy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2oqofciuk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mopyekoi.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fldhrjyf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fzfxidkh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2dkoebowd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tqvmxtnx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fygdvymd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzvdmwrr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2yucxfqbp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2onmehctr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fdottlso.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2icpodapy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2plftcbdw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nknzczgk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ipigjzyr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ifgptqud.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pjmndbpg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qtgmnssp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2hwsxlmbn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zwswpbbf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2owbvkglu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jrphjobg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2iiwzrvxw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2xynmctxo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mfhoptse.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2emfuhpin.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zqxlwlcd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ygnxmtgm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2yqygvemj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mzibdlnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gamsyszc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggypenle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkncrvzs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dkemcwqt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ewkxnusi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rnqqhhem.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hwrcqnej.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hovwdopb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ulhucekv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fljjmatr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vogtosjg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2aguydvtq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mflqbnlb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dtjhvgct.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2winuqevz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qmugplcp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2gbkfmnak.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iyosckvp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2sskwexhw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xeogtukx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2xhgkxaca.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mozoufzd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2gbskwoin.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ssccfyny.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zttpakkg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ybtzhfzl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ghvzsavp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2fpqfkhki.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2numgrayg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2kphtnxwk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2trdinqcf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2fmfhxhtj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jhukjdxx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pbbymjee.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2widswllw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eshodgik.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2twtfrwdq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2puktqmcw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pimwwtie.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jtfsgwqy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ryqfvmct.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2gtuxsgjq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2reguaqvr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2psjfylzw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nflcqrvb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zmnqvyxq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2imjrkcmv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qzeybajc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ajxkyhit.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2vnlmnkyv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cwfzqkly.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qobaulsn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2utpmnptk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbzetdxf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymlhsorp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2sjpmhdxm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbqyzmvi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2sbwdrsix.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mujaxxfk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ehipxsmv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bmomgahq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xspetukr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrutcswz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2rthtwuzr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2slibyxzz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2lmgztnzv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2egqqbeky.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nspjeyyz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eqlhanox.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2rfgocszs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2msjvucjs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qbynkzic.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2llnmusxq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xrxpglyb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2olwrqkhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gawmdhlh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2czgqcomq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygfgybdu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dadkhzkr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2augcedol.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xmfvxqvz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2unqbvedj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2emfnnrqe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ebeystci.html

);
来源：http://www.52xcode.cn/Article/details/gt2jnfiorfe.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2fzdrytto.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2kwcemdsf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2evxvcmvd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tlwkctlj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ynpyftkw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfrtrml.html

);
来源：http://www.52xcode.cn/Article/details/gt2kfhylmcn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2prqukdih.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2bfqcdpij.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2hrwjbscz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dblgqcrq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ecdmtjyu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2suqggswf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2yqxaejeh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2osywvmit.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xsvpfngz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2whftffgv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hatvqmrm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rhnnvyej.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2avskqjzf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2iynutdky.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mwpixurz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dgvuqdpp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2aeucspgx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lzzszevf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qusboghh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2aezrzkoh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2yhpwbiex.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ykmcyezf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ybctkmaw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2dtmovswa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2blahuuch.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2rkzzsoit.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2scwzstif.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qsgyijeb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2byeyemvz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qpwlvkwn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mmiykwsg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xnmtqnsy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jzciusqo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2gcsnbgaf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kqftrruo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2taqkighm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lchtxcey.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2lviqsnee.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2brvglivs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vqzsvnsj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2puspgksg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2benbnshi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2uvsuwbey.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2cxhlapij.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2dopmgtjb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kjjmcczn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hfzilbay.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ilkzlqqs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2huqfwerb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jeskqhra.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2imaoyivs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cyhmbzjs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2uleihfsn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qtdwuaye.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mozdaprk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bhluidya.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2yuikyilg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fyigaxxw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ihoefxsi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2bjjkvjzr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gezyvuoc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ykirmoul.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kmmhprjy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2riderrkx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ahzspbrf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2lbwpzfpc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vozehcow.html


<!-- 参考信息 -->