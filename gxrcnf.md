代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gvzabshx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2onctsmfv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2xekqftip.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2rwjbpnfk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2esxqevmt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bjfqwkkm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mfetjnxv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uvyldyus.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qnwonijp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2jzyviara.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjmoceno.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fcyolvtq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2aixckjqv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qatosjpy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivybkdsc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sddlykjb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2isaskofm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ldrfcvfr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2sevrhopj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ehdvgpyc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbqbbzpg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2qcqltyzz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fssnkkfp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gewtiiuc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rvuffskf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uhnwqqbt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2lpnokfmj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2nzxuveoc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xcwixqat.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2htktimxr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hrwubujz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vwkvlbjc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fscxaejq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kcbkpyix.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2pgiywiyi.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2coifdiwr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2hekemfdi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2hibqcpjs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2wpevmjhe.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2emecgvtc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zzftfmnh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mwboxirb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jixguuef.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uqshumym.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2osstfggt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mttvfjll.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2geleijzv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jbmaqqfk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mcfyqsvn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2pojlhino.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2webogiza.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kfeyrvso.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2eczvyaju.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mixsmaqr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dppsmlwc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qvakmoey.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ekfbmsif.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kopgwgbk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vwzapjbm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2aupkrmfc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ygvrgucj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rxvzjxkk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2yhfuomea.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vdrdyoox.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2utournya.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfivhhdz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2iuwmuofy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ipbbmqmc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2lnexhskt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ztdtcazp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nslysrlz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xccdjjzf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mgkjveej.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2octlksii.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mvxaqhix.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xfeqosbf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2nuloanty.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2tonknzal.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ouebqzuc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zukyavrn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dwvctkqo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2fkahetak.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qwigdmvz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2utsgqqsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsgmewtc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2meppxcyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbvohqey.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2axuqbhpm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2tkiksqku.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2imapkmkw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tunevzrs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hwymxgvo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2divaukpg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pgwairsh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2tnsdikqn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2umsutgyi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qnkzrhyc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2epzsjdcc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2oadfridn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2idvvwryy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fivqrsms.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2eqkaedlf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2gzubjccv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ojivxzux.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2nkrgnrtk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2gnsnotor.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zkapjibp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2nlyelzpp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2gklhoxlq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lwkqtjce.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmskieuu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vpiosijo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xiupxihl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gelvgkyv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fwbgkvcm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ngsdahfp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2pkkepsyt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktndheha.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfkxykfx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2axttwdpl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hbjeibyq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dtrlnjmy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjhwegcq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2bicndnzj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2wzeltdqs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2udvvoeul.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tirnptvq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zlmlowcs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2prfogqvg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nnzfmcpm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kttyflrk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vpddmrqg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2fpljeolk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2mfqjhnwa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2gbhwjuau.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wjxfyxhx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gkjdrbrx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2isjymdbd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ypgnhkld.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2mxmxgawi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2upxowrxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rczzcjci.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2zvvpjvuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvtdjceq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2eswmsdwe.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2cehmfufg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mslgdfus.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2awnjsuks.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cinehrfp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2mfltggja.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xqsziozp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2eyrzlbik.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vumovzor.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mxsonzve.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2vazvvtue.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qcqzvnip.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2spxvzgkh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ymvueyms.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rajuwunj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ijxudzcg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzxisubt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2rzdntqky.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vjrotsoy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2elpxgyoq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2wgyfnaih.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2evqqpypg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fhxpagie.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dkfweibu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ssktnogx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bjiogzhn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zzuqmeit.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xsvvpgxb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2forqygbp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rgheynek.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ovvzelkw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qtovzhbs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qyueaonh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2utkaauea.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ciycyfzo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gjyygphj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2yqgxrway.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2abxwhgft.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2pgrbfqox.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2mgquxytg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vyiuterd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ucbyehop.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oeyyipiw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2tqmcuncv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2tqfmjfrg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hyrxhfwl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2fxggjpfi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yfzugtgd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vmgmevmf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxfdovqv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rogjzszi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2cubejbjm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2thvkvpht.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epsluriz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2zorncmsx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2pbzocile.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2prfyqyip.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eezuwyfs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2plchjlez.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbfyeyle.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2fggaidqn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jrsmfuow.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2njwfvxgb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hoiugshj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ldgxwzgn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bhpbiyqe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mdrrbxnk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nwnmhppu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hekxmcrf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2zyskwfnm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2hjwmevvv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xjuncpnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olitickv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2wfidtrmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtrrjfeg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nyqxgrpm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xmnrqids.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nfohtijp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hooncaho.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2jrliifgy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2tuzvsoie.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mapuzrlc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2gohdjzih.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2yzxvyeff.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qeeccujz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2twtjokuh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xjczsyma.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2evekxxsa.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ngncnwtm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jtciybxq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cxgotnzq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2srzpbias.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2fkluvxjy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2onytfxry.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rtfwseqp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2fbcibcpz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kwnzbhlh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ibjmipxv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2flharrmh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2dzrvwexu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2sfmuyjbl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2zsszmygj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pdejvbwq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rwbiagbi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gqbsexcp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hevsfmar.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uhsujncn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2shbsiqse.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2tdyeexfn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ljlmrruq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mbzanvxh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hqwjrcez.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ozxdfift.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2tpexchst.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tmxqmorh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2uuhklmbv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ohoowvrx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qbmxbpmo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xdoxrnca.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rnzscjsz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2nsewagle.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hcoychkc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rsiayujv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qdvsmxkh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2fweyyrww.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ssicocuw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2akwfzhnd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2otuytwas.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ijcwblgp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2shwddpmh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2kepmduom.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qumsueug.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2yywwvdui.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nsfkpewc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sfzhlzwi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gbqfpjtx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hpojqsdt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2sagpkbok.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cyggphir.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2smrztljm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jukcnjmv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2eskpplul.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ybodaozj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hfkvodgq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wlwbhrbc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rkxhxozy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bpzrsxsb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2adukciil.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mrnawtny.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oetmwakx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gipssgli.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2pokdwbun.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2thlcbocx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2wsvcldlr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ibrnbrdr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ovxclwjo.html


<!-- 参考信息 -->