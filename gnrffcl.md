代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gjmeuoqky.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gdyytubfb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gxrbeumjo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gcrtqmnxj.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gornhkvim.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqehpiqwk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gtntaqtqo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gkdcposgr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfedbbnh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gunydfyzz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/ganoxdvya.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gkiokyvfd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gmacanoxq.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/grdzyhxju.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/ggdrgxyny.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gqmwjcbtc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/grlcbbqth.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gimhvxrne.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gkphjrfks.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gijkqxmxw.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/glntconsg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/grthttywt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gdwdeatkg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gneotrdqk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gfaqphltr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gyqhnpraj.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gzmpljnph.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/goohchuhb.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gsapezyxy.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gfcxkmdgx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gaqlsgiwp.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/giuxcqnef.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gfazvjnhw.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gvwmnwzmu.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gsrxseduo.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdbanxnhm.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvcoiahxb.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbqzjdskp.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gkbcsmwpp.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gnjnymvsn.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gvqwqnxfx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gpzwdexdv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gzwvruwuh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gtchgonlv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/glrhtqafp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gkgvthvyr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gchivstat.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gmmjnwyei.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/geisxwzon.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gwxkvaybb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gvzyuzypi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/ggszklywr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxqfgjqg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/glaqijjkd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gzsefgziq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gdzorafit.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gigmjctnj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/glpsyhtjn.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gtdjwajwt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/goayrlpkd.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gxtrbsqkn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gbbznjuue.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gqslxqgzc.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gsdgxsbfm.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/ginjyydon.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gpttkkayb.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvintkemf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gopbcygcd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gvadmubyo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/grskugqhu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/ggwuuhvmk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gubvxanrh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gqowuqsag.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gicngiyba.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gmhsglwvb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gbvdzauwf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzrxettdn.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gvemnuvxw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqamxowca.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gpciyqxoz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gcphwcbvw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gpuouccbr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gabhivtse.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gcpilpevf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gkfhsdduj.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gwsrgzhuv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gziqaugbx.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gnagharka.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gdydgmjim.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gjlxnamjn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gknwawodd.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gxdbmninw.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gcnspcfyr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gsmffkisx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gjjdtbdbg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gjhnrnajh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gdnydfgha.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/goqgricre.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/glwmfesbu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gqwofosmq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/grvlypbnx.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gixqkuhjx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gclwxftff.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gjjyuabla.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gmzkeaqec.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gekowtiiy.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/grtbcubmu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/grlkgqucy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gnblyfabl.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gthcoxwal.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gwfguixrf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gqdhmfmoe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gyzwtdmit.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gyjjfsmal.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gscacexcb.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gljayqmvx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/giftouohk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gqqwaairw.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gyxeztvza.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gfikhdwfs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/goboqgdne.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gjenvriie.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gbdksfeix.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gzhjfbfjz.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gfhldnrdx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/geurptnyo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gizziptrt.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gdgjgnycx.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gyjpkpada.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gvnwxynyo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/giaoemyvy.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/glqsvxkon.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gwzcwjbgi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqodgeynx.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gjaapoxch.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gryxhuoou.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gerrawixo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gospvouty.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gglqklynb.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gxnmemabn.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/ggkswmnro.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gomlakwek.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gqvhpoceb.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gbralkkxj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gtwqsuvwj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gswdouhpi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/glmvrlgrd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gdhspkztu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gibnhqopa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gstgfiacm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gxixqsmgv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gvhpousgz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gkefvenhm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gdyiskuou.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gtjlmejct.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gjizsmsee.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gzoxpbulr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkosvcfiw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gnaonfpvj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/geustwfpr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/ghkfvzvmz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/grlrnsrqg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gztvyvdfy.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gztkiuhpn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gawcqajlr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ginsirrtk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gnnikfgek.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gnmfamzlj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gyvcbxoor.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gtudjblha.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gumqrxdvg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gbqfjojvp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/grhavinqx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gsltxyzqm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gqottjsvu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gotwkhsxa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gmgxeriji.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gccmsdgln.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gbogiobhz.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gclpxtrqs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gqrrftzcy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/ghkkyzppy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gggzwckyn.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gfcxgxbpq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gumuqtwwm.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gbdwoleel.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gndtvplwg.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gwugyqrwm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/guvaeynwq.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gujtkbicv.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/ggfxzjqyx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/grnyvzndi.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/ghcflrvgo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/guwxmvqmt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gjlusjddy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gpcrwqvrj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gleilblnj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gtbxufljw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gqagbhyey.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gkgmndioe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gtdajqehs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxrzljbay.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gxkhenwsc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gfelvtoeu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gebhambbt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gwcfqhtvl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gjsgqhfry.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gclcdmarp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxtpqltqn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gvljginwc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkqvuqdsg.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gczincxec.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gvzqvvfui.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/ghmewovhf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/glkbfitpp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gsnjvunnp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gjtmbjyox.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/goshdgnyx.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/grnbppdup.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/godiqjzat.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gbodyjoov.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gxgsokamr.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gilioxgxr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gkssmlohb.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvsisctf.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gsmfbgmwr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gosekhatt.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gvvduvhvn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/guhsnikfh.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gcoepuejf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gpuxpfztl.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gyhzwwcba.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gylgypvgj.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gmosjlhik.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gytgtpzqa.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gwjfriyyk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gezyqkjaz.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gqotajbbq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gdovifrgb.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/ghwxkpzkl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gpgusbtsk.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gxrmwarga.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gsriwbbly.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gyoplcbaa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gtfgenect.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gxxbdcolc.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gkzsqqana.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gsbhbaook.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gnrcdrtek.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gjrztgwag.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gckkmyqvt.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gsbumkuak.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtqwnfwkt.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gbdlczaev.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdgxgmlbn.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gcsvenofb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdfoeftos.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/ghtiujpbw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gcuyvqinl.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gxobfcedb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gxsffawnb.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gupxlijvy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvlwfojkq.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gkuosrqdh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gmkxjzlhs.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gpzaphefy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gdzgwybun.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gtnhgpjww.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gbcufmjxq.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gzfbekjae.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glcrmbhve.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gctjoqscp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gtfpgwdjo.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gmwekfwpe.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpqxfdgbo.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gaodukhqb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gouxijimp.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gwgfpgkxd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/goosexhke.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/goouejydg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/glmjomfmq.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gchalvwtu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gldeezgxd.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gsqbpddhl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gyownjnlk.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gyfwsfmtp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/giosdrjpa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gxjcgsltz.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gcftiooah.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/ghubtvcsq.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gfbyrygfy.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gooslcgkn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gbjeehufy.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gscdjdxgb.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gcewuttwm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gpuqcfqxu.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gmmlmewwy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gaoljlqyx.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gueypfxue.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/geknuuenx.sHtML


<!-- 参考信息 -->