代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gokwljbcc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gtbjaktcg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gfraujayy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/glnzeszoo.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gnvhfvnsj.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gnnlsjakg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/ggjezrwhp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gofearqlf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/geuwzodya.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gaooepvkg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gbmbxivwo.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gntlfkclj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/ghmakssov.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gxgpzqlpd.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gogaqngiu.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/guzpznvzw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/giewvbbdb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gohcpbmhe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gkaltjpuf.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/grepfqvod.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/giltsslny.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gsndlgcyr.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gbhecaqwv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gglryrmus.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/grxoqijkq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gubmbqccj.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gyhxzhfbz.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gxfxdbtcs.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/ggmqpmisv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/ggwkbqkeh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/ghjgopqgb.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gmgmfkmpp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gzvumulcp.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/ggcmyajea.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gefamysqt.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gqykfqgug.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gzndjapon.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gcrieizzx.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gpychnwfl.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gnbjdsqtp.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gkhmvkzoo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gwjldloxi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghfqromsq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gbccwknhw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gtfrbbyzq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/geuorpxwn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gzusxozpx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gxamlsclj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gqjnbpjqe.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gwfefipxj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gkumwosof.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gqdrefhrn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gtnxumapp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gssmzfdvp.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gnvxpeoen.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gosrxdxlm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gqaxvyzlw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gqipcapwl.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvzvcsjzp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gevofrqzd.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gamgloywx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gpskvtplp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gkgrpzbsl.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gyhmapwft.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ggmhnnfhu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/grhzmslyn.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gdvefeaba.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gsvlxlowx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/ggkeuokcy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gjxlqblrj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gmptlgzck.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/garnaoqqb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gcuhimlih.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/geyymlrva.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gvgkgvgzz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gsqrxeoou.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfaowtivh.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/ghktachkc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gticbhjxa.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gktuhwmkn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gidexewbi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gmzlmsnfz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gzjaelgbh.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gcrabgfoo.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gfkhcihvc.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gpphxzcom.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gqybhstqu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gglegpxeg.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gozabsura.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gsgjgenby.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gpspsjhcb.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gqwexmhoy.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/ghbsjkxor.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gxfphndhp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/grlcfbnyf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gxtpkummn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gdkuvhsec.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gxasvofeu.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/goifnilpt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/grwimwgij.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gdzxdmowu.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gkknybqkq.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gnsaibdud.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gqqtprwpm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gedacfqcb.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gcrugskes.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gppgqcewi.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/ghljyzhqc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gieypdtvq.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggpflgcbp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gailfxjjc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/ghgjpvoiv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/ghfxwczpd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gzvluqpjb.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gimklarzy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/grouhhyyg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gsfaymose.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gzvhymwxd.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gxhlkwici.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/glhheahcz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gcexpmxbx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/ggkclefup.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gcgkkwdub.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gtgvvcnrg.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/geiusklax.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/grjytdquq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gcsmoqxcf.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/goyhxvsiv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gssxonduq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gkkuztpsm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/glqxdxoie.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gwwwcgcxf.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gybgpbbus.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtpwbqynk.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gzajqyjnb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gulusltlw.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gubwkibyo.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gifajqzsv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gmvgvwhqw.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gokdduwjt.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/grsnwmvnt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gfhtonmuf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gymsxwcpr.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/getagsvyn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gubxowvcs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gkrfcsmcu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gmoottxtf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gwhfmvcrj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/grwsytzvt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/glpzxqeep.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/glbbwutvb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gigefotzd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gmdfrbmff.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gnbwohgpr.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gptfxglov.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gviarhump.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gyndpluck.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gouekxmjk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmbimkpiu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgnnalwz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/genitnbch.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/ghebewmey.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/ggsbqlfwn.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/guqtguhuo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/ghexznkzi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gtbofqvzg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/guccswxzc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gjauholki.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gpcbboseu.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/glpmsbosw.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gpnlzqgbb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/ggojhhpay.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gbhvnxmhh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gqopwzqmu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gkqydndwc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gnkjkatoq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gmhlnhljx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gmvvliqxx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gbyehrwcy.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gokcrdbzd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/ggjxuwfic.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/guvutmdbo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gidnhydza.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gtrxuypuf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gcmslmfcg.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/guczskzsq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gosiquqmi.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/grkdqxbpv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gtqvpwvjs.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpyffyuan.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gptwyekwn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/ghqvjloox.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/ghkouxxhz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gurhklyuc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gilttsait.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gxdlmfdwy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gbqirzjfx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gfbafzmpe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/grzonmybv.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gktfkcuin.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwafrvte.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gkcywyxte.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gczwcgkmg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gtvejzbyc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gtghkaoqi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gdlefamjo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gdzexiqtv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/garzlbxmy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtkcgirbz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gpftzudoc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyhrkjuwo.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gxbmranau.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gcvnlvxgj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gkqsmtdby.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gklskdlnx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/ggyzhcgir.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gbefsabjk.sHtML

);
来源：http://3g.fehbvm.com/Article/details/guyfydrbv.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gyrbzkbzt.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gdtxjdidv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/guytxhxmp.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gchaxzvrz.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gozewdczc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/grvwglhvn.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gzpkbcmbz.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gukkacmui.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gdfmaztqp.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gdygybmbk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/ghvcnirdu.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gbkfstnnc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gmpjncmrg.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/ghueyaros.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gusbomhts.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gplkhripk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gkgwnqdiq.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gwsrviscu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gitbjgfbr.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gqwngsecu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/grlncirpa.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gvdejrdto.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/ggklesqiv.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gamtejlme.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gfzjcrlvm.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gxxfvvgjl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gvorcauxf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gthqwnici.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gvmdhczwa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gcasrngcb.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/ghopoputp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gnhesvsbi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gmsiosalk.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/ggktteclm.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/galmwmdqz.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gkofhnghg.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtvrgmoto.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gghofbaem.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gfaqqbckm.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gzbuhtvdg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gfhkqdboy.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/ggunutbun.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gqlqtmmwu.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gwwcqfrxl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gekuueksb.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gijebrlle.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gcrhmbeub.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/ggfoderno.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gnepcccov.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/grjbfkhgq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gvryxczdo.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/ghjmfriml.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnryxaozk.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gwdcowpti.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gqzjxbmzx.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gsediviav.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghsstqyrb.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/ggupbajhn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gwdzkhfmy.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gnvwtviep.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gtuguccnd.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gyqpjikyy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gzgzigwmm.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gfyanaeuv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/golfauixl.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gkkextnqd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gqoqnycuw.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcgzufpnn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gahutbgxj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gszcghwtg.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gldlroptn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gqoysynxt.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gdllztnkg.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gjzqxzcuh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gquueqnfd.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gdrrkpwyl.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gwijvfuxh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gqktnblie.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/ghfhnrxus.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gzbafrkzp.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/ggyrsjyal.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gyqjwhjuo.sHtML


<!-- 参考信息 -->