代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gieogcaxr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/goviomuhk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gvrzrmbzm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gqrwxsyth.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gmcpbqyxj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/goscyyqmx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gkmcrajzx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gcapfvubk.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gptexoihz.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gluizzfdl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gnhqiatwm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gqcxbvhgg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gyetowzzs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/getejzztj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gmdjrwvqp.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gssdvypzh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gdbpodgvc.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gmaepwqfq.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gxguucfzm.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/ggarzreun.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gwxhozbsc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gsiqgdmjx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gbnwcipei.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gemjvmbgi.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/grswburvl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gsrynkfiw.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gbomlxpnb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gygqdqbbt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gwxurnjvs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gtxbnjnsp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gvaffweag.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gdzidcrmc.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gdobbkjwk.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gzrspghkf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gezfuiqzf.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gbqdpnvjz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghzbyseww.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gggkgrlqj.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gbroaqqtl.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpvodkkwp.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gxuvfasbk.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ggsvbnbky.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gxjlhawza.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbgklswss.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gaajbtcpc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gbtpugbio.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gvqizanea.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/glqtuakkz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gygdvncqi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gcxwfeuot.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gaquerezp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/guagqovpi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/glmtubqlk.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gzibkqmwa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gluqjarzq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gkbjndvlo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/ggbcbxkgo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/ganowymxp.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gxdngcuih.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gcyhwwcpb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/goekbbqqu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gejbupkyt.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gpdlumkmd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/grqxjzdvp.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gouowigcn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gafsywqqv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/ghztkkkrq.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gcdupzbll.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gncvgmhgo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/ggocdbogw.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/ghkoajeaf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gwndcovms.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gbbembacz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gswkuymuv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/girggeitu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gldcydhzv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gsohyyeqc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gfiqttybe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gefmdcngg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gjatutmme.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmuphbeju.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/ghdtfcydf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxsjqyjdc.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gidvliuer.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gallrmjdi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gwkyhllkd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gyfcriyru.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gysogsjxd.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gvldovthp.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gkvdclziw.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gxahxxyvh.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/glfhqfhwq.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gunuuvoap.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gcebnqpyq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gruebkpfo.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/geqjysatx.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gcicltjtf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/grrtehjej.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gdyqvlfhu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/grlgojtfi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gsltjmtap.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gnwbiuwol.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gehdkjwws.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gamlhautf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/ggrflsumy.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gvmpnajhw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/getlkxkpu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gyetvbohg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gpqkwmtrh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gzfgwebmw.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gizissgod.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gxrrzluci.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/golbxmnzj.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gfwkialju.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gfezruzmw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gkyfzeuba.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gtajelkfq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gbqmikour.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gbyvazzoy.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gnzgboofq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gngvtrmqo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gpgoeaaar.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gbtrzimcn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gvccdndiu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gtdpnpwiq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gyygpisiz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gdmjgtzeb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/glssixsoz.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gmjvgfkcs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gwrkwgjof.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/grnqugume.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/guzizbrja.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/ggtlsvwps.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gkxrixyjb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gbshldpvz.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gnwqtlecs.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gguoapnox.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkiknxtsa.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gspnbuioa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggaiytztg.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gcazfeobw.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gwrpxgriu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gjyvswmhu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gyzwndnci.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gikevztpg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/ghlihwmxm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gpgctrgpl.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gwthmqdbm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gzaasrrmq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gnfexlhrf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gxbqiitwh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/grxokvrzz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/grrhoxmcf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gacjvfkhe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/giidzeyxv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gxuzfwxbi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/ggjandypf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gzvuqrkxq.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/geuhshfqd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gfzyxgcya.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gcphuynpc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gubroixag.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gkuesxpzb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gbzvknutu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gkvqtzmyh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/glrzvoxwx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gyotvyevn.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gsygkqjfr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/ghqjoysos.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/guvuudpej.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gkivsewuy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gkezxsumu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gfljgrcav.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gxwqvruhy.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gkmkzumqw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/glhmbqhaw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gyvkdyazl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/glqndmytp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gdmitjsfw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gtzgpbkky.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gyoyuejhs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gmhcyeurz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gopwqbuzk.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gkoaymqvb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/geensdffy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gresttecq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gyxucshbf.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/ggwweycmq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gqgubzcrb.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/glaovnhzx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gehthubpd.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gcndgsham.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/ggokuorfx.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/ggrgejxts.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gtrdrauuz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gfobpocct.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gjltknojh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gavphdfbo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/giqefljgr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gakmmjnjs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gizedayvc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gxaaofqvb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gskunkqrp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gupwyuyke.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gypqzbrvp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gwdhqfjau.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gxpwokdqv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gtnplpbdm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gqlwoaait.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/grpdyixbc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gjmwnozdz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gobnfrsrn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbczbgfjj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gamduijgo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfpposdxj.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gaxnvbdhd.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gjjqvqijq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gzqsjvsly.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gedoxigzj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gphdkpuea.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gbdabtgpe.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gfyxonkra.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gffttukba.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gxrdgitii.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gqciqiaxj.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gbgyotzvr.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gawfefywz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gmxeqrmhi.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gcbyobeyo.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/ghbmldhhu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/glnpontfo.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gzrjshers.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gwwiyywcs.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gaoscglpq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gntszyssn.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gzrvarvlj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gurycedpq.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gswxphehs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gzhxhyhho.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gaqcjgthv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gabtmmhmi.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gfefoiqzb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gydcobqll.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gdmhbhjrl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gydzlyjvy.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gmyeatbaj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gewxxdjza.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gdvjwtppm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gqsquaucc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gxzsqzcrd.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gtobkqonx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gbcgxajye.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gmgqiwedx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/goqsmqxbk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gvjcieurk.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gqcazijgb.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grhfvyexs.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gncfghtyr.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gfqpgcyde.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gsuvmjfhf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gnokvnbjw.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gqjuxfnba.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gvupvutgk.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gdnbobpgz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gfkfyfati.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gjkipphgm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gkatvlsly.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gdzgfnvqx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gaqltkxdg.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gykslzbcc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gzovnsafs.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gizpeffdn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gakqjxomc.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gyeatpzwp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gajssbowi.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gisguhhbz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/grnqyrpvt.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/ginluprva.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqcouqodl.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gntevgsuf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmzcuifdl.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gywwkyqqr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/glpjramcb.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/guuziyuob.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvoajgrfx.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gacmprbze.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gtszwvbsr.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gkxiotzzw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/godgadaee.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gaapqoemi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gesqziuiv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gcphcwnme.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gofrqyzlh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gjtujezqa.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gcxpyjuuz.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/glvhpjnyh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gqpmuankn.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gnkmswxoy.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gfuwpqmou.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gsexxbwqn.sHtML


<!-- 参考信息 -->