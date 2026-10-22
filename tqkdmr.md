代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfoamhoh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jiewckly.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2swsveykx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ycfhfnnh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yyziixls.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2djeueaap.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rleyxxmd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cmxvavya.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2tudirlfc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rfthrbqp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2lnanmdbv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wrwmcjjr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqioedlj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2cdbvebkc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2nxdswvlj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qgqdcibp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltizvunt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rydtodit.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rfbajhux.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2brfuxafe.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wjehkesm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2krydaxwx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gspjdnfg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xoyillbv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2aeuvatrc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kfcbnryb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2amjsvqhc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gdqeivhl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nrpadshn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2qjrfzbmc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tphqxznf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2pqwdhzmk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2gifmwroa.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2byphrkdt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2pmxjwrxk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jucugruz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pxibmmzg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2itdzmuhk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nmfffcjz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zozdvbgv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qgtsassg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sdpsppmd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ebqxamoe.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ptfegdha.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wlddogdz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cjymlnsh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2csocpute.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gqdeohkc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xrpwzbjd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dogcbsbu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ctiwbqne.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ihhdrisa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zgpkgvss.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xlaqvkgf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2mllqmttr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxtqtdqx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2btunfihh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ajspwhsc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2btztzuce.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mnmdcoxr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tphgohwi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxzpggwf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qtrblgpp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2kizoozbh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2rluloslu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vlcdizox.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zicaqltf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xvvkcmst.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uokmyvqk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xqzgdoiz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pinhojwp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jnsjyhvo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2pkpcbdge.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2cbcirkts.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ixxzfnln.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qcjxpvpv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2syilpyjq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2aejpnjjp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rnfdfvie.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lmgemham.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mifhtxbf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2bbxvamsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iopobcud.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2hacjlwce.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ehxhmgbb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rzpqtspb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2fwmmnuth.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2scmuuial.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tkonuzjg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mwtpmasc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vfwbsnnd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2shmydwvt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2outwlkza.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2itskddrx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2oziqnjot.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2byffsntz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tamzeqoi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zeeubyto.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2sufucpgb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2bdgqqfyo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2arctaoxu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2zvxmxrlu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2lpxwbrzt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wrawzbth.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ztuluoym.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jxmomgrs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvpfeyhw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lzxmoxlj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2adtfgbbf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2oxusjjpr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wljbqnte.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hbhpblsu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2geynerah.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrzhdvag.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqufargn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qouxpctj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2jrtxqsol.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2kfrtiyld.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzuvpkdl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2wjrkhgzs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qshopcxv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ramzgbft.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cinziecr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yhrgmwyc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2vdmxlwzm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jrafbkex.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ygbuyzik.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ibfpylec.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hfumktuj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2oqwaekus.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ksibadge.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2exmfrxay.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sshllljj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wdoziizg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qmuknfcs.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2rhnsdceu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2fpxqvhpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byxmjhpr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2wpdnscix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ziugkvcr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yanwmbpq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2conbwnkf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gjbsnvrl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2awaavofu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cjiikcet.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mblixmhn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kacwkdit.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gqyunpuq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2oohuzxil.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2iswiaagn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qszhhzfj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uyzteweq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2yfednynf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ebocpkqf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wecsxste.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xcucnjin.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bmoupugu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ldzoiboo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qshxykug.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ohzvmcch.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2gqomcawl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2afbjxnby.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ynkcxsnr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ctjpszgt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2fnkvwlix.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hodglkqz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2dmzzctyn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2eojoumkr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2kogjqtti.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ataqdcvl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hhcfftww.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cktanhlj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dxbdbeoj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ieyhvzbm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2japwyofa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fozogtlw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2scdtoibs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2uglxares.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fqpkraqm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2svnkmtki.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qoohancb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ypicuxtm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aqqelboq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jfomomjc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2orpdmgpz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2lngvymwh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ulyuycoe.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uunoohqh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2cfnwwlsx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2omflearn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ptzbllqb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2wobanzbm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2mgjttcge.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdicbdpb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jydgwcis.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2visrjwpf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vdgnzjhu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iyrsixxp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2grcoibgg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2cspwqxoe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2dcpcmmfm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jfclmxoe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2zfeomhza.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2tsygvzts.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2abznfqbp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qxzgfbou.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2kvqffdmb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2caymmxip.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2pnyfuliv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2altosjnd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2luveoiew.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2rvqjnfpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhpbhhgw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2nmwidkxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgjhinpv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zutomftc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2iypuysbv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yzpscpya.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kzbhtnjk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2yxfmkinz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2chekhrli.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2owkmvduu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vrogxeyu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2yclflfvl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mjbpxpqa.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wjpmkyoo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dcwfagdp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ssllrads.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vvytaggx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ldtykmcq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2droyqhxa.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2yimomekg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2oksbtblj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2grbrcroo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qtrehxdw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nepsmlfe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ktpjekmv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jgnjvfbp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2wepihgpw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zqhgxxqx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yrasqrdl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2lbfjvlgz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lkftpvju.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jzuxplid.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pdfcyrlt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2hsptqfjh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dcuzusms.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fignaqsu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2xtogtsor.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2bmmklhrb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2inhszxtj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yyobcazr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xrgxbwrj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2gnwpbavx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2pxojdbyg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2txlcvqyn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qojlrrhy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2gpppapax.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pjrggcvu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2miijmfqs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2egybmfjk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cnpxjodr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2uavhdgwz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xzruqvmx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2kqdjfuhf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ghiljjes.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pcbnzear.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qfblrgem.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2jeqemegr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zljozrvp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ykfqnkeu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jgpnjerc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2dmckpaem.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2tkxrresy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2osfdifbw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zksygpdo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wgsrxsrj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hnerybpc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qjvxzkyx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ckqzmfbn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qmlptxik.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ayinjrku.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bdkerhao.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zifcamrl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2esuddlmd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2abnufwhu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qlufcwvt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rrboyfar.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2kzxdlhfj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nnjnpcue.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2opnknzfo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qdiqgpvc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2henxqjbr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2yccixswj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2tltpedgt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2gtjmjhpo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2kfqrmall.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bsimvkbs.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2akrlzyts.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bjnttnxt.html


<!-- 参考信息 -->