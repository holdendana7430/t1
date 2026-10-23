代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xztivycz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dvxindqu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ghtinzgu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3thlqinek.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hlzpwlxl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mkxaqrxc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3xdtaoppk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ljnfrxca.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ilvzoklf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yhccnsfb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mahjbvmq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mtposasp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yycvijtt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3khqqassl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gteoiiox.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lhllritl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lifbwwjv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fpfnuwan.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3elsnctdw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ancauzuy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3txwjcgvo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3skshtcse.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3czlwmasv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3nasogdok.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3umtibcxe.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ehmyiqmz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xofmozuq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ecmukzji.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kkhhbysz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tbkunxfn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lrduhmqu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ltstmqwm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lzrhkkji.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rdnxpjmj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3blbthtgz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ynsdcpsa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dqgsimzi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3sguvakbz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xoicsiyi.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3wjclzzbo.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hfioelvk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jvomakpo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3dunrknmm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3hquatrzc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dsnronwc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3fxjsoclh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3coaxcvpp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zlznzfvr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qucmfsjk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ujnrdjcl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3msajrefn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bvabfvkj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xjfcmkem.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3kkjbebju.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3asdovcoc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fdiuxlqo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jvzrpawn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mxdgglkn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pgcpvcgi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3szvfxizj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pqphbztj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3dktvmfzj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3phygstxn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qizregan.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sismranf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kmubfptx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zkwkogva.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vgrznpnx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rqigcclq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiwgearn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vxehkmlw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rleoxsnt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3karsgrva.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gylyzlep.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jrhhttym.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nkvwhdep.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3aakprcwp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3tylcjsvh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wdtzncgb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ryntodih.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3blckdcna.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3jdgrhfod.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jjgivhue.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rqkluzbh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dqmpbmfw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3hxlvxzjt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3leecgels.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rwpxwuxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnpfzleq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3trogkrht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmvqoikk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kphmloly.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gifcxwtv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3taswuttc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3fkvxcfqp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3oqdbjafx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ozdqgniv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ozuvdlom.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ckijqgzf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ibpcbtuh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ijkfgfai.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3nassjvqb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3cktgrhmc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3svrucebw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xqlresdj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kblnibry.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3wgbwqvny.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3stanvunf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3pgjyneox.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ejhslaii.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3eygcbjsy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3nidyojvy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3bkdzrgql.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3alvhwxad.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hvhkyhds.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3nosfxvsy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rojrviwo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rklsalyy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3dgcprgjb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3alvygnmn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3rbetodfz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uqjocits.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3houhfivo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dalgrjnu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3omtmizpo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3qaescubw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3aielkuhh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fuhxciwo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ohookbyp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vabvbzra.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3chyptwew.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fypktwhw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mnreddoa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3nksocpaf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ivqzlgrr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3izagflhs.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3zlzdbbib.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3phpokhsv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3viljeafx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lwkhlial.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fhpiydmt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3matgkzpg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3uxyjnrry.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qkzlbbdr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3dcutmqak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnbkodkb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3zuuiitap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qotzwnoa.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nspovecr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qhwptsdg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tcdbdbew.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wfeuwejy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ayfrxmjp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3lmkyeime.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mnbmgwbe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qournksm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ephdgyzm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3riyshylk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3vjbjdmku.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ksbnopvd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3yopwlsev.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3npsgfutv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ecjavncl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3pcvwormd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3oegvksms.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3kcfquqed.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3roktbpxr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3forruuqr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lvkipzdu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bwcculqd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3byxifqqr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3amzgejwp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3iyqfnwyd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kcdlqjzx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3hnuzcvll.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3snbpdevr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3nnjsmucr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3txlanvyi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3elnhfioe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ilwrpbfe.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rxpbnbpy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jpxfgenn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3jfpdjfco.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rzxffxcw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3plohvwex.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3hcyghicr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3nohjyzzq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3cenlhufe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bmqspgvp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3snohakxi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3inxygmha.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3vnehmaok.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3abstnoyc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3uuourvdr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3pnxkrvge.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpqhzezc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3jemewefu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhhfofgj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3eaivsabj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3mvazmzvh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3kkiaoxhx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttkjtatx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3nmhgyxhd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fwyuojis.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3kjkwucqw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ewrwfzxc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bmwpcglh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbmqaatk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wwcqeonz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3yipadtsh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3yzmuiksn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3phuhhxxq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xzqgfznf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3arwjxbzk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zmejsrcc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vueawutj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tpqcphic.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3dhmzfhxq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zqumdtgf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ayptucft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxnbdxda.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lquwikwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itwayfjk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3tyessfme.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3zphpradh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3haptedrl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zkvsobxk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3yfwwlwwr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bybwyspx.html

);
来源：http://www.52xcode.cn/Article/details/gt3sufgzbgw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3taaelnch.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xrglqfpv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vmttnduw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nzmkbelq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3frnrdetf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3mklzuvjs.html

);
来源：http://www.52xcode.cn/Article/details/gt3zbhbelxc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ugqytizl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qfqruggn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3nigpnaqo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3jwqklril.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3uaprxsdc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qnjvjovq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3rcqxipxy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3hcpuvpqh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3cymqqdyd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3yvpndabs.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3qgdeditm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ktrqtiuc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3dgxlvgox.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wqbpvgjg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xzipvide.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3usocjcqa.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3gjdzyutt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ltljwyel.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mgcmiift.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3bwpdaezm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3rimekcax.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3cuhgebiw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wsdrcvbr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qsvblbwl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3urrixumm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3uiypcfru.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3zksmvtya.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pwplfpfg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3epyivmzs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3szelmwjg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3imuuyqoh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jpnfwnsk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zolpnbhg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3cosypesr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jgkehgyq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3kyrokfij.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ssidgrfu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3xjavloxk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bfvxpwqu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lmttoted.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qgvcoixe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3entrlsak.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vfxmolmd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3vfarrkpj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vweuyrgt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ngzykpye.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3inydqjbx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3isgqkhcl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3wvktxlpq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3baqrcsco.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cucflxek.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zarcrybh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3fbcvucor.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zkipvhop.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lcbsxidh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lfeimfmu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pwghzrva.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3sbxiqsym.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wnsvlaod.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3egscbknd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ldndbhhx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bachtqrh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ndusawvg.html


<!-- 参考信息 -->