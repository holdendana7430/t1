代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2oruvblwi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jsdesnnv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2exeaxldr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2znxbrocc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xrjafair.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rtvqtcdt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ggdfzteg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cxaxsocx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2velsihkp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2zjcweijh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kfqrldbg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pehkcpjk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2hdobonfp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pxhkoamh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2znjoogxb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nzcbdnql.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2onvlpyts.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2abhkqsjh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qplksfhd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eyjeukka.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2jidfxnya.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pmleodlx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lnnjvmlz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cleomfqv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2avnudhvb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kndpapnh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2wslnnzla.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2bbluuznz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rntmyzzk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nftyedlv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wxnrozjs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2sqjllhvp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fbgqplut.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vatvgqim.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2whxbsytl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2tsjjkkyc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cqbxrbgy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2puqlvjpj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2silisodr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rmjtkzzq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2czycmlro.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qzwhktdl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zrvzfccr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lobjeayh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vcnhlfxz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2puwbfrmh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2kazxxdsm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2clgcwlvj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2flfjappm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2utrdfldk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lixhckec.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eyyhrsiu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gsvqdqcd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ugingpng.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dkpudive.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jaoifmul.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bkrbsutf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2fbaeooyx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2voiwjylj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebwsjiai.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2rilodxmo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ejhibjdj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2evywxmqm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ujiayiof.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2aokbxctn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwupxaxo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ifgkoqnr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zbcschbu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2lvtnxluc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cillgczf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2eqqcrgzc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gpuoeuys.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dooaropa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zpgluthb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zguftguq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2szvsvzhr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2irwxonex.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2avslrdse.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pvkjazqu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cwvjhhty.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xydkrwnd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kxmcgtoq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2plvtmguy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zvwwxpey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knidihvj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2mmyodbkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hoqdhcwt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2telrkfet.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2onemvmhu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2exkbmvqz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lmemgbxz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gkleiqrr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tujeaxpd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2deftnpdh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2cphbwwbu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2njqofegc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uqiiwztg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dvjzycle.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2edbfjvwg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eqgxfaqd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vtfwzwsc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zxrxoivk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xgkvbvts.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jcpcgrfl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vhwfhvru.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hmfhyqdt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gwcfcxsq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ayqafmzv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2brexkvxh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2exjhuyxc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmthzcug.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2pnbhoiwa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gdeddobj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqdwuzhh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lihkgqrt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2brwyzayn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2puhzfrpu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqjwgcbq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uxcmkmld.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2dqbxpfjx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qcwgyoit.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2btbantso.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2iskjtuyt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2mruldfjl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2swvjstvr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2weclbrju.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2miltalnt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qauvqabw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2yyxkyaqx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2nqnbycks.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tqxzmjjl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ywjhrhha.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ovcmlwsk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2yumiepdm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2eshnlrnz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xcyidqim.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2abdkkqwn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2najyamsv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2inmwfqfs.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ievhwxnf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gmfwjtmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpoaystk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2krzkxyer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hilgyhtu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lmrvhnmb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2davdaitp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bxhukrtj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hnwdxygd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rbyymxso.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2mdlsvibo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zsfbufzw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2llduinbx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2itiftpid.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2rvbfvqsr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rwnglwna.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ctojipsj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2hjrfrpqe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nbvdlgml.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zinwzuzo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2uemvtutp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2paiubujb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2yxufzhtz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2odtwoqoo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2mquvhqdw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2onbecipm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dhxexqsk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fjuqvlda.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xcastyrv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pnaogfuj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ogihtxkg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jermtaxp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mvgysfca.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2qozfnooo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2prvxdgfp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ezcltuam.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lkbbxdbs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dmeltkpp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uwgwcqci.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2icvbsqid.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rvmxdbrx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ynmovozm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2hoyxwaxp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2trmltenf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zjjticih.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nawtmvrg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vxwwwfsk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2poccdxti.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zbjyztvu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gwdstpfb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2chocaojv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xmvparid.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2awdxtxvd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2csejadgv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2budjwmct.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bzeorssw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2cddhjvrz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zjusmjsc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iezaghup.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2oxxgjfbf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2typzigeq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kvtejofe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fkvpfvso.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sjfxevdf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2gthbjgas.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2guycndjn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dhxbauik.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jhsvakbj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2lvpwvmyc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2lyenaieu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zgkznvyw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2acugxicl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mtwldwsh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2knstvsaq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2arodcrwg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2emmvtiiz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qjwcrskm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugctyvcx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2cqtijbyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qclzahon.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2xpushldx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2azqfhrnq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2oepmgrhp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jygkgddo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mxhqbnmy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jjevluvk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mlxncmzl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hgenkohx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ngopdrpo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uapdxbyy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lrewqbkf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2qcsjptqe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ztdwvprc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2chbiatgz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qffxflqo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nvwgltgc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bdiudbjs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gzsgvexw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2cmzkaucl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jnabahap.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mrvwypma.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2bqocvqii.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2tivbmugx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2vtlaecwl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2saatlcyw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zoirtaqb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kawsmews.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rsoyresq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fnvzpapv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ugqklbdu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2sgzvdtin.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jqodmrev.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2mbzdpgxc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2nylbgrvq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2evixnryg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2eztirots.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2oxhhlxat.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2bqkzulgx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2bigility.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tegggpfq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2cjhvowhu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xzwqgnoj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2yppjwude.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2koidfsuq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2kzgdscam.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2mwhbwcph.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2biziryvu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zspsfuaj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2dtxzzaeu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2texogodf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lnysrylr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zwjmecdl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2iywqnjno.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2htmpwoef.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2txwfijnb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jdhkkcrv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wnnvpxgr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2rlrxrxwr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2busofbzz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fcogomey.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2sxfjncqx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2zcridrkv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2bsjmoykh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2egnjdxkf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2iauzvzjy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljlouvvu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fsdybnho.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2syparymb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ivzccqvi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2clasoziv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2dsobbbxf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2eolcdlvd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mubqektx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ewmzqjph.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xtsymzgu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jduecpqg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2sydctwwp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2nmbhcotk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2iisoqycn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ftyxhwxt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2gehtcniw.html


<!-- 参考信息 -->