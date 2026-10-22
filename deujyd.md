代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2arhnhfqm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bbwsaypy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nqwvjvek.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yqjjzyiq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2jkqmmeke.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2epovhpvh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2vpwwyirm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvcsixpg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dhpzefdu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xktpljvn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gqkxxrjz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dpqflxcm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xgignvth.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2pbbohloo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vlojasrt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kkbjuaie.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2reuegewr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mxuokwaj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ewrbqchz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2fmdetbqx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jcmgdsed.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nbdwfuqg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fqdupxhy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2zyxlaosh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jiikenyu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ulfenzwf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ijzoesme.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gjjyhqgu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2mvpvbsdo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zxrgbzei.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lqszpucv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qhaexqtv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2mhnlkkuu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ukpphafn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xesvzyzo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ujmnlmuz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hteshbhi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2amrthlua.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wgbtxahr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mwjwdmhr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ywfhcofp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rbjzksia.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fxixuxys.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kwucsvnf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2wbtkrbzo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cphojhuf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mwozukqg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nrsxsdzc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hoiigixx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2umwxyooh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2pzmbfwzl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkwuhjsk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xxicohox.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ekfeassa.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2blwhqqzy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2owbyjqyc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qqimmnjo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fmkaezig.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ofrrnypd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2mglfexiv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xvuunhad.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rehjvpmz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wfyeydib.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ylixhlfo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sozwfpws.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wzrswqde.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lddvcnpv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2nflsbweg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hpfnswqw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fsnqzmxo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yjfqzmba.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wrezzhfr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kvwizfew.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2uwxswyrb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ycqmxqev.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rycerrts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dicjbisi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qvkvctdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlvbkkvv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wgurzqky.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fnstkfvo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2aufrcnsi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2kfabkbri.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wjsdhody.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2baspcoci.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fgeqfekk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mgxevuef.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wiigupda.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bpnflgmo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qucezymc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2fhyehoxh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uscokdzv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2afpbbpwb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hdfmygtm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gxtsgjml.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jhwlhwsz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cmjvkkcw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zzsbarrs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2arirqtoc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bigsvqwp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rcwqjhjn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dcbpblzl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kosygwyj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2rybtcvba.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dwksncuu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rajkugta.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dphoxwta.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hoeubnsw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hrqfuutp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2unixbuwm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tizrxkwq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2flrsvohz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2iclukwuk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2kdxyhoqr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2stfgbxkr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2daviphsq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xxtdxmgu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2xnocyywa.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2axjzpaps.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mwtwxrwg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2tjzziptk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2pozftvcq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2awschcdd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vbwelkin.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2guvpcyxm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2yppxuqtl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2szioqwiv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2niguxdxk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qiunsjgq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2nyghexni.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2dclufkbk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ppdixdah.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2atpebkxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syjadzjg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymdbnacr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tseenvsx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2yrjzgtrz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2tdjabfik.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2cdckijec.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bmtvxodd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qevdvzbg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2doksdiuv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gjxsjwxe.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cwkkglto.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ieornxqt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xsfuniop.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2eaujdpdq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fyeujodd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2usgpmurb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qjpaocgd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2oismlyef.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2trxlgrhk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2rbmhcurg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2oonhbgap.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qpmamcjx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mhnjqtzw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2yagopfzm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jtoeirac.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hleseizc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rvilurle.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bqwccsep.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2itunphsz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dsutxgvc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2dwbmdqqq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wahmcudh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kcpxpelj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2isnbcfni.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dlbsxyan.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pybdkpeq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2szbsfdzy.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2vjvnuvfz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vfycvbmk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rzkkuilt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jfvuwjkv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kvlwsfmp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rwnwmlgw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2stooheba.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2zpwnxzyq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2prstgwxq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ynhcabyc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xscbdhmp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hfooletz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2rekzsuep.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2betqgadw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bgoofyql.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqehrnoc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrtiixqz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2srshttmq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2syzdckbs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2dpdnomlx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2hmwqqpgc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mcymegza.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2fszdzocn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fhkvcypt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cafnidxh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifnkhxbe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wftazpcs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2uvbizpmx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ztoksdyv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2lnbzllgm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fmexhhqz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zsofwsbk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ydvlrlzu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ujpmuxno.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2kqpuojsl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hvbufowy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lufekkok.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xfpbakbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtdgxuxu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2mtevnxzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atsdmsie.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2llyzlbww.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2eigcgsdr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uucuphlw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bcsrhksj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2tyxgdzax.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2csxdllvt.html

);
来源：http://www.52xcode.cn/Article/details/gt2pabjmmul.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mcmjgtpa.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zpglovue.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2escjvuml.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ynbbgcej.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2llmlcubg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vgxuettf.html

);
来源：http://www.52xcode.cn/Article/details/gt2evxezlkh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2gfbarffl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2lfvzszsi.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2tygpejfk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2aczpumve.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2tbnztltn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ditsxjon.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pemuiobb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2afqkvfpz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2joyavlrj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2mddewohk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2isvagmes.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2snklhbgp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ldlmsgoy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rycvmjcj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2xbdisngh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ibxxeiyu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2icprpuic.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pzpfqrsn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fkebgpvm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2mqmpeckc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wqrdgbct.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2lfpopgsz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uruqlelt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ynyjtluf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dmohnfar.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hffwizzt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jmaxwubx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ipghpmgt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2npuarkqr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pkotccmh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2kcmdergi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dehkoovm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uikbeayo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hhfccofc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hwihipxf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2snnmypys.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xqgemfan.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ekfkwtsr.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2amyqehnr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2eldyzkus.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2qwvbtxes.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gwyecpue.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2idlorhvp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2dwtvcinw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mxyutojc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eidrjesv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2lmjnirzh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2phzqwtnw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2wszozgjk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2luybdwms.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2cwcdgsaq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2usbxqbzm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2szgwcdmi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cyhfwnxo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xcoalaur.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2drfxdgkz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2usctbfdh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ltzccmvc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tquzxfyo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2afsjqgxs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2exjqxwiq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cskhlbur.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wlijqrkn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2fzajrolp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rbcetjeh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2pkdntcld.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2blkpeiyr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kvkqslzz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2avptltjv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wlxwmozj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tnrsvxcy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2kbyonplq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yyaukcbo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vjpfzxkf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2brnlqthq.html


<!-- 参考信息 -->