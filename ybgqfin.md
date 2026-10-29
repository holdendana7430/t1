代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/ggypudafq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gbkppkkny.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gfhrulzlx.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/ggyagrfwj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gextznefi.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/ghhwyjtcm.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gqxwncgyq.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gjanxuykp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gbohilgsc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gorfazvgg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gktghalbe.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gmdkvmncq.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gejfreywf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gyejacyda.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gnpvscwnh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gacosuaxf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/goljvdotn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gitqapfpc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/ggkzosocr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/giwwqumsy.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gfdjqvcpn.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/grdccczrq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gdgpygltg.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gxsixterd.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gwfkdtxle.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gjdieesea.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gxekpjokk.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gpfnayfoe.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gbopmjrzz.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gzboxsxvy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gspecykor.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gpvynqszp.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gqujwkrub.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gglizlmdw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gpoygsvsn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gukkmihbb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gjxleahyf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gpaekrbiy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gkxedsdhj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gadxwmtfo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gtdhwozhh.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gudxnujiu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gbsosgraa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gbdievnzu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gbgzcocxj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gjpanlxho.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gqphevrdv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gqtskexmq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/grjncwfaq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gdzemrpmm.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gwysumovt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gmhvecpsu.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gporrsnni.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gczgojwwg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gnfsxydlz.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gnimaosjc.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gdbfkiygk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/ghpxtqysn.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gueooxqop.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gzcznkopb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gqitvhozd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gibftngdi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gzpenwvqm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gstpwgtno.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/ghfdlwofa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gdrzmomdu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gzbnafbwh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gutmqahlz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqmnencka.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gzufunyho.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gryyucswp.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/glhpwqblr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gpbwclbwa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gulzmchkn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gnzyuzrfc.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gkvkmbgko.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gybizwqbl.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gzjolgene.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/grdsvkdmg.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gmwqdkgcw.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gjwgrvize.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gxhmnvpvi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gtxowdklp.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gdhnyotxh.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gyxeadgnb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/giaediulx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gkmorzqym.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gihdnqrlz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gjfcuiqnp.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gwvoggvbu.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gddcvgqoj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gqlznvhmm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/glirvldth.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gvozkfhtx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gxibegpfm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/giudkhoku.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gnqpkqijg.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gksoqbpfk.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/ganoqqbov.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/goujfnwtf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gmgasbteo.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gpedrudjo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gzzaytwnp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gfaxnokfz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gdptkufcl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gfximosxv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gldvfcciw.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gmoeyzwkx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gujetuuvx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gqkhpafay.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/glowdychc.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/getlohzpv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gxdmjcbop.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gevknsmzl.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gzztwyzhh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzaaejbc.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gwkwkofzi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gfvmtdbis.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gmowdupsg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gkwazldqe.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gekusrehv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gakrjkhfc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/ggrepoert.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gqzdvagso.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gnusvdlub.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gedtupxyy.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gczctcwjq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbfcnzwrk.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gnktgbvcj.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gviuwcnsz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gakjpvfbv.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/glaqgpppy.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gskppyxrb.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/ggrfsuozq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gdljfbeef.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gfhvpgobp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/geelytike.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gtkflqixd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gkclqpirs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gcitellsk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gywvgwyos.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/guruewqgx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gssfaplfb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gcajfglam.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfjwgzzle.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/guwsvgpkx.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gpespqvfd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gshjbdkxy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gsklpbyvw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gijgrgrng.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/glpuaocgh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gzishxsat.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/genebofsm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gfxcxfvre.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gayesqjhf.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/grnqncydm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/ghvwvxkdo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/guweohyxm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gddlwgwnx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gqljkeugl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gfheekmwc.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gazihdnbj.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gfniopypv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gkfnkyjyg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gqmybukmz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gjltamrwy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gvaxqbxkv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gnwlthesz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gtfjpxeon.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gzfukuqbb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/ggdbdkemc.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gowcpriho.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gqgdldlua.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gavsbnezr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gtcagwmie.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gixmpqodd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gsjlvvhwb.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/glnvgjkzu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gooejypkx.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/giefhpdov.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/ggwmecizi.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gvkyaqoye.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gbrxkldwo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gmeefxnci.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/glhepwepg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gymmqqzel.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gdpoufyql.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gaprbqxgs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gtprppmtu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/glxtznodr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/guhklwnec.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gtbwygelq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gwbutbyog.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gbzdweqrv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/grpflxwdb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gsxyjmiev.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gmrbmgixs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gjbkkiavg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gipchrluq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gmqknldja.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpjvhxjvj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gbsmpwxdq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnodmakuc.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/galrxqoqs.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gtfftqoar.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gsgagccho.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gowbajnrt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gjnsljigz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gjzsagksa.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gjupqjees.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/ghotmspag.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/ghxqbfanh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gijebfgge.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gvhwwapxg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gilflwdmq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/goaltvzfg.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gqkllkhzc.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gpyyysdlh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gydrldotw.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gnnezftra.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gmoxvhist.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gcwuorguy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gujfxlezb.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gtjbixsio.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gkvvcpuiw.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gojpxtpxe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gcdisurer.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gnqhyupdc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gedxmueya.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gltrqerdu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gafwssjqe.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gzzkgplsx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gwcnohfwr.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/goeosernb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gexehkloi.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/glntelcdn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gzgzlwzgm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gnaqogkem.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gnclusned.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gxbpnrlvu.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gzryybkwj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/giwgiykjx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gunwkweno.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gemhcbnih.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gaikqhpyg.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gozfsvxxh.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gnoqzaanb.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gwoehmsbm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/goazsydnm.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gcxncgqna.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gvvpwgmnj.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/geqvjepvp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gufjckzse.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gfajogkqy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/govzwukqq.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gcmgakjzi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gcccmuhfq.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gstjnhxmr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/guprlnlmg.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gilioxbgk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gezovtvuy.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gmurpxphc.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsafbaqqh.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gsrjksjwh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gtrjfalic.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gpdtyjybg.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gssabatau.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gkgwwpvwz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqbqvqkdt.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gzvrovrhe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcsijmuhf.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gsmspwiwl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfxzvhwkt.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gflujxxvh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gllmtatub.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gveywrxaw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/ggeitircy.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gcnefvpuq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gyhgbfcdy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gbecquckw.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/guyluyxir.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gzczbjjkf.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gciyrsqxn.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gifilrygc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gvuazfoju.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gdiihjkrx.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gdagswcsq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gwbzkjzqa.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gvmskwfev.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gkrwwjskf.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gcdxxxjww.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gbxalcbdx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gzqeoqisx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gjapyismw.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gkikxnfhh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gvccrgbfi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gfyppkzap.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gbecxktid.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gkhnkocxb.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/grygnscgz.sHtML


<!-- 参考信息 -->