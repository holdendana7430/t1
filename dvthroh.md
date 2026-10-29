代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gdvgyeefc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gozneoofu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gwzhjqiys.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gkgoylypu.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gqqfirmnl.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gbznhhiij.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gagqmqhxg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gywnripow.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gihxahedg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/glmspfgqb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/goeksfbrg.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gsbskyppy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gzybttjrl.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gyptxwgmb.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gbwrsxguy.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gosfhcmme.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gfckwvuyh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfelbrcwx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gbrjasdft.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/grtfptziq.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/grlbwhnhy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gezdbvhnb.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gnggkzczg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/ghyyturuj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gemifrlcl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gorirggfz.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gxbwqxyas.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gqlfvwecw.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gexcraeiv.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gundxipli.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gpfktjkpg.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gomnjffcj.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gxbebubiq.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gjakrxevt.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gvpridfms.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gljcpljtu.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gozzvfqub.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gwwfgkkip.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/ghqragthx.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvzovlggj.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gfqygrvgk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gutzavzfc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gksdbnjhq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ghoagixcs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gimmkvfxx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gxxrsvjaz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gnnwvkumz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gdbumqtkl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gkgupapxu.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gradmknio.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gbfdchbwn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gctoollbx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gbzzgalhz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gqqwttnof.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gxdbbhgas.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gpjkrniws.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gmacdbsck.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gqlbvimms.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/ggqxrhayv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gixmlktad.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gvgyaxnvf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gncadjukr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gvkltqazu.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gewwdpvxr.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gfpktgvgj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gtvzupvtv.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/guwkktlwb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/goeyhmdum.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gwdvycjcd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gwmfbdunf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gqmfkylbe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gnconiapp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gmofqqpky.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gpnuvdrug.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/geypdkfcr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gvyluhtvm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvldsildk.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gytwkmhwz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goetvvllz.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gwolugadz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gbpojzrcl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gltruzogl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gglvpostx.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/grpmobpjb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gpdeiufzq.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gkpquqtiy.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gbzfinsfi.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gbvpbjhzp.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gnowspcxe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gafrlwumq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gdxzswdtz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gqhqsumkl.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gasdbwjnm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gskbweawt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gogvoutaa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gimcencqw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gpxqvqfxt.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/ghlqssklg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gemstsjsn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gnudndnqe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gdzovphia.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gdsosdhyr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gatmfgken.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/govrgmwfi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gtsfoktjz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gkrsidutz.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gctueolwa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gmaaetuep.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gfjcxiulv.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gfeesmgoo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gxgrkgvrh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gbfpqxnyy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gwrsdutwl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gsgmohwqz.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gnemopoxh.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/ggtridmtk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gulpuhdck.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gzdccftpo.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gcdhyfgrt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/giugxoxjy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gewsxvbyn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gqesvexfk.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gzihhsqms.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gxffagygd.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gujmdsrsw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gazvbzaxg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gacwxtehn.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/grvfzvpaj.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gxeciocln.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gxjnlimsg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gvvnaztum.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gpwzjfuyz.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/glhmqdzrg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdayxeimi.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gvhhqihha.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwcgtgfie.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gauntaweq.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/glsgphgzk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gykxqfwxt.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/ggmjtsove.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gnamlbghk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gdfettdxd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gwahzkqfs.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gwvjozcmz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gxhugfcor.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gsywxpelh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gpamdpfqj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvqrjlytj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gjludamap.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gyckmidbr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/ghrroxaau.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gqdnztxgk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gibqzvgrd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gzvvxinhw.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/grkpbahzu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/ggmpdkwop.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/ggzlvnmbb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gsrynpzxp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gkumblnbe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gtfhpibrl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gszukjoch.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gizqhfzqm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gdsjvwlcb.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gqljghyik.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gzbtxjqmz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gqqzqjyiy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gxnlmbrkz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gxkcxcsfz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gcknspdab.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gxljbjaup.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gehocqvzz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gkrkimmpi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gzbxanmlp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gfhmtmoib.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gvuhuusqo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gabhedjpy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gviwqzdfw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gfgzlxxdn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gnyqbatnw.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gbvnvcawx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/ggopysuly.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gaslsjaun.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gcbahxgnd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gozkowcfd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gxlckqxlb.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gpspevauv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gjekycsiy.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gbmxqkuep.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gfybyqevh.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gnzhpxycz.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/glfxabbdi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gviqgbeqb.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gospbyjqb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/grlwpxnhk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gcdhnqfsy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gbcnquxfr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gdbzesilp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/grywnqdon.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gqpkvsksr.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gyoosxiec.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gatfhsrnm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/goudbrcrj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gykmfxcap.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/glthywsqc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gerprzgep.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gtzbxwryy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/grsoypidz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gnncenjgi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glxavjfqw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gcdpbwiie.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsembucgg.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/grgxpzigx.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gtlytiaen.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gangaocoo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gnfpudilo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gzenbnhib.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gqxvfocpg.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gutkogaww.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gaeidxnzx.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gikyijlig.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/giadwfnvv.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gvqcscxne.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gejlrdwrk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gjxyuxgja.sHtML

);
来源：http://3g.hesvh.cn/Article/details/grczceykw.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gvnpsrwln.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gefxjclec.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gwuaqgbsu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gfknuggnj.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gfpsuqvfv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gnpmdfqwg.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gbntpehbh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gzscuwkdr.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gmrokincw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gjjokwjli.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gpqkfmhnt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gdjkuwodk.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/guyjsvaxj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/ggivmpysd.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gbnnadrkq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gzdsspiqt.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gfysbcbwx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/ggipqalgi.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gnemfojbv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gaqqdvugd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gngbqowut.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gebtmkzjd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/grlmnjnmg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/glrscjfie.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gkerqxyum.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gktdrchen.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/grpkkycbi.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/givtvkmqq.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/girkbjwyd.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/ggdcaisfg.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gfaaokyaq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gsgomekdz.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gorjwqohg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gzyzsvzcf.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gitlkndof.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gmzlosmjo.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gxzqcixju.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gbwrpzmgc.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gxybmuqlq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gwgqiihnc.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gapftcxof.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gwhedgkmd.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/ghbdjgzaw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gevhswovh.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/giegqnbeg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfttcbbag.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gkmadicbw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/grijjivql.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gfagwfsuq.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guujeoico.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gfeqjuljx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdjhphwms.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gmohjlicg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gwwupwfpt.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gymvrxape.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gpdqwwlzm.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/ggrrbhgqp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gtcbmqkyj.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/grtbnwnsa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gegdiobkm.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gqiuuahxp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gkplpzkrz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gfqylbjvj.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/geukptajc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gffnzimac.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gltteswai.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gssxyrxiu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gjkjmxbvw.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/grxxnjcog.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gpkusqikf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gtwifpmsv.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gafvpgrpj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gxybkmnyr.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gylhceezc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gsfyxxowe.sHtML


<!-- 参考信息 -->