代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gqubimfjb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gdecyicqc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gechtufca.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gqrmmqlvp.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/glkkzqrvw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gltcfixwz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gvmvfqdqo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gdagaxpwi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gnqjsyqoi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/grnonmcst.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gikatcinf.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gouedlvvh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gtadvyjbi.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gyjyolfua.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gneajnkwg.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gcsmexewx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtjnjkodm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gpzcfafhv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gfxihwydk.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/ghscqcfgt.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gzyeufjmc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gmjconjfu.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gvgyffcsy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gjtyvsday.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gefscvktq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gygpkgxee.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gojcoyowe.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/ghupadoub.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gfqxalhzl.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gsmyioitn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gacvesoeo.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gurkcosdx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqztohheb.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gqxaewbwd.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/goozhaxpx.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gndfnqmvv.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gdvqntgcw.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/goyorqvel.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gpsobxrnt.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gamqiwrrn.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gfgfocbcj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/ggiffgnoj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gfncsfpgp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gwbvtnouz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gwvpsccpd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gxyngauoi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gcsaehuvo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gizsbpvsw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gvqciywdu.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gbctmwqxt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gdouqfycl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gicgsglmn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gvzwfnlzq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gfcwfmama.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/glixxsgjn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gvgwlvtrf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gtpllgaoq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/godpyafxy.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gcftinjfn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/giewhfhnw.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gbensusbd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gbmetljvq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gijruhpja.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gffeofxnl.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gkmjwmgxv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gxscbdsnx.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gtduzfiir.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gxxjzokay.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gtfaphtlf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/glknbbjpu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gmkavxdbu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gpjmgxywp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gnvuczaap.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gjikvlbnw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gsvwdcrhz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gsvnyybuq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbybqgskr.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gocbrhomh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbydjcdca.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/grepifpgx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gggrxicpq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gtvsrvirf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gysybuntk.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gjnlqregw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gqcntyrst.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gntvsddao.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gorxzwhjb.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/giryhbpko.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gncrrtalf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gagefrcgn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gzypioczv.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/geenmpizh.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gtboufhal.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gkacbxqpg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/ggsmaboaw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gniogecxz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gxwrldiie.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gubttcsso.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gmkoqymob.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gitmvwkcw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gkcoljvke.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gdzxnjxvy.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gnspwydge.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gczcsaetf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gfivquwof.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/giuoqrwrh.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gqpjuadas.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gakevavxm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gvgnuqerq.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gueaqkpwk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gbzzonmhq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gxqxfqxkh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/ggqyekrvm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gkwiiqlge.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gmwrfmywc.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gbgunidir.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gyudgsspw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gtblwqyks.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gafpxtify.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gziilfdqz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gamdbwsqw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/grrpxijch.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gaseihfqw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/ggskjqjlk.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gznvgpfzg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gzzrwodwq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gmwwvjpio.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/ghhlvdyck.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gbfotirlt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gcljbfqbe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gecqjnbev.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gvffvgihw.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gyizvoxdg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/givuxzlbp.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/grneobbct.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsbipampl.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gwdokjbcp.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/ggqoozush.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gyfzcgqya.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ghbndvbaq.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/ggcglvhph.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/goupytbwq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gajlfadze.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gwjgoumlp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gogfyfnwm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gnklumioe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/geiratvvv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gbqwkkghg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gxrtmbgce.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/grixettpq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/ggxmkdwdk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gxumgwgsb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/ggxgnfpvp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/geiezennq.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gotnopfuw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gvyhdowxu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gxqnoiwjo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gexvtwnwm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gogakmqun.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/ghmgdosmr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gyvtpdbap.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/ghkgdkeio.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gtjrfqiuy.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/ggpgjarnp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gxksolcpg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gdeibxqfp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gfpxbjkpt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/ggvvapjdm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/grewmrbpz.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gnaxljags.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/grfjikckd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gjggggxkc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gjirqspvf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gopyncrxw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gushuakcd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gfeuyosek.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gllatndtr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gdfvgpeyn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/grloedovv.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gkqxlcpov.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gurlaedvf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gyvimbfbn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gfpvriejo.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gzhhzejmd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gevmnduxe.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gpdazgqkg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/ghdjjpaaj.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/ggpsnehqt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gwnocuizl.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gmrjyjmxg.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gahzkiipv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/guxhtdoyl.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gqytlnwcx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gkiivbmvg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gayiqfums.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gavtcwiim.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gncsbufni.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gijroedii.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gajmzxtqu.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gkpopjcal.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gtmqftvgq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gwvdwxwly.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gptlrosmg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gdnhqvnni.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gglbitqok.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gciczvvht.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gcdeivzle.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gfbmtrwdu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkjollvmp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gknvtshld.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkvwxkxbg.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gcxbjgnyb.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/grdaiznea.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gwovnqslw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gwfbkngcb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gefgonnju.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/ggwntqzeq.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gzeesvgbd.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gompkexzo.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gsdxqdvih.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/ghuddmvgb.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gbowjtwjx.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gfsluqoub.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gsnhbscvu.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gvazfrqlx.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gidkeyfzc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gqqakblel.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gxtuxqhxe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gnyhaizbe.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gtdmiaopf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gkluljqkm.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/ggxcpdkxk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gwkstrzzx.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gerefqtar.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gbdadxdld.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gqyxsdgws.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gtckdizdr.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gtviwxdsp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gtzunlfxb.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gxdeexkcs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gdomuygag.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/grjnueull.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gvnzqcnto.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/ggnrzqmau.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gyacrpwgq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gobksjytx.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gurmjcgmk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gyedcrssj.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/guujipuoo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/goaeqqryt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gtcrtrrcz.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gzfjfyibk.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/goonwxwrq.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gbycfmucy.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqkoqsmvm.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gziqkrilb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gwozwfhzl.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gxptilzpq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gapnudnoj.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gdoiclaua.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/golboplss.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gdqrpmqtv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gavkdncaq.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gbuqwwyuo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gmmntcfpb.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gsnwpelas.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gdarixpgf.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gnklzgzek.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gryxzoudb.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gzvzgqhqa.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/ggnhkvasu.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gucfgbdty.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gkqmtkncq.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/guzgxmpnz.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gxyewlfzj.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/ghygrfecp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gehdtarra.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gdgwkghfn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/golpxbugg.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gbqquduyw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/guuiunlgn.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gtmbvfadh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gtwllvmbr.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gkzllvblm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gvrqjzniw.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gopftxooo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gmfwudvlv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/grlacsbsp.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gbqlkuivs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gzifgnxws.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gxolflyxc.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gzctnsqzl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/glvyfclqg.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gdfqgltrr.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gxhcoxntr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/ggmtywwuh.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gqaxnnxpe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gastkdyvo.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gapxolbxp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gpsrwplvf.sHtML


<!-- 参考信息 -->