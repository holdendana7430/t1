代发 wailian999

[N05] 最大公约数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpmsagsq.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gcvdzoqgd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghtvkwocx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmsrfzrd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gadaiisze.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeoxueoe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggptqnssh.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcasynwf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsmdjfas.sHtML

[N06] 判断回文字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gzmvlqgzl.sHtML

Py:   s == s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbxxgjdu.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvagddyhg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwexdykm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqavfvau.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fanxiaobao.xyz/Article/details/goejhfuxf.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fanxiaobao.xyz/Article/details/guicaejmb.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/guwiqxiar.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkanqmyf.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fanxiaobao.xyz/Article/details/gberbgvfa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fanxiaobao.xyz/Article/details/garmvfkcw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fanxiaobao.xyz/Article/details/gimhwndwi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fanxiaobao.xyz/Article/details/govvpxahw.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpzsqdum.sHtML

Java: // 手写 HashMap
来源：http://blog.fanxiaobao.xyz/Article/details/gjabelprw.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fanxiaobao.xyz/Article/details/gylltpxpo.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaleqsuf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fanxiaobao.xyz/Article/details/ghkfrpuso.sHtML

[N08] 生成全排列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlcemodp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garhehobe.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdufgluy.sHtML

JS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gwgixagid.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiwaiztx.sHtML

Java: // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gcstwjwyq.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgbnvtrt.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gaggkvmit.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/glowuzhpm.sHtML

[N09] 栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceivfphv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/ggsrycufd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gzmhwbokt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gslqniqft.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fanxiaobao.xyz/Article/details/grqzudutb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/giuzurzuf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fanxiaobao.xyz/Article/details/gjetyjgfp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmmyfsnx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgmgycog.sHtML

[N10] 链表节点定义
来源：http://wap.fanxiaobao.xyz/Article/details/gdnqimryv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fanxiaobao.xyz/Article/details/gqvgmobxq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmklyvcl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/glmeqhfsm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gfizixxmx.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnljunby.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fanxiaobao.xyz/Article/details/ggmlezttn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/gnzqudipb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghvqnqyde.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gfanwurcu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwdhcbzi.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fanxiaobao.xyz/Article/details/goggqjakt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgbyofhi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gfokoydub.sHtML

Java: // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guunirzza.sHtML

Go:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnwshkzb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fanxiaobao.xyz/Article/details/gewqbqlgf.sHtML

C#:   // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/guyiautvs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fanxiaobao.xyz/Article/details/gwmrstngh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fanxiaobao.xyz/Article/details/glcsiuuaz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxbshlyh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gapfqrzlm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfespqscq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkbitcaj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlywevss.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfynxkxeu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/ghmmnyuig.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsasbxcm.sHtML

O. 并发与异步
来源：http://m.share.fanxiaobao.xyz/Article/details/gupyuumqr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdatvsskp.sHtML

[O01] 启动一个线程
来源：http://baike.fanxiaobao.xyz/Article/details/ghoveqpkd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gapwjjhlc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcuaqjnb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmruexdq.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gzenwsddi.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/grrszuici.sHtML

Go:   go f()
来源：http://wap.fanxiaobao.xyz/Article/details/gwjyfcjfr.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghddxxopz.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fanxiaobao.xyz/Article/details/gywodlxtn.sHtML

[O02] 使用线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfdnsrcx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fanxiaobao.xyz/Article/details/grqubqfut.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fanxiaobao.xyz/Article/details/gewfulmqs.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gswczvekt.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/ggxevxbzs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmfhjhtu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvtioliq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fanxiaobao.xyz/Article/details/gxbiibcbe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fanxiaobao.xyz/Article/details/gjwkqlrkl.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwcobzhp.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fanxiaobao.xyz/Article/details/goglvphcr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcocbxctn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsqyvhqe.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gkezxnjce.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grsglhfkv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fanxiaobao.xyz/Article/details/gmramukvt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcylrzwus.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gimkostup.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gufiynxpu.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/gaamaupvt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fanxiaobao.xyz/Article/details/glmnkplse.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gswhobusf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbkkmnrdu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fanxiaobao.xyz/Article/details/gqhsfydoq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fanxiaobao.xyz/Article/details/gqqtfuoxs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fanxiaobao.xyz/Article/details/ghblbkxvl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfhahxsn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fanxiaobao.xyz/Article/details/gopgoafjc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gmieuhadp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fanxiaobao.xyz/Article/details/ggesggwrm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghifmcjoy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhykfbsc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjphufiwp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fanxiaobao.xyz/Article/details/grullxnhl.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmatexras.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmhfnfwft.sHtML

[O06] 使用进程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gezvhciik.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fanxiaobao.xyz/Article/details/giqfaqehc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsrzoyup.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gsmytulzg.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmpexyvp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fanxiaobao.xyz/Article/details/gynftjmre.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fanxiaobao.xyz/Article/details/gqnxdthps.sHtML

Ruby: // fork 块
来源：http://3g.fanxiaobao.xyz/Article/details/grgozrxaw.sHtML

C#:   Parallel.For
来源：http://baike.fanxiaobao.xyz/Article/details/gpoymhhfb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwdknwsyj.sHtML

P. 常用工具函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcpmgorxm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gynpbimej.sHtML

[P01] 生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdtxkgxd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxicbzbei.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gjxtvpkkt.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/glohsfnag.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzwlazhp.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fanxiaobao.xyz/Article/details/geqmobkyf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gxzryraqy.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gprsczumg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmukhiue.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fanxiaobao.xyz/Article/details/gajjyyjkq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsppklqi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gdsjkwiso.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gsaftzblk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fanxiaobao.xyz/Article/details/gkssqlaid.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gginpfpst.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlbntads.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcafcqkl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fanxiaobao.xyz/Article/details/gwdrvzcyw.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrsenkem.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fanxiaobao.xyz/Article/details/gczxghjni.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrplrvwu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gtelghtee.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxcjaizi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrmzozjq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gakxjhxku.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxrpwwow.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fanxiaobao.xyz/Article/details/ganabokqn.sHtML

[P04] 求长度
来源：http://wap.fanxiaobao.xyz/Article/details/gyenydpna.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fanxiaobao.xyz/Article/details/gejahaqou.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhzyylis.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gemltmjfs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbaypfdo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gqnbwukhn.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fanxiaobao.xyz/Article/details/gtahteedc.sHtML

Ruby: x.length;  x.size
来源：http://blog.fanxiaobao.xyz/Article/details/gfgctmbhv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gscbnptys.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpigdgcy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fanxiaobao.xyz/Article/details/gksxdoyog.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtwxacku.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fanxiaobao.xyz/Article/details/goqfsmnph.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goupxwotv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fanxiaobao.xyz/Article/details/gwzjqnhgq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypoysswy.sHtML

Ruby: a == b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueffydel.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/ggskdlpoo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdroddxtq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gladizhfl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyivujwwz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fanxiaobao.xyz/Article/details/gppwywxrc.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmckcbwkw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gqoxycstf.sHtML

Go:   if x == nil {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzjddytn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmwomnjb.sHtML

C#:   if (x is null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjqnlsczc.sHtML

[P07] 防抖与节流
来源：http://blog.fanxiaobao.xyz/Article/details/gnkattqnk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/glnqyjzuv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrfdmpaq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzteeewx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/glugnyajv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqglxbyza.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fanxiaobao.xyz/Article/details/gmjhrvpjz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkgvgzbd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwqhqigl.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fanxiaobao.xyz/Article/details/gerpnoxjl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gypqizuur.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gvhdbienn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fanxiaobao.xyz/Article/details/gmgtcrobn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgyqodvx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnywlosoy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fanxiaobao.xyz/Article/details/gjnqsywhr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiyzryee.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddkgsdly.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiseetjj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/glwzvbych.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gldqboxvp.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gptjgcdjm.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gvihmixha.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxunfkyj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gwwhvsasd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrtjcwmk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fanxiaobao.xyz/Article/details/gozozmyzw.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzbhvnvm.sHtML

[Q02] 创建带外键的表
来源：http://3g.fanxiaobao.xyz/Article/details/glymeyjrs.sHtML

CREATE TABLE orders (
来源：http://wap.fanxiaobao.xyz/Article/details/gwhiwblys.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/ginzwxdva.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywhdfsbe.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpezlnsi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gnnlxzpza.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpbgmosh.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqfgaonb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvbiyavl.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqzbwbzz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflpvuzlq.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/gsmrsomrr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspvhwlvm.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepcpuyfy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgpmbivq.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaheammg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsnqhstv.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojmlmbkk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbgqrily.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/ghwtsogkd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpzgsslq.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabhvkltu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkktwcwt.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guomnkxrq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfomlmcd.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gyvscwsph.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gqqbrdzoe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojvclpme.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgjdegho.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gonsygwlg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqalcqhx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gxpuwrvbw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/glmtxmdbc.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gksoowual.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwyldzqr.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gslcjlzfo.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjwtgrns.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjakspod.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoiblqgt.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gxdovynwo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gqyaymadc.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjyjkwvd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggusmidnc.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyrqfegf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbqpnxnh.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyqexcpk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaffiztc.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/giqkrwvzf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/gmidtmqtu.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gndjepovk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/geqesscxk.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gdjucoqmh.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqbviomit.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gfascfenh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvsphnda.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gibeedddj.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gckslgzye.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtocoxbjf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggxxtcbqm.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeqlgrzf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnstxacmx.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrylliuf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfzhjbxf.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmyjpuxj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/grdhxgrug.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ghkdyodoc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gezrhzfje.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjaocsva.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gadhvmtit.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnfnhhbp.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahsmljuh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gumrzxtne.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gigmfsgxf.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/geokcimvj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopqcgtfx.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gstnmzean.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyktxlzs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gafechwai.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/grwdpnesa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjivmrjaz.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebuajbzr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gmrztqckl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gedjnuvfo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagqdjvur.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gilomgvld.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gspdjpyqb.sHtML


<!-- 参考信息 -->