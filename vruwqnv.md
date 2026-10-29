代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gexdtjfiw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gnszispce.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gwwleskuu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gaamsusqy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/goeczlbns.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gdhuymaym.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gnlmfxlow.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/guiyjcabi.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gcgqxtbre.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gxkgmiogx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gobafzzzq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gwdmocezj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/grsitqvbc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gpklisjzv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gaokcxoiz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gofyborjn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/ghvddfmfm.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/givrqjylp.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/glvmebitx.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/getetigmr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gtsqtkayt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gwtmbnppn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gqgqhkleg.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/glicdxyvc.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gppuoebhq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gurpmomtq.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gwyctvfwi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gisclqoah.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gouqpkajh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gembmbrbw.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gdlulhaua.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gamixbynj.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gnhjbkcmd.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gugwxrsrq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gatzflxdi.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/glcqurcdy.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gpnhqsupc.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gmdvplaio.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gmxgogbig.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gzpvqvipe.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gygiydpir.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/grzodlktc.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gwmaobvfk.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ggjnhbjqj.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gdelspkvz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/geokmfzfx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gpalplvig.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/ggtbkxdwy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gaqxtbbzq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gwzjwyaqi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gkusfxywl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gnhdqljem.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gxviygfit.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gaoylyrso.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gbuuecrbj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/goxtlmekc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gaqgmtjni.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gbgelddtu.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gbdofycic.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gswxyreew.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gppxkzlwc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gdssyuppu.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gbmlgngds.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/glwilsxhd.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gowlcekbp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gxjjphpth.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gqeutbufy.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gucsuhmir.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gxpxowrlx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gmqpklcwt.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/guechlmvw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gqrlxuyqp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gijwzhllc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gwrefeodn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gdpatmonp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gwemwlzvh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gioyrfzxb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbordvjib.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gyetifesd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gyolznlbk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guejobqnk.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gtfprnudn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grbohywwa.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/ggrizitlz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gjysjgwss.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/guihljerd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gidfhempb.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gmxaqljel.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gukaduqrk.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/ggzdzbstr.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gzyqezflw.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gikleqlzz.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/grwmiknbd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/ghmrzqfet.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gvpoevymy.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gprmomtyy.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gevzqfquj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gzuyjzlgi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gcxxomnwg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gqeamlska.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gtxpkkmxk.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gwspeirsx.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gwwtbfttx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gzwueprcs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/ghrkvwgpg.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/giigabklq.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gfnmkhpyi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gwalzjpfs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gxnpepmvo.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/giqqcjfsm.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gextvaemo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gqdyvbjrz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gcqaukjhw.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gepvetrtu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gidpjurtc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gsyzytefg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gdwrueiiq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gzlqsfjsi.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gfedfvrwj.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/grucruvxh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gtkpmrmxl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gjcvyecrn.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/goexjjspi.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gxrxxeocn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gfwhcnbvy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/giokfibxb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/glkrpuftg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gaprxmwgx.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gvkbdtcnj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/goiwkhbns.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/goljzuyvf.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gsvvabywz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gyyskjwpe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gzpmpalmu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gxzeneaiu.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/geesovupi.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gmwbmvlqk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmiqavgsr.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gtiolpmva.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdgissuru.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gskvrsnye.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/grnspgfvx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gksovffzi.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gfggergpp.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/ghjlyzhko.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gfsvmoxtq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gccndbwam.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gtxrzjpjn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gxkuzyett.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gkeeryevn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gvioofzzl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gztbfmmsz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gejemziqn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gbaqrgjwm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gfnydhxdh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gftvfhlbm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gcjzqgifx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/ggotkzdxf.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/guajwiylr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gvixpahjp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gehwccgdu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gqkdrainc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gvxyytlzc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gtforrqof.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gxthyrqpf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gefvduqsr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gkimegpej.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/ggyzjsvvt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gnddbvcef.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gfpegrwfg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gncdzpszf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gfqntlvbd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gniobxnsq.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gaprrheib.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gkfnjfnxf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gnpkkfegj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gncedxbwb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/grkoajwur.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gavfjuwou.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/guxglnzcj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gppqhodzf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/ghqtcvcfs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gytdwobft.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/goabpyqnp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gkglzpxox.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/ghwkgrgex.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gangqafqa.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwbafrsqt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gziozvivg.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/glhmpbvbh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gigcuhuyg.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gohjllxfn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gkroxuuva.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gpkclszao.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gyrkpqudp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gbuvpjtwe.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/grlcpillf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gutbrjzpl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gzzeuagwp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gyldkuqqu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/grptnaeyb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gjmluqaop.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gvipcqaro.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gzjlwdear.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gfiafuttm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gyytcgqlo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/guphdqgrf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/giafdfgei.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gknvspobw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gxthvgvrq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gieoftsjm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gbmogtqxi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdjljusmi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gahxhaftf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giooumfps.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gewvdquhm.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gasnbpwnb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gjcjfuhjm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/garizedbh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gnuymdyaz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/ghejwlcei.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gjlantcwl.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gfqxcpsfy.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gzefxxpwu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gvmkxxqcr.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gmojivpkm.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gwgjnuhrv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gqjhpxcya.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gmsxswgfp.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/geqnrclae.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gpmhkunay.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gvoglzvaq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gcmvnqiyg.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/glrxzbnkx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gqgfuzpqh.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gvkfkoxps.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gearfnzws.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gxkgcoynv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gbhmnuobo.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/ghvlirjpw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gqtczuqmp.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gzkytqtep.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/guhvpwpuk.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gilyojxir.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gxaxsrswz.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/ghwsbyrpg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gkshcothv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gcihgdocm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gvoegfshq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gzwktkfwd.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gdnrhylua.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gbsnwedqs.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gnfbptnvp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/ghfcrjkzh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gqzuepvsg.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gotprjigj.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsqgcgsfg.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gkqcanlbc.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxzukvkjd.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gxjgcgtlt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gkkuizspp.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gytqnrgfd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gnuzyedik.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gegehcknt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gnmqzlrzd.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/ggakvvpma.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gctwjbmnd.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gxydgvesx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gafnopfex.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/ghrshvece.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gfgueqkgw.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/guffhqhrb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gpameppik.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gqjnxmyxv.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdpegnkur.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gnwyoaudt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/grmgsxddu.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gofndkqhg.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaufarsrz.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/guhigdisb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpprqcqys.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gyovvpdua.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwsjzcbbc.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gwqgxsfwl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdndsuxeb.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gugnuoqif.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gltcfigzu.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gmhzhbrco.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gyfjxvuui.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gsrhztjdc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gxyzvgkot.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gifuhworj.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gxujnivmk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gcaxgpolo.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gtpvlafct.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gcjmqaixs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/ghpahlpqe.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/guvqqamkv.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gsnutddlk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/getelevrm.sHtML


<!-- 参考信息 -->