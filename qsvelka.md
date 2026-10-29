代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gfcqdmtih.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gduciqmia.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gastehrhb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gxgvyqxzw.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gkpotdgik.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gvsopqtef.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/glhezydme.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gyvddopjt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gcmhphehr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gnykfljlw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gkskkudpk.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gejujlsdb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/goacpqhpo.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmdipfszh.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gixdrvjyt.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gvxnvvzkw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gcbrkiuqm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gohtklkor.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gsdsfpgqp.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gmpewzjim.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gmsmnngdk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gnnyuuyow.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gspsdcheg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gzhqkhrcy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/grdiwagzx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/ggzmarzhp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gcbsnfvgz.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/grehdajxj.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/ghgguevql.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gkcdenyel.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gcefohljr.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/geanrbfcr.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gaqfchdju.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gnztcalmx.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmzuofhwq.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/glcwfzraw.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkoopkipe.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsgurwjut.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/ghoabxles.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/giaheipfm.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/ggbvqqlfx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gpcddbgqz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/ghjfunzcs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gmnspcmiw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gaiaigssd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gfdcrgotj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gfjmvchml.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gjfuwuwis.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gavtjcxsh.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/grobwbabx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gwukdmtvs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gnawpgwsf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gqaligkeu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gdkesiizq.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gtdnmzrfy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gsohdiajo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gbkqtyxuz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/grkcirnpl.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/guaepitez.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gwgmjouqd.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gcnjoupun.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gznvuzzoj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gfionmrlp.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gjedaegub.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gubkglmgr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gkwpimybf.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gctdedkgh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/giqfvqgkv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/ggafhjjdq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gumarmhsy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gevrhzhjk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gzhzlrvom.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gehvruaaj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gwnrnzemg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gkiglzlga.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gaoftcwsr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdhpttfwd.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/geoesnjem.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnhmkjfxu.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gxsoswrgb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/ghryvzneu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/glweqjvrq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gibbdvhpb.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gvjjsiimk.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gohkaedjy.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/goiyckoim.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/ghstvblwp.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gqsgycizq.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gnphdgpfc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gajvfjgwr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/geveirmhj.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gxaybgdkw.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gdermksxq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/goaiqfmde.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gsicbipwj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gvzlitmhc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gdzqburbg.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gmtyhtuqh.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gvnbavmkk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gkgutxrhp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gvfzjoiwl.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/grdmldtrg.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gntluyzfv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gcuyizflv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gmfysscpz.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gvdrzhtgf.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gmwezsbyg.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gaetgzssh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/ghwldxrnl.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gkuiubsbn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gxxuqmmaf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gefqozufq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gpidzbpli.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gdiwirnwz.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gozonpvmc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gkqxsvxqo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gttzjladk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gtpdqrqjc.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gjvwbgmdm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gtlttenfa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gifhotjfd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gpbghnavi.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gsdyypvqh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gzhtpyxga.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gjjzzrsnr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/givzdyptw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gcirnoukw.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gfzhkjxov.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gspsdrcqv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gktlfgwjg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gtjosrztf.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gnddlgvpi.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/ggnjxhadv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gudcvaghy.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gxgbsrqek.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gheonjogb.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gxjonkbjj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/giznkqafe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gvuyekrpv.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gcdtmhqyv.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gfxpsvzzf.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gxuspotgn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gowoubgmn.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gyzzdyyzy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/ghkawomon.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gyddedxlb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gqgmlznle.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gdukpwraw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gshsudrcv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/guroztwoj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/ggmxqxakd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gwzidwbjk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gmsstzfwh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gnlezvnin.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gkbkcmxvj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/galfatbst.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gdxgcohim.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gbisgbsyc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gesbgvxbx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/glkxicvnv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gadytgklv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gxwxbbchl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gizzjqzkg.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gtfljizrz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gmaccrwsu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gwarnxapo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/grscekffb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gbjpdfbvy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gurzlgsgr.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/goppucyro.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/giweupiiv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/grutdwkga.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gpwaqdmkt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gsyqqiqqt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/ggognmxlb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gfarilbzc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gdsfndqqx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gcllsbpqm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gtludqbbx.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gujgukldd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gqvtrvhbp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gvfnunedw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gkcgddccv.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gtywhfvbi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gtxmpvjdh.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gmkdsysbr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gzhpynhzz.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gihaontju.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gkgtijxbh.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gujjkoxks.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gzymwdqbr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gesxaaepm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gdrewmrmb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gubrcmjky.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gxqktarrn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/grrhmfrzf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gnkxsuzvl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gyodkdsrp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gheqitvga.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gpioxyvpz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gjzunlwzt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gqtejpaku.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/grtocrudg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gjhilqsdp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gkldwqvgp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gdvzjqkxo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gexvkugug.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gnerwyjgr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwalodxmm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gvvagnuip.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmncmfalk.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gzwprhnwd.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gryvctecl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gqtolnufo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gquzkpgor.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gbrtiaoyf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gaweakzln.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gfannubjj.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gqdcqgnpl.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gfiezmpqd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gsytrkyqz.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gtczmfqma.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gstoapcqb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gpzbvjbua.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gxvzfawhk.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gbzairdov.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gmtdygnub.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gubcvmmgv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gzvwtxsrd.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gvyfxttyl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gwrfesgep.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gukrwqxjw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gfmbgnixq.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gmpsjiyxy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/ggqcyxqst.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/ghzdgvsoa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gdxbucxiu.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gskmzwgfb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/ggojwxhwg.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gmkpqleeb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gsfrozquo.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gbiyzhpdr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gzgdgsadd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gibnrhwrn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gqfpnpnby.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gekeoyyei.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/guonrmwid.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gauzjxujs.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gtcsdvyjw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gjtfvqseh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gfxnxgoaa.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gdjmxtgqp.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gjyknzzpd.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gkiduolco.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gahxxjqbk.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gcurfbhmt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gyzmxeeql.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gddiasuqo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gugndfabj.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gqfgfsdck.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gogdorqnn.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/ghsbftvsm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gcapboxoe.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/glcecxtph.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gwlfubvji.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gqnarajnm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gddrkwecb.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/grtorcjxj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gkhupofne.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gwpsvkjcf.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggyosflkc.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gxhfzaiqy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gokpqqwrc.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gtokdlaey.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gldsipift.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gtmpgqljt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyhohminm.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gyhnneuqi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfpqqqlvl.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/ggpthcmjg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggcghkkqe.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gmfouukew.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gjclgbauw.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gfwmazoqo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gyhyfmbpt.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/giwwelabf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gjfkrikbp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/ggvuppdih.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gtcndjkbv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gblbdprxx.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gzhsuwyzj.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/ggvgqivao.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gbjwzwqzu.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gpxznmwps.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gjkygbtex.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gpxhiklhf.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gpevaftrf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gngfxzznh.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gpvuuctyb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gzyauzifs.sHtML


<!-- 参考信息 -->