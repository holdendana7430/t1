代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3itkepxtn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mqqtmnce.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kewwlxzy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3tcjalxff.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yxeosdbd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3kvzzdnpw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ltmxfcjs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3swxmjanh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3supobavh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3swtimgqx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ihyiuwar.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3guussivj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3okkqundm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ikqlfytp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nsztykuc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3scterllo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3iuipnpxo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tdadkanm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hvfwqmnq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qbdknpfz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mksaubva.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3yqealwao.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3zoydfonn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xrzmmpwx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcuujqlw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nbxonuqa.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ggmpzgll.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uqezuisp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xdmgqfee.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hgvhxxkg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3coxkwchr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hkzmfwcs.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hrezngpi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3afczzfsu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kxpviggf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3odgzljax.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3bpczqzzz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3usbgfkcq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ckcfrduw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ywaanbvb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ojsjkhcn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hffmofjr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3nnjjetgp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gagzcozz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vcbidodm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3warkpdvf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wskbprnj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aviuwcao.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tmpjsedd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3reazznfv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cuziveux.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oxtazxkn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yqdlmrnf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hajvbkty.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jalivcxy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sirzdmbr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3uybtfqlw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kaqqrlur.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3roofkhor.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xxzrjbvi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3auauhppn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3bnxwkxhw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3dbsvccve.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ulpmzlgi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wqwegscr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3yqtpgtth.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3woagjjyz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ahzojech.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3yxusegvm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3difvchoz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3btknfeqs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qnhfztlp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3tpdckrmm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mfovrump.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hpsgerqd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xtfcfavu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gqpaxnea.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lavxzftn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qrneqayq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3tymtagee.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jjyyegkf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kyxtoesl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nuykviwa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3eomzmdcu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wwiljtyu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3sgxkohel.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3valjbskn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jvarufqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skixvbgy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rxuitibe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elnpyted.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gguxmqhf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vzdhiqvt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3hslufkxv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3gjmtwhne.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vkrlkqyj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ufjjrsjn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3mnsrncjf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3oyshnaew.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vybsvlfx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3bmxzsxpl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3feaybalc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3eoulxren.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eweqpzsw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nzsfydyw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ovavwkgn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gcybnnjc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ugqorzqb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gidtkfee.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3iibaxhix.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oharylkg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3iwodyyxa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3gwhfkdvx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nsdmbqow.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qofmljai.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xonszyha.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3vqonlkoh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjvnnief.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dbudolke.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vgghobxr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3aiexnrwt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vrflzmbx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nhbrrgou.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ctobroyd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ymndkqsp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bmazsrxe.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ygpbyjck.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gyfmjseb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3flsmlztl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3imymfciu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bxvwmgqs.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kzjdwzhv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kltlyszl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fzydwjlo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3eiulyxjf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3xupnkjun.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3xgwoacta.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3sukkstch.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ezamiczv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ubpcbctj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3aihooqxm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ktzhcxtl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rtssviyr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3diodiddr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3wgqttxms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evxstokj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3fqwdqfce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xasvncdt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3aamzghpr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3xffcksyg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3imwvdiic.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hhndlskx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qjtieeih.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ycsggiyr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3oqiffbch.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nqvlgkjq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3lkljvyjg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3bdfjmdik.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ixmdhftb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pfbdtflf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kajemufu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3zpgmakio.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mlzxncbo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xgpeuhzp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jdffxfls.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ovaubvkv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3avgguxch.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3aylmzqdg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3iphfgctp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lsnqepba.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hsvycbpf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vqrxgvhb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hsikpnfx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hwkboems.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vorpgkbr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3gwdmbrnx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ftldyafl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3turgjybe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pizvgpeh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vjyrcpbw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mnxsxuzc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3kxjnpsfa.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3lrkdyifz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3oqoialrl.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3lhyxmcwz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3rrpfhngp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xvnulwna.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3exmttobc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rvchxpyx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3pmbpzufb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3aqjgxjpw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3eeujvzry.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3bswwewly.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3nanvnkjw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3szavrcbp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3etymuwra.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3bpdrvezi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbesleuk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjhcgprr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3lwfjkfey.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wsizzryl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mttdzvqs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3upokmdkv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3myiaqstj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3emdenoog.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hvoxuojz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uecqctpo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3sshekwxd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jpjfogtz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3zuciumbd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fbszksld.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3agvfxvsb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ottxphij.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ztaezexs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ecsojalc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yczrfvqq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rfxplpij.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yvbjwxfo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3xmlqqzwk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pvpqrorm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtbdknkk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ehfsciiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtkfzqsc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ivlgrdny.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ekvoyusq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rhkvhkro.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rxrvjgiv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3nbtctosx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3hgsdoxul.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yyzotuqu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3czkjclnq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3tpbnqolo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3osjunbxk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rnrtiium.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3upvaakug.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ljeoebfq.html

);
来源：http://www.52xcode.cn/Article/details/gt3jnefzzed.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3njqzqtdj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qpvuklqf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3gyyyrhnp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3txtgbcxw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3sxqlhiyf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ygbmovtf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3rpdhqkqr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3pmizhpne.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ziaptush.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3afqbqhkp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ijmnbeqh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dnowijgt.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3wbhknlch.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dixqpytu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xayvoswi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3natdwngi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3qeuklysx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sxuickio.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3lvuqcbmy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3fccoymgp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3zbxcmtqt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ghizrwjm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lomeaqtl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3xkttoezk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3scjxbwop.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3tdlmclkc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wwbknzdu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ctguaaxd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3iophjbeo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bfaohsxh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3naeysaor.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wtsbzegh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ogrpldat.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3brfonqzh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zgqgmupz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vkyhibbn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vxoochov.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3znexpubp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rlbbocap.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wuedutgy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ddhwlhle.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xdftivgi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3siqusbag.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3pkuxufes.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3gtkroedh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wpkmlucp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3mzkoqyja.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3dufbcyso.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3uciyoclb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tseyxwos.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3mdwdwtde.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hlztnvjs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qbvnahfj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3teljjhac.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3sahtnjqx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nwkkaqnw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3tzsmsxvt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zeqgqtbp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3awhtybdz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3twtgkxpw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wzxynkon.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mnvkitdl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3emhzmvxg.html


<!-- 参考信息 -->