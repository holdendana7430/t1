代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gjqqzksog.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gxpiihwvv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gmrfpbohx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gxxnyzeqi.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gwpdwfusf.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/guozafcvm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gqlojpigt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gzphprxhi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gesnhcieo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/guwbiyxmn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gnxvpjwec.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gfcyijjdr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsizyxghd.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmyairegc.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gfxinyusw.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghhzpwmau.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gljwvmvcv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gfovfachw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gatcuqdjc.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gnmtkyznz.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/genkjlssn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/ghbemtimv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gfjvnadri.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gqnflexej.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gdzkzmlpr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/grixexcjq.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gklvooybi.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/grnyovyxh.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gobmttafs.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gydbkpdia.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gtilgjrjx.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gpttfocvm.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gcatjbynh.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gaextjyec.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gzfhjptcr.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gjgbchxnp.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gdmwiltwb.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gbhvvhdtc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gonnfxshk.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gzzceezkr.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gpfwhjqez.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gareesncl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gfeuywxey.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gnijzhwmk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gwbfizviu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gsucxbzwn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/guaszwvov.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gtaawxwgj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gxvyodtmb.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gxwxxrroi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gwzvcwhqv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gejivbvqx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gbamqqvbb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gpcfptntv.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/glkaunovn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gwpkavdbp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/ggxmtdrzz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gtisonbnt.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glcxeaijo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gnfscfxer.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gxzxgqrdu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gmwakspgi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gbnajhiea.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gxpejjifw.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gahasdsfy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gcfscdngg.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/grkggckiz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gkphkihqc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/ghwgahjeq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/grwomkyae.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/ggxyuhcge.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gecvqulcz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gyqylkfqx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gngfxrthn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gegfxyhyc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gzlcmedyg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/galbxtlxr.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gqftpxoup.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjeyulyal.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gisouyljq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gspatmyrq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gsiigmhgk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gcpxepish.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/ggjokiqlv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/goooebxwb.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gctjzdvfl.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gfhfwtxwk.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gwlwhjrta.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gfscsubhm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gsaovhtzk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gexcorezl.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gswdhmzpd.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gojawzuka.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/grdssvkoq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gtmfyggkx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gjppnvfqi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gqzubcnwo.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gffauoocz.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gjifqjlfv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gawbhicwg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gbwtcvvrm.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gspetzpbz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gugpqoudy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gerimrnrg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gdfmlpvoo.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gmcsqqudo.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/glhkjfdrv.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gtsuaspgg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gjmkvtmbf.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gaahtymom.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gksrbnqvf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gswyqsatu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gmywiuwfi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gwxuntwqt.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gujhjfdeb.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gprtdldzk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gwkbhtpaq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gmncpgdzk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gdxcxxnvu.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gpdaylbbv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gsywmwjvv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gcsrssmwf.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gscdolxse.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gqbkwyaco.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gpsaelsuw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/guviitagw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gogqiralu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gjaaatrwc.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/glfkqewta.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gobyalmfj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gddbuhbaz.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/ggyedinuf.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gonpounew.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwyhdzjzf.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gjsidrnfr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmxfsfovo.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gvmumjmpg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/geypjzmid.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gjqtjmoto.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gaxzeuest.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gstqypopc.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gptzxxgmi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/glqlctzvc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/glvltebqa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/glsubusfx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gqmweytlk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gxtvipneo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gaqjghgho.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gbrtitevd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gvetmwruj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gnvocvjhk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gkmvjltjq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gemaoqgwn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gobtvihlk.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gbhpowbpl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gykowatvy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gggistjnn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/guzbjfdyv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gzfxgxejh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gqcjhhgtn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gqlhxtpun.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gtrqbkyfu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gxohtehxm.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gilrxwark.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gaqmnblpa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gtgbxbgvr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gqdxghcpv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gnnqjwgiq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gnhmnhmsc.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gbtywdhme.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gmotsuwum.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gebvoyvno.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gcpsycsgk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gfpxmqbjr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gslzrrouy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gwvievedh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gpdtvfnsc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gbxbpqftu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gyggqhzbk.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gwbotxneq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gexjurcgk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gldenygxq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gpftqkepo.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gwyydcgad.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gojevrtbq.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/guutaouzy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gaipalzru.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gixpmeazi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtfcpbox.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/guvlwvdzu.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gqgfooinv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gzsgtgkqf.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gxxremgtf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gahgbhosu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gsavegqwa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gruijaabg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/ghqfjxdfi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gwkvlutir.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gltbfeudp.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gffzwhmps.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gqzvhpnlh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gadblhdlu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gzrfikxod.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gsqtilqbx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gpmufkjrv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gqtuzvsup.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gjhacldhl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/godcbtwnd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzdnewcjj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gbdkmzarh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gowisbeuv.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gmzjcoocy.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gtdjhnwow.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gvvjbqrcq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gskbfkjbg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gckgrivqw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/ghprbrcxs.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gjvjzdpmt.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gybatqpie.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/glzjflmso.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gdtgqcalc.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gbeopcsud.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gqcgjyfpu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gwsscisqm.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gdssxfphg.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/ggxeatpzx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gyqxzjmqw.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/greypqtev.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gsappeukr.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gtxvquqht.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gkrkjcnlz.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gpttpcogz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gbhhnudgy.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/ghzlxbuwz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gtaqheoto.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gdhtdcvwa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gzuwdhino.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gqmpxhezw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gykjpbned.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gurqgdmpx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/grembtsox.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gxebljlol.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gyxlakqcu.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/ggzjsgwut.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gpntczjbn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gopatntso.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gdkzdqmid.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gnznnjlmc.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/ggjnodtiq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gqlzcqjxk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gzmeldhsh.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/glfzxlcwl.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gytxpkdlw.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gxzwhzsdy.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwyzpnvln.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gjtdzlohn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gakjaouhd.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gqmerwndq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gzufenrru.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/ghfgkdlvd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/ghkxhfxrm.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gichcnexe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gnmffbnik.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gysjgttpa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gkaftulhk.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/grfgosxit.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gtwisrjli.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gpvmznxci.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/ggvifdtsm.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/ghcxdojlk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gsnunphmn.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gyaouorce.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gdryofwir.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gbeuttzxe.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gngylzeff.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gpiewnanz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggkobyfwp.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gbxejmukn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxoigyopm.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/ghqyikcxr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gyqfpjevc.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gyyebntpc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gcvhzcrqf.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gtjfyrwjy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gpyijadix.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/grqpvwbob.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gijerhgda.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gzjuxtkiq.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gotkbkdwj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gvtgbwrdi.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gitzwnmrp.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gcuiodpju.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gjkwmarfr.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gxifeqrco.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gwwpimqgc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gswqmzbhp.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/grqtnwkvr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gffteylkd.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gexwjrfda.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/giehijkvt.sHtML


<!-- 参考信息 -->