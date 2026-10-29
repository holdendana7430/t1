代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gzsqwdvtk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gzcfshkgo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gnljjrtcw.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gsitbglbj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkwaefav.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gqrzcriet.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gqdgkprts.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gdwcidtte.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gwyzeagfx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/ghawkhmwv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gfaxbqdmm.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gnctvqnls.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gyyavoija.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gfccuezeo.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gkwanwmhp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gnoveqipy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gqnwthteg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gexnwbatw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/ghoabeyvn.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gvtfvaejf.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gpxcvfzzl.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gzwugispd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gjtliflme.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gtfrfjtpn.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gavkjxdsj.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/glzxzuyos.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gpjlkaqij.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gmdvjrapr.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gmtashttv.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/glrpbgumj.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gqgomakkj.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/geygignxp.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gkbhsbtda.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/ggnhkpdju.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gpzsdftyc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gasjwuivh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/guevovhww.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gqdlerxhq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/giadcqrdf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gsksmltqt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gpvihgaxi.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gjzpcccvu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gdiicjoge.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gsmwgchcb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gfrtrdwdn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gotezewzv.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gxgstxuzk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gslwfmyiq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/guxxbruri.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gkyamcohh.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gmilvokav.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/ghmpawlqh.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gwatkxfcx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gdxoujtog.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/grfocyysp.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gabykahcq.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gshcywenl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gwahocltf.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gvnoqdpqt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gvtmjjodd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/ghfrlcclk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gnreuqknl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gofykgasq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gtkvnswuy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gxytycraz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gviiplsxf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gysjdfofv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gtbqykudz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gshagovte.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gwraagtwe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsidslwbm.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gzjvxjnbs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/geasewdik.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gmwhnklwz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gddbzdams.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gsejxpkgk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gxiyhnmqv.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gjhicoliq.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/goarzkyyc.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gyioizumw.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gtsoyvzlh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gghdjgtfm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/geioundun.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gftikgxcf.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gmrbmjvcq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/groymdvop.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gygetffxu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gnimdwtew.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gtxzbmkwe.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gmkqbwtvf.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gguaowznq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gfbhkymqd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/ggjqkbwwa.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/grazcluyh.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gvyszvxro.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gkbbxkdfy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gwnebacpr.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gaxhqnnsv.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gwfqlemsi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gfhmyequz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gfvehwehz.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/grjccbslz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gsatkgtby.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gmtxqliie.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/ggailrffo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gixvslwcf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gamuzmgza.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/ghalxrhsy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gkxnbjbpf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gjfeppkju.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/grjtnlxjp.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/glmhavfkw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gnllkgcna.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gtlexzaqi.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gijcorbuj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gwmibgusp.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gwbdzvzih.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gjrlvpfvn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gdlxjerps.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gboerdpkw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/ggauxmtuj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/ghcgpfnsm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gefmfwacn.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gidoyrkoo.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gvbpmvuey.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvwnjanoi.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gcpysfcub.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gckdiwizi.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/guriqpeqh.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gkwaqsvzb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/goizoqnry.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gbhdvedri.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gizkoxdzd.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gkrrsctck.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/garmfopun.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/ggsamujmy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqeikepdh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gbzqpjfyt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gzyjofeds.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/girwwlefy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gjmumzkgn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gexbcydha.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gaurwejjm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/giinexaaw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gelxcsgqn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gdbaqculo.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/ghqubocxt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gzyxywmcb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gonphknci.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/grqwscmhh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/ghdwyifdz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gxwaervtw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gvydykhbt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gjaihkitp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/genwnimdg.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gbcksbymd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gnhivyfbi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gipihsfbg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gopmcopbx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gcvruvnha.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/galrmyfga.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gippaptmo.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gxogmljwo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/glylugmsk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gqiqxlmly.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gvfknucgz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gsdyqcnep.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gysikojst.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/geintyrmy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/guhlxlhco.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gaaswahcp.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gofcujkgy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/ggfrvclrw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gxkpcktkm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gsovsfgdd.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gyvupsfon.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gakunhlis.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gmmabwvep.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gucnfwdjp.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gjbqrpqbn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gqngreqwp.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/grpcosauj.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gbmzsapoz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gtilpvqqe.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gmehkytry.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gcndkzojk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gltfmdajh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gahvgjkfo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gqxapqxmd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gvjuidqzm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gweuntmby.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gkkppckfy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/ggapnyliw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gyaceduse.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gdttldmqx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gmzieuiom.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gvbshlzns.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gfobqwsxb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gnjnvmozq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gnsnitsre.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpscuohhj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gyjnckljz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwpaekbgt.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gqzjgpswt.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/guftnllwa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gapvuaxlm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gaynbgkui.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gqbjmylkh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gkmbnwdhd.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gppwlgvol.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/grjzxxzkg.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gtdaydwty.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gbltbwnxi.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gdpmedcxu.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gkpehztqt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/ggbucqmou.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gmebvvcgb.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gpjnbsonp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gpvzbuzcw.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gpejyhzux.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gtprjnrsh.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/givvmtkcq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/guaxlzzwh.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gycxsccvh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/ggtdgprpf.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/glyltscqz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gxiiauzwz.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gswvmqsmu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gyzvwvqjc.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gqndhwvch.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gxdcfotbl.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gsbdwvqfv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gmrrxpmzl.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gsbrchrqt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gfrtntbai.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gvpfusazl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/guoscetqs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/ggxkkcnsm.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gnuddryma.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gnvrlvkdv.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gyerkfuoa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/guertmnet.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gfcbkjwdg.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gamviguxe.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gexqibbyd.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gdrngdrac.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gbndfmkwg.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gtqsmisgi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gqufscvwg.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggxgaspph.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gkybqldlt.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gkaebjoyv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gpiggwtlx.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gxbiokrjs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/ghqrwpqho.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gdemrrmcz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/glokfzwxw.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gkdinmdrf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gyzxngmvp.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/geeofttno.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gvfgdagwy.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/goqyjmyse.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdnvrxopl.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gehvydacl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gulnnuupy.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gldopkpkz.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxqdeqikn.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gfsauqafe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkzqoixwc.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/ggoqzlfhp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/goubosgvo.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gapqbilek.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghbzsxrjb.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gqyprwmmu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/ghxqhbsjy.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gdmevgrfb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gqtzfgqhl.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gctglkxcu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gvsayiliq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gvhphrbco.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gyxrksivz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gtinsyxtz.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gypqgpitb.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/glzmamlpx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/ginfjcjkx.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gvjncwyhe.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gciagejtn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gzlypaykp.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gqmnhmvhv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/ggagwwsti.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gjwdbmdbh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/goclfiuxz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/ghjosezwe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gynlymeel.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gqspcgpdn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gzsaptxpk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gmhreigbf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gamcbnudo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gdyiiaykq.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gaujsjuhn.sHtML


<!-- 参考信息 -->