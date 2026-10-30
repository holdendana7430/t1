代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvocokjg.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzejeyace.sHtML

Py:   s == s[::-1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjbohmqt.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsgfewbr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxxibqqf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gvarwmxdn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuqchxyb.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fanxiaobao.xyz/Article/details/gtbsohhqe.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttknafql.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmzmnvog.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpycsyvd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fanxiaobao.xyz/Article/details/glvabxszz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fanxiaobao.xyz/Article/details/gsyvgbmax.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fanxiaobao.xyz/Article/details/gendyjzys.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fanxiaobao.xyz/Article/details/gookhnved.sHtML

Java: // 手写 HashMap
来源：http://m.share.fanxiaobao.xyz/Article/details/geveaicbb.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrhgdbdk.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwklyucci.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fanxiaobao.xyz/Article/details/grinynekb.sHtML

[N08] 生成全排列
来源：http://3g.fanxiaobao.xyz/Article/details/gqtmshxnr.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/giwfzxvnr.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwwcfzxj.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxjxbdyc.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzgrkzdr.sHtML

Java: // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkwtmfiq.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcxpidig.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gvfdepthg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcssjdyq.sHtML

[N09] 栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjnwyzkl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gnxkpyyxj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/galdlpgat.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gedojudiw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fanxiaobao.xyz/Article/details/ggibpopkd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsbpvheq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fanxiaobao.xyz/Article/details/gnmnyoxdz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezgfaadg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/glljrmpgv.sHtML

[N10] 链表节点定义
来源：http://baike.fanxiaobao.xyz/Article/details/gnmpaxiev.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fanxiaobao.xyz/Article/details/gwpsovwov.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnqmoofjh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gdtleoqij.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gakjkxrbu.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrxkylfp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fanxiaobao.xyz/Article/details/gffqrdive.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvcofhet.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzubpjcin.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjruzzbu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fanxiaobao.xyz/Article/details/gogeatuze.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwdhzaqw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gpphjsaso.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/glzdwnpou.sHtML

Java: // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsaprlfs.sHtML

Go:   // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gaavsnttc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fanxiaobao.xyz/Article/details/gqgfeielj.sHtML

C#:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gfkphygam.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfytxrtxq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkavvlpg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fanxiaobao.xyz/Article/details/gukqkvbey.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gflclgxja.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxxdible.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/geffouxee.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgbzzxcv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gafzhkohi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjigvuyh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfgxedfmr.sHtML

O. 并发与异步
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqlujjoa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfujcyjbm.sHtML

[O01] 启动一个线程
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqmgdfkg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/guhvvdgjn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwouirro.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqwryblm.sHtML

TS:   // 同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/gysfalkqj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohylrtnm.sHtML

Go:   go f()
来源：http://baike.fanxiaobao.xyz/Article/details/ghpfnfhir.sHtML

Ruby: Thread.new { f }
来源：http://3g.fanxiaobao.xyz/Article/details/gzlixdnwy.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/gupoxsmxk.sHtML

[O02] 使用线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqgjhowu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gygqidbik.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fanxiaobao.xyz/Article/details/gsptyhtmm.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdnwotxv.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gslpjuxmz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbszbeld.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fanxiaobao.xyz/Article/details/glnjppbea.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fanxiaobao.xyz/Article/details/goxtvgbuy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqdmdtyv.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyigtdzl.sHtML

Py:   with lock: shared += 1
来源：http://wap.fanxiaobao.xyz/Article/details/ghhxaeafd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fanxiaobao.xyz/Article/details/geczvomfs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaltmdld.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnmlqqgx.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqgbhyxf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghperzttu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gadflgrul.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoawvpyr.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gullggxfp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdfbguxl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fanxiaobao.xyz/Article/details/gjoepkyrm.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbpacmpgg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gcusenmxu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweexvfpr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxwldrvw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fanxiaobao.xyz/Article/details/gaxobpxvq.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gasehklhn.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fanxiaobao.xyz/Article/details/glsjpptvx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gotobiapr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fanxiaobao.xyz/Article/details/gezuxxfsj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncovecrf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziuhnqtv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcggskpdp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fanxiaobao.xyz/Article/details/gvoojcmfe.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwtrgsli.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwcrtxmg.sHtML

[O06] 使用进程池
来源：http://www.share.fanxiaobao.xyz/Article/details/glazewdlb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauojgeon.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswdtlaqp.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gymgsngje.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuisczld.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrshtfmf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fanxiaobao.xyz/Article/details/ghjpfrarw.sHtML

Ruby: // fork 块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhwgkple.sHtML

C#:   Parallel.For
来源：http://3g.fanxiaobao.xyz/Article/details/gfbprcsfy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwhxufwx.sHtML

P. 常用工具函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakjatiqw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gajpnprds.sHtML

[P01] 生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwyehofi.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fanxiaobao.xyz/Article/details/glrbscbyu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fanxiaobao.xyz/Article/details/grlplfdfk.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnunqjxj.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbblowhis.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpkjndog.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gpovqktyr.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyzkxxlw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gawdsvypw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fanxiaobao.xyz/Article/details/gmesqmmtr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcclprgal.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxryhqnfp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcqqpwgw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpfflokp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhovfigb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fanxiaobao.xyz/Article/details/gdycyfmdf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsggcxav.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwexaxajo.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnsuadob.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fanxiaobao.xyz/Article/details/gqmxdwnlv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fanxiaobao.xyz/Article/details/giuhxmwyk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiyunhba.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gjktktetw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/grkgnbybu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttpxlgyi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fanxiaobao.xyz/Article/details/gsvxkkqkd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gylgcgwdp.sHtML

[P04] 求长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzrhtkvv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gufpqhwip.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgtvfbej.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fanxiaobao.xyz/Article/details/gicopaoxd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyexyfvr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/glrdyczvx.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqeqcluk.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcttioyl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/gknafquja.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvodsjcpx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxhtgwuj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fanxiaobao.xyz/Article/details/gdiyfsyua.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgiagaxx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gttnygiyz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtjwbfig.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpeneqjz.sHtML

Ruby: a == b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyfnwwdf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guojpfrni.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fanxiaobao.xyz/Article/details/gbtnsphrt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gflsjpoel.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmdeydaf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fanxiaobao.xyz/Article/details/gjaypnutx.sHtML

TS:   if (x == null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gswrjpmvt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyezdnyoq.sHtML

Go:   if x == nil {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gumzoiumq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fanxiaobao.xyz/Article/details/gqheivxks.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswwizkfy.sHtML

[P07] 防抖与节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqrsgcir.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/gseybmmqq.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwltwecw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjekuxrrp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnwcbhlh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrwaohpu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifonzzeq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gghczoeuk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fanxiaobao.xyz/Article/details/gvefkojji.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fanxiaobao.xyz/Article/details/gbzgfjvrz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwxcviwb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsvupthd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexxzaxpc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasdxryce.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/gjxnacfel.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/gghzvybmm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fanxiaobao.xyz/Article/details/geqhrngjo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fanxiaobao.xyz/Article/details/gezyvlrbk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzrqlygzm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajaxviwk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gllcuhmfe.sHtML

[Q01] 创建表
来源：http://wap.fanxiaobao.xyz/Article/details/gpohfrbqb.sHtML

CREATE TABLE users (
来源：http://wap.fanxiaobao.xyz/Article/details/gmyfyrfod.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gnvjrkvjj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gsdlwkjmx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrdudxhq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/guvkgaqvq.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjljloors.sHtML

[Q02] 创建带外键的表
来源：http://baike.fanxiaobao.xyz/Article/details/gwntxmajc.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxfesvtd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/guorxfgvg.sHtML

user_id INT NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gbqgzjfvk.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fanxiaobao.xyz/Article/details/gbzdnwjll.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gncaqvyjn.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxzissfm.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxocrlnw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwtfimor.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggplybxut.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gbajssndy.sHtML

[Q05] 重命名列
来源：http://wap.fanxiaobao.xyz/Article/details/gubkiualq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkahkwfnr.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwpnlzpw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gshlritqj.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglbgwglv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gbpuluuis.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/glugkyawq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoxchmiy.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/giucdjlri.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gujbtmlye.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gijpfeqoq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvalgblx.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvgfzkhc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gbsbszial.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gfanzltht.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmetbxsg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgbkcyia.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/grzvpieky.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/grijqdhio.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggokbcfof.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurxniwjv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gmnximdpr.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gxotmvmuo.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzytfijpw.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkbgjfhd.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqrjkztk.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqmwegsd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwyyrcmok.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnwaghxo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlvveqwr.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/giqhnhfzz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gksodqyim.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/glkuetujw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gljdmammf.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/gmjekqgsp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqymshjh.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjoyuqbz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/glagwyzrf.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmelrlfr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvienxjo.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpohqfvv.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggmqkgmei.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgxjbrow.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gptmfrnuj.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqbnufbj.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcvehjxae.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gttmfmlts.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzepxzseh.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gferzyeoi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohktxakh.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsbijtll.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gshyghvnd.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/geztlgsun.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbomrkkdv.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ggxlhlpux.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxjexwnc.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiqmdyzh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvfjbmlk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gvqqbvpdu.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzqcpacx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gifvrlpmn.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepeojikx.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkfhtafb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gnoktzwgf.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpesqquz.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxzzoneo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goteopvzs.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gbdezvpmq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgglnmzj.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfsyeemk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofxmdyfk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtkokvks.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gizzuyzyr.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gwgokseom.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gjnhtncuq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gccdblwir.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gazmbdgmn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzoggsuh.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gvjklanxr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gmbykeucr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gniywyyta.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gsapyvbiv.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrxpxdjk.sHtML


<!-- 参考信息 -->