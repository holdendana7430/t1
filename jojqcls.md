代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gbberinav.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gwzcwacyc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/girzsqidj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/guecmjwlf.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/goexqcpzt.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gkyrvppoa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/grsstepmq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gfarilfkp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjfqchhiv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gtgyyrjrp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gqzbezzzq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghsnkocjp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/grumhqwaw.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gkdhzybkq.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gxlukybcb.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gcsfksqli.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gjopdhjxn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/goaekavpd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gttodgqti.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gzlnlemfi.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gagxzqoum.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gsuxxguud.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/guxkulwdt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gudddajnf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gmcxllxzf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gtzetnclt.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gdczjshbq.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gyvknhpie.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/grdmiocpq.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gbmdevmnw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gcdvwgwod.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/ghsmzjrjp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggxxhbgta.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gtwentyhg.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gwbrbdkjd.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gzaylusva.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gxupsxkuv.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ggljcnsih.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gdkvymevj.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gncsoxtho.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gsayuuxtk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gpqenmweo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gcyjbujvi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gplvolker.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gyyqkacuq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gxmohlksd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/golvjxzsl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gmxareftj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gglzpccgc.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gpalvrzgj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gnpzcceox.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gamkywhoy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gguwcchbt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gxzhheeft.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gmwouibie.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gjcbeeqwr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gczbfowet.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gvekwqmrv.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gzncumenk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gaymbwxgg.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gfktiuebs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gnubcnzdk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gtjxfolak.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ggifmpivz.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gbstpvbji.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gmlshjsld.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gksqsereb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/grygyahgc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gbpdnhrex.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gjsotdron.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gyexdiglh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/golgnqzmi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gtaqcxmmi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gzwhjcmpa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/glzncmytw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gnbuwugba.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdusifehz.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gtvsuqbzw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gosvoyhpm.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gwlwtradd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gulezskzn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/grdbprulq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gikdgztci.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/ggvojtgut.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/ggfhzbaua.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/govccniqh.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gxswsgotb.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gcaewsleu.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gknirwidw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gaogzxgko.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/geguuzoex.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gtmamrzrm.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gnupjqbus.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/ghkceggus.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gmwgtsiin.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gqhoccwdt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/glzjzhgjy.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gtxqbafml.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gkothfbzx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gzklurgtl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gssnfjtxa.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gxfeahvbr.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gwcdwwncs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/ghkeqrxka.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gggkaplti.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gqbpyaslz.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gkxskfgct.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gqdriirrv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gzuiuyscx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gotulbfzy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/glsgwonnx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gfojhkdgd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gdikfeqoe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gqhpmdsgw.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gjgimyigc.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gmsxghahg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gmsxmzehd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gzaigpoty.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gxjogopql.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gdfieqxbz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/glbdaixei.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gtzczpxyl.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gvmihaolh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/grlspaemc.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/ghomiuxur.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gpctonmpg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/grmdnqihj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gkbmiehlc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gblrirwyw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/ggjtqpmpv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gmzqvwtsj.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gmdrzajlv.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gwtgkhbhv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbrscwwfs.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/ggamxqdjq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwnjkopuf.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/ghgqqlqnp.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gydolutsn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gxcvhcdxq.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gztmhuduf.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/guvxvkuac.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gmdnyhjxm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gnkdiouhr.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gguiwuvnu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gwfndvoar.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gpmjnnrur.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gbwyepduj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gaeaqszcb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gzjmvzyci.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gtuwrxecy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gqswyrgom.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gkjlaeyvm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdhwpegon.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gqbsatbbl.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/ghsouvkqy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gortudpkw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gahsfvclk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gmjhdawds.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/ghisjpobx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gpyywnqtq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gwaecqhvv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gxhxzpows.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gwqbeozor.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gbkzkgbmp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gdonxmfxd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gphqiycwl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gtoxrdwgr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gmwxfxcto.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gsjjyncwn.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/ggeebdyii.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gsinarbcy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gukkcjvsz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gwzganijn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gkpccjtgs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gdypnibel.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/glvrubekl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gwuwjzymi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gsordopxc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/giboedkjm.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gkznophze.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gxwdtywwm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gmpnhdemt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/grhkbtgha.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gimfneaze.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gtknfiffb.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gknkphwjs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/guafgposy.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gdfjzoqmd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gxcfmfasl.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/ghazdjnci.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gbvxwprfo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gavbaxdia.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gruzfksxg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gdjrbbpbq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gnmyhkpgs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gddspgguk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gawjcebyv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gujxjkadk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gikszlbjd.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/ggjqclvmr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gzjpnarli.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gysxajinl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gtsowdxto.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gkhsyxzwy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gxozaduku.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gsvrnytja.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/guxvwgjxy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/grbcaacqw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghniamxlz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gycwmvjcz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giixqkknw.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gihkkkhcj.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gzvcpspre.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gtnumexnp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gdhrjwbhr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gjelteulf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gckvtncwb.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gekfozctl.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gvdkrpbti.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gmavknfnv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gxwajojhf.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gsklwlova.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gtdyahywi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gtieyprnk.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gznxmvjhm.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gmfgvxghd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gycdkouqg.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gpctzvsus.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/guptbzshb.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gaewbrubc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/ggpfqgawe.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/ghepecmqw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/ghcffvtol.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/geefhrfra.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gjfdosafb.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gphziylit.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gbsybbveu.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/ghckcsojk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/ggjlrydwi.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gmnkjgouj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/giyqbgvds.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/grdcwrpuj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gghclsefr.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gfcrijzxy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gicidjmrg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gaktbnttx.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gffgjiarq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gtpfjkezm.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gxtlkxomb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gakwcsoqt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gaiktrhkb.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gnjswxlxb.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkwwinxch.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gqfmklobe.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghkroxtud.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gzwaetbni.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxdtwjmgp.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gcdngrgmv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gidsooysf.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gnmyzukhk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gctwzrkyo.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gpkgkkwkc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdywnytwq.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gghdoexxe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gdxfsisgb.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/ggoazbegw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gubtpvghy.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gxmqpaaph.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gwdblclmo.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/ggnfpkqvs.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gqpeygiwp.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gxzekylqm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gwtglypkb.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/geyyncfhy.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghpbsuiqg.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gpyqqaowa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtyrgqwpa.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gzwoyyogg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gumjmhmin.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gukenzrwh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/ghrcosuoa.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/ghzqykcju.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gflguryey.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gqqojyhrr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gebguwney.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbmyoihrg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/ggznwudih.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/grysbsdpy.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gvzzqbepd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gnyelqubi.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gkbchndej.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gukdxfqxb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/ghgvrflcb.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/ggsvzarth.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gtltifqbd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gofuthltd.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gbnuhcxfw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gvnqqjkll.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/giwkrsvqm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gmuquukdy.sHtML


<!-- 参考信息 -->