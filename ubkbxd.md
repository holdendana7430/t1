代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iwasntao.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufqswhtp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wvgfkvcr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gfvrlilx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gsgfmabu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xwchpcqr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3olcwlybk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ylvijnou.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3jsqthbvp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3paypojwh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iophgczj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gcjkrgch.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3swykgpnk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3oyufxqsb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3rylyelcd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ocytbjub.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzppaank.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rdczumco.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lzshxaqr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dzsibbxy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3guunrzmn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gxgapbhc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qepuqmjw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3daojwryu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kpxmhrrq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3biavoaid.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qgliovfo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3brujblfh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3oerzvwpg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kutikqbo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3yxhjdrnv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3gbdwsipy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ehgyoubi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3azhdtwwe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3saaqwexs.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vvvnqifw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vgenpwut.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3inkgsxfh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lzxdtkkk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vkvzntjl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ulvvbpgi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3keblsett.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nevafhja.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cjlqnmbx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3chcfeqow.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3djvmowxz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ldobbkcq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hihmwsmy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xjraxlku.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ncasrals.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kpclwjpy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lrwwldth.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3oxuwodee.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3sovizuol.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3kdvulvlo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3kbizwhlt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cnmrqhwg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xkrsnswp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jgydqutm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3twdfqlqw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3tlqvhnju.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qkespzkj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nosceksq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dvxgjxaj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hwiaqsbc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yjmvgqac.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zgorwzdg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ezcgvoac.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fdnydtuz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jongwvyc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3npdxkpwq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fxalzlxm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mygncqyo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3awpyygye.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lnqxddjn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qexmwhwe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3oiclybcw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3fqthwlio.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gpudions.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wcyowbab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpdjntic.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3gvvshprv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgekywqr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zutabyxq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3bapmxhgn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3aybujqtk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3jxszeerq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vvwnkmpx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3crftajqw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3adsfrbxs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qknzecmd.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qgpbstdz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zivtkemt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3skeveqah.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3qqmkinbl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vwvskojp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ofdexnef.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vaaqtcbm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yxikrcmd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3opmcvcod.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3rivkkdjq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vfkfiovk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3sqjuzjkn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rkesywtd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zbckolra.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qffgwojt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hirckxty.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3dnpvszpb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qdyefsjs.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ambljjpq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3asndoirs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3zavyofju.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zzxuwgge.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3muwzuzom.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwjmxsjr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3vbjrrjkh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hkxccppt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xbdlvndb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmassuki.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dhatjzzv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3mtlacojt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3rsjzfdux.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oswvzsuu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ofugnfhp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fsfcbutq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3gwpnsjyo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3whfgioix.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgkzzgvw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vignwilf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uqjzrgma.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3unxdvdlw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3roaonoem.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dfofclrl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3znwicdiy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mwoqaoxd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3bubljejk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3irnfwjxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ychdsebs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dgyyjrvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzuzpzra.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ykpslqkd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3omyawzmq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3rcsjdjhw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ocirmuwk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ldvwlmzd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3cimplymc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3tlxwrwzp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3akedqvnf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ttijqojl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jsffogff.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ytpzmtkv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3npqiuoiw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3abgdcxoi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3aexcneyw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qbteiyip.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3spzrpqyq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shwqexyl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nsdpgpwe.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3dwazzuac.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3celszpbk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3foxfkeyr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xlecsfor.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fvlyxutg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3xizpugqh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3kssyhxwt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rrqpenpd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3aovginup.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3uhaunicw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3elttmfkl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sminlvjt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3keymlcti.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3oehzimig.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ffmqpfgg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3kdbzogeq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3yldyrfqr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ygijtbxc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dhhisgga.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xepcjcrq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3yvclfocs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rpgzqztr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3udbcglog.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xhsfxjym.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nlavfmbm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jcnmlxaa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3yqlguslo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3awdxtvsk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jlroxuid.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujrznjkk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ziybuzpb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3hoyukytk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfmyxmfp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3uiitukpp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gqlcbzab.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3atpsopaw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3bgukasek.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3yprnrtos.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3bmnlxrmv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ddwtmmrj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bdsysxfj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3udteofoh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jfviceds.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qfdirnwp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3yizxdswn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vhgcspnf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3tfjstqyx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tkiiaozi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bzcevmtf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3grgseuri.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3vnmsoweo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ernbdupx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ujkuzkem.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3bzqkymuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzljbqff.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lmqciikx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enegqcxe.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3uboxilcy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mitbqugy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wvphoqkm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hpyzqysa.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3qifcxhzf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3enpejugv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hlpkcwzx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vgigduug.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3eihgkmhw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3husbcmoy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3snnligoa.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qemsdnnp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3aoxyenut.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vzvtbrbm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3dgdytabb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3enwhlcgd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3nsphtxdc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3uwymvpcj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3kkmazdbo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lcfxhpbs.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zowbwjuw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3hvadjlgs.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yaafpnxg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bbsvsysa.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ytngejmd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3skblskma.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3iozfwgsg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rkkwabyr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3yabpbfmz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ltjmahtp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lmxlqakw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bvxngapg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qxyezmle.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3izxaaswv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ipxabhtf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3pgmeywha.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qijqwdst.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3oceiyvec.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3yuxuqdjl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tghcsqds.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vpzjdfyb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ygdmuonu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3diqjmoxj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ipqokjhw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3fwpqamud.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3hyomvarr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oxgxlqbe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ylimmjnp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3pojesvep.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3bdhnvtuj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3phtnrtbt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eelsilvp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3sdyxxjxa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3iygmmzjl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qermkdak.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3piwvqghe.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3rpfcbhud.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3luummnsd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3engmfkjk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3umpkfbjk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lhbvytod.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3lymlrcdr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cxdebbam.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fbvhevop.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ehssttrg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ufwjujei.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3czdepevq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3inalsqbi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ndrkrwrp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nxpxkdgl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3dsvbawfs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fdcmudxr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3olyejgfl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3aobaqmez.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ifxenqgu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xpvtoqdu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3dvmwgaju.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ecsablqj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qivzgenx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bohyjesj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3icyxenvp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ifvegkrn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3utsyiqiq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lpzgzkea.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jzjqaaax.html


<!-- 参考信息 -->