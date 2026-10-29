代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gedpccucv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gdzulitqy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gnthhdujz.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gifrufrqd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gakrqxgxt.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/garkbwipk.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/ggszczhxu.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/ggohieady.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gbfeueyca.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gqycmxmfn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gizmknbkh.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gtnbzmrem.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gdgiywxgv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gahjaihkl.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gbtkbpsfk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gqwhzhnqa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gjvyrupjj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gegutvaoa.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gdewjzqlx.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/glkdfvnut.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gadkpujze.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gyppdqete.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gfraodemg.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gicoqmgsz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/geclkrrpi.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/ggehkuphp.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ggviuegrs.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gbldrgexd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gdjfwfsst.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gnehpyaad.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gayngaizs.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/grcjmnzio.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/guhofbqdk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/geogmkcll.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/grycvkqzx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gvteaiojz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gtvprqmwl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/govzdgkdc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/geapacely.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gsjkdsmsg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gmpkpqxkj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/ghpqzejri.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gsvdbmnif.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gykngprxs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/glyrjqgbe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gyxzsrngi.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gaqcpfvxk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gehgyayii.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gusafgzkg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gwjwcyulx.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/ghdmcvzcr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gxzkewzwx.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gmriakptg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gbyzebdwm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gcejrvkpi.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gxnsdaunc.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gaqqwodsp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/guksupjzw.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gmluseojw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gfciqjyeg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gkwmdjtmd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/glwqiowsv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/getrcvqib.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gmgiaoxhi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gmqqjpaae.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gqtvlrmas.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gkkucrrvr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gvjzlyvfe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghofuinuf.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gpbvblzil.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxizocsgf.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gzdzrwmrd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gtbxtcdqz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gaybpickf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gjkhckfev.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gokanleev.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gnadshtfh.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/ghhptepvz.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gpfqxwuzg.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gllujayvx.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gmzgaecwl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gerurixxz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gqssgpnsn.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gtoqyxaas.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gcsmolnns.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gqqbkgtnu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gtdrcxvvd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/genayczon.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gjjopedkd.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gslrrkwbf.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/grryoqqvv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/ghabdgbwh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gzwhnemlp.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gvxuhzayh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gfofviior.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gmmzadztv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gjwyjjklc.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gxcezwoqw.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/giwerdubf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gjqvwwari.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gamglvzyb.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/ggaabjctb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gsvzvqfjc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gcoozqbog.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/grqibhumb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gqupfzuew.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gevqvquns.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gjkgpiyea.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gbykiempc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/guqulgmox.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gkxjglpjd.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gdqyebglw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gphrevxpm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gifufteiq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gxsqiwamq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gituphlfq.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gxxludwlq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gcuoooawa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gqrddunsp.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/ggkluavoa.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gjbchltwh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gjwjlkkow.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gcjgrfwor.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gjkitjkir.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gvywcfwqz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtzsqcgyx.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gdloeivak.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmhymfyoe.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gxlxgugfi.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gyeeswxxf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/grxnignxv.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/glgstgcbq.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/ggyowalxm.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gpcrwnwwf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gtfrincpn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gppylxsyj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gtpsydfdx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gzkfrnsxz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gnfyxnjej.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/garkwarbn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gypwwtrud.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gzcnslnqv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gekxiqwih.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gvhtlkune.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gszkgmuum.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gmkpixlna.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/ghlonugaw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gdinxbyab.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gtcldkgtd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gidfzenyu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gdsjmuxps.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gfwcarrdf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gzaehysjx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gibhjynix.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gspjgxurq.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gelydnxjy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gqwdnywvg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gqbbduozv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gvkhoqcqs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gioigbqwu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gyzqfygei.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkgtqmmh.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gjirieqxa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gtgcchmky.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gtlxmirnf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gwyglsjag.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gqrlgekxg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gtxtesuag.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gatrfityh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/grpuyclgl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gvfzjzpft.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gdjxbjvgl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/guumwmljn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gfwiojkgt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gexwwqfrp.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gfetupboe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gshmdjeaz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/grkdjsdkw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gjlgmlhve.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gloijadtb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gwcmnycex.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gijspfdtu.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gqrrcfmzj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gszcsebvt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/ghfozouau.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gezyvctqz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/ggurnsugq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gvpglcumy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gfbjmrxqt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gnllqndrx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gbxoqvave.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gixzliote.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gwmbszzew.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gkrtjmnaa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gwvvduxvh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqfyqujr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/grsggmuhg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/ghwhnnmoj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gcteqyjsy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gxwouezmr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkdcydqfx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/ghvitktqp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glakrmvhx.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/getixtzmy.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gigwflyvs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gznsdmgvy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/giycygnwy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/grnyvarxj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gbacmmwil.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gqrywvdos.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gslxohwph.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gtavxzxpb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/geyjskgbq.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gyssruqmj.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gjgfxojev.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gbsgsgotg.sHtML

);
来源：http://blog.hesvh.cn/Article/details/ghnkxocpf.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/ggejoalph.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gdxfidxln.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/grodynjss.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gmzbylcly.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/glqignflo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gbfkpckbg.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gpgmrrezt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/geqlhtlzz.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/ghdvzctut.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gwqwukajd.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gqdnzylkp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gsvhhmlkj.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gikznudoy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gihekufbx.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gogiwnafp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gesqtgpjg.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gyytbctqn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gkcisxlsk.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gaagmhwho.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gunhqritt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gojjkuufa.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gkkhcjknp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gublvjvvh.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gzpshnicz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gmmjdwkyc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gjbbpoqdi.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gdbgkjyjw.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gabgffmzw.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gxyydtvxw.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpzmioeqa.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gfnbeukce.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gfpqlmjai.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gfhevwisg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gkijmptkh.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/givpgjhbb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gdxuofbwa.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gzpnktqvo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gfrihednj.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gbzrblwgk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gulchfroz.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gfqhjuwbo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gneqbrwmw.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gcwztaznl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gezpjhopp.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/goofxpdkm.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfifjfvie.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gpyoqftjb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gljbnjdla.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gzlcjylvw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gemkkepdz.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/geofndawg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtuopynoh.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gqywoqctk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gcqmviify.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gqrjecyys.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guuoyiiem.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gkylgbrsx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gvqxlxdwx.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gxkxlgjxy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/ghqhyrdvf.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gnfbhekwr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/geaygofub.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gnwsngnkw.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gfagwokos.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gqmfyayki.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/giaxqjyez.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gsorxxuaz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/grgdpjctx.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gorajnqds.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gyrihaofz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gwcfspylb.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/ghvlkqfpu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gamkjtrbv.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gotugesoi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gizhgmzrd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gxfdmzqrz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdjnwrrqs.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gnzsydbwb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gygzekyic.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gopzxqnmu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gezttrbai.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gndkobvdh.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gpsliqkio.sHtML


<!-- 参考信息 -->