代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2aizprkap.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ntxyhjhp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2jrekhpix.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fgrrcfej.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyvvfmtg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2niyzdtxq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pfsnxmql.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aqdudlmo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcquttyn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2bpbxwjsm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ibwqdbqu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ouqejxsq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2tirwusqx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ujwanfkc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kfzlosyq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lynbapuh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dthjgjdt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2egugnbej.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2nmktzzdr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cfurwxxa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2absgcaaw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tbjcjska.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sfzewqtn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2slvktqub.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2szbyqshs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xnadwzft.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2clgyapyr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2eoqcywom.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mypqueti.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2eadhadxz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2heljhyri.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ppagzbmm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2tdyabfzw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vgkiwcmd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kndeccmd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lekdvagc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wprmpxxk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2gmomcuir.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2gxixzkpp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xiqfxgal.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twjkasma.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wgitqpfz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jmrpfgoq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lxsezwxm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dlpctyhz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kimfbcjn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2uzmkclyn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qaefwkrw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dcrivifr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jluuvzzg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pbfaonjb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uqpllnxv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lzoqsyny.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2aujvpuzx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vjgijrkb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ogsrzlib.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2eueabbyx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2dpdxtonx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2dzizlrrl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffbcyhpe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2eoyhnccm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xgtmmkvz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xedagstr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cebszwxj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2uckjvctl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xazljaur.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2vusdovkm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jtypeybw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2eohklbwy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mqbavvfd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ofraldex.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jautwdoq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dmwwotqr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2alphekhn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2czgtvfdq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yevfaucw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2qbvunccx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2uetamzfw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gumihwfc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ekooifmi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2njaonuvm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mkcmxqip.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2nequlrdb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dsdcdheo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqpeeehv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jretyjig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujmfrfgp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2geonualw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2enxpflqy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tysiuajw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2molhusdz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bcvuxvie.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qalerfrh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bloveqao.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2shrefyum.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vwacciet.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2arravbrn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fwobhabv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2xxjjkcap.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2diiownmd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iayxexuf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cyrwggud.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pnnafvgf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ncmadjnl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2muzkdtux.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kvwngies.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wkqyjzlr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ozkjyfoo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2surimuzk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gvhgtqtm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qwehhfql.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2pvwubotv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nrkbfnom.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zfcyjpup.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2iiaetxje.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ydbnmkan.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ysapaivw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tbeqluya.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bprmlfby.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2vzjxnzlz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rumhbvwg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2iivynntm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dctdmhaa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2bjtpjvne.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2tsoyzphp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rcjeabmz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qdknrqjo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2olffxknq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2crwrrhvf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vztglpss.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vletvpfl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ehcnlsyb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2eveancox.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hznecajr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rrvjhtll.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rxkigpoi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2accvwnov.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2thwpzwph.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2hlyzajis.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2sstezkwz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2eubeeiov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcsopnmw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2srxbouax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzstycxw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2aqzfvyja.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2yrojwbim.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xyqglcae.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2azeakcwr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tpcidwtn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2lsbnvbqy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2paydjhtk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ldeysica.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2shjegryo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zvfchohe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2spgspcix.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2lotilqyr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2tnqvftar.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2deleowqq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nymphuvo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kgkrtdmz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2qjtvxjhb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dhjkfsoq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2edvxmnkd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2isjuczgw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vzgtetvn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xxegkfgm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2quyfowbx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2kfojlfog.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2eqfcjyfh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2uvxdluaq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2kwdogaoo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2poqpkusg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dytzndcd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mdydpavd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2udwqsrbu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xdslkvyi.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nsfthkmn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2kbifpdug.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2trloywfj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vdifluko.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2sflcanpw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2yaihudou.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2osuhsicy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2anjzrajr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dyjizedy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rryplopt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hdmsbsgf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2beccbnrx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qycsmmmd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2oblbhzkq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hiogywyq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2frtlninb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bcjphptd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqgcuaay.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upqudhxn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2kbarppdt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2hxsqvrkd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekohblfz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2qlwicehx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ulleldpn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2noosjgbd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ucdbnmvc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hdmnpgli.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ddlmidup.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qxzkegoo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jzyexnkf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jmgcrzwz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2dxuauhxj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2flrfqnku.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2djhofdil.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2pxgxxjpc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2heusnawj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2stcgcreu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2prnfhkgo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qvuzujkw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2qezmctex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwbmftxx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2atnkjaqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kcgyieen.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vldicfrz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2eyqtiwmr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sfpcpfrb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rjcwbjpj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2romwmprf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gkwwzyzb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fgbgckzy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bgebsbhg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vlszulaf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kfioeooj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2swkiuwvm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mfpykemi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2dqeookwp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2taabiczh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2npcozzxo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fsgwhica.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2txkxpqsv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2dbkvjjxc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2dwuzpgjl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2grgbhlhm.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2vjaragfc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2hbzrnrfk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ejjhacyl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2diwnyjix.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2rzwtntyg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cpuxsqkd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2bdofywsi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wzyugvvl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hpksvzhs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wigxxiip.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2htmtveqa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ajktymmr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bngllqxo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pnftzggo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hotnzway.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ztjpzcpq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nemfyywz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2bgzsmlov.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wyknafsn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2nmpvneoq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2urvjxngv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sauxpqrj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2asdftggw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wfjjjftk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2viilantf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2taetewkz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oompwzew.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ahcksqrb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2elsnofop.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mnbfcgjq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jvobjhje.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ybanfihr.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mxgrzbhk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ntpsaute.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ssjpwdjz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2noqvdfwv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2pkvtzhng.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2yvqfweyj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vivymalo.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2thswhqgn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jiryigml.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2eurjqplo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2mghcuwft.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2khvljepg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wzccktjz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2etdbzyqo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wuzpfgtn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bwczzrwc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jqnkvjba.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2upvzrrdl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2segrxlui.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uwyjuexm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2xrwujifr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gtkblgae.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dfakhymd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jurdmfls.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ngqjcndg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2njkmmbhu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bridhrtl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2lrmklaii.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wmxyjsnd.html


<!-- 参考信息 -->