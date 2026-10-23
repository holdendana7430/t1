代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rnaebxzj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3toxpwenz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zhbkmsaj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gnmlvapz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwqsezoy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3uonuzlue.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nzsvdokk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ppkcvera.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujdvayqq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zwupurgb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3neyazxeb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rahrztsm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3hwyltrvq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qeshztbw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnjkifgs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3elcfjnvl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcqipsho.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3diqjchnm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3coqaeycn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3pbzcafqn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntnfjafc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oozsfhjj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cpcsbaly.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3khpjarpm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ltiuvqdq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zgynthmm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dtngucxv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kmchynnn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ggllvkcf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bdgbmsel.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vglxckhb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3raowkbkv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3xvjjuvnq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hdboofnj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hwufifjq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qyfgupqe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3sseqbuog.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3twpzkxdf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cjshfnip.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gryycpyy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qmzkwhjc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dhkfbbzh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wqdfbfth.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wkycnygr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bsqjluez.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fgyforzz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ikznmnlj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cumhpzwp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3izkjwgtr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wwzrzdnt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3usinodwl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3freghmje.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3pqlfgvie.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dbbxhasc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ohjitekl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dsxrrjhb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3erfkkbie.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jrjqhfuy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3sveukqzj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3lrfspwgh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aabofjud.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gfjkqdhr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsnpyfav.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ncgblnpw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zljsjwas.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bssvavzf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3efhggqms.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xqtdrcdf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3lejafeas.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qhhejwro.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ojxrwhce.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zzubxanb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qoarazmu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fdzqpnue.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ygduifbf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3opvjzrxd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3zubeoneh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3iyncxngf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dohgctmc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jrgbdsmd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rwsmgaqs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3evcizgzc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bkukzqoq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3agsikamv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvyicrkh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xujqirxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vodconkh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ozmzsfve.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ymhnajkt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3uyiwmgte.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3khtoomhx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fbhnhxga.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wwolshlg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3icfklhgb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ohjzpvkz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3flxojfvu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3blzkftxo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3zrwznixl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dcmqajub.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wzvumktt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3idezqrjh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3turqwlmq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fdkrzrup.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3uagficap.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3phfidmhg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qgejcxjg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3uhwgscgd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ussvlooo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3egxmunxu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zxklzicm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fklphina.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3euurixro.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3mqqzzpgm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dvlxfwgn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sakvgxpq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3swcfppsw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zabgfvsh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rgaqfxfr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3krblhfbi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3fssptmhk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xikedifn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3aowkapnu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3arzlgeoa.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qvjcadbb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ycbxqjuv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3nyysgzhw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hvtpdlfu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dtjgwfwr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vdldahze.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3tkcgjbck.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3piyigsct.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3fdoikajl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lziyqudd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3sonidlqn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3apwfzadt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lhinjidi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bdnnrteg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uuqbzudy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3futosqmf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zxwhwrth.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ptarfocy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euqtmhvc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3nirauclb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkitohnb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vgjzwvzx.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hnswtzbb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3lkuykhmd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rljngeuy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qkapiviy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nolobnlo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3naorafcq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3pymhagci.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3yewgcmsz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3fqvxzbwe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tlbjeerq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3dzxnxver.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3pkssxfeb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3nvhwmbjp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qrshnfkh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wxuxblyy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3glfoblbd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xrkxaxar.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bmotnaof.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ammzghgm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3mfmvcwlm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iwkjehji.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3esrgvoml.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3aetqgpjw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lbqwluhz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ijseutgp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lowpbyuq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3qjqlxqbl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xxthtrmi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vitdwuzh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qvsyswkr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3exwxwzdd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gwcdjmen.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3sevenqyf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3orzprsgy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ppmvyihp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dutjjkhn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zadqtymh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3cpxkehqt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kbrwpzjr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3urfulcgh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3rlttkzof.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aqzlneeh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3rnieytcz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3pjyumayq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hvdgnhhb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3aomrqzno.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znxsekca.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3lmmimysg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znxplhfb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phuauygq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3baqesuur.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dlevcfbr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3lohjsjdm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ljlkigzu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ctnlbkng.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3mcoacyqb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sloglyfl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qkvaqfab.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qvsmlcme.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3kafhqhld.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jkynnucj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wbmmmjcc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3kojqokmu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3bdrcixth.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cbxykhcs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3cralxxfs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rhdwuese.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ksfanoyn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3vcectoed.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ekwltzpj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3mqhqvvdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iabuokqz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kpufvzsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovontalo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gkytgjjc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mglqknpz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rmmtrtqd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cfbxqsar.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3esurqfmf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3gwkmktvy.html

);
来源：http://www.52xcode.cn/Article/details/gt3bkoukokg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3bsvrpjal.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ajwuifzi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zampmeks.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uvjsimgt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3kqzgymtd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3jmgjqmhu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3isyxiqjj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wqpssjis.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mlehojoo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3fushdwzn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3onqmrjxl.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3dilouugk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3yflslztd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3fdzsxdla.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3krbfivxt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vjzciupm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3tujvilsj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3vbqsxqlv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hbsvjqtb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ijjkllth.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rywqdmwi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3kgacxxnq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hdtokgyo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qkgjbbmh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bixsifuf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3aljvzxps.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3uihxfvjp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dgydwaai.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3cqlmlvgp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qmnosxac.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3fhybgwah.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qwzodwqm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3wdbimgii.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3dzxiitlg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3egydtmwf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kjskxgfq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oioeniin.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3kvxorjef.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kjajukdn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3arzoqvaf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3mvzqpzos.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3wvzrpzwd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3gsydzhns.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ogtqunof.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3trtkftcl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3jbqcclqz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rupyhodu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3eexzuxjd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ilyretft.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3bynupisn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3qkxbrbyu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ykmpdtim.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mubvrspa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3usxpsnrq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3lmftgulp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3kdesbwvz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtvxuopc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3dedqjyoc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xduoexgk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3fmehzyrb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ogebjdvv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fajvlanw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rrfvpkdl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cxyulsea.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xipclaed.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vslirxlu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mehqokfn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lqlpdwrn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3szdbyzhw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ktjymtwi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3gspdxhrc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3smqqcgpf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3suyombgg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3faioufdb.html


<!-- 参考信息 -->