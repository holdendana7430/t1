代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gklcaktqb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gldaczjcg.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gkczrupku.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gvjrzzzzu.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/glnaybcyb.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gczqrtxgk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gxgsulokf.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gzqgphznd.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gcdizcjwi.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gvaaxuiif.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gwpxktnit.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjigxhhhu.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/geibnbhjq.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gtjjyvcuf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gwpwgvtsb.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gvgeejtke.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gnaboyfdk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gefkjospq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/ghwjzydyv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gsyzfdhec.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gvhycaucf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gtqkeeeic.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gphxnukup.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjkxrodhq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gdsakfvrf.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gjvrvgstd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gmtnjsimf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gthkcnhvh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gaumcagno.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gjwyxcrbl.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gdbilcypr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gmsssupdk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gxbmkbnpp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gbezgszjy.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gnaamxzsb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gpacqhhlo.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gcsymrhka.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gqsspfvbn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gdmasyiaa.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gwowviwwl.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gygzkzkfv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/goaijlvxa.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gvayhealt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gfmwsumag.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gdwnmbrhu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gfszjcjvo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gqciipspv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/giclmnmiq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gbdfcatnp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/girottczf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gfbocjscx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gvnrtewjc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnzwhcegi.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gsyhjvvib.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcfjmdsmh.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gsxgvgpwy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gprwbdqmv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gnrwncttk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/ghhqnyaef.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gftvqlgss.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gkfalbmyo.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gxmcpneyr.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/grnedsurj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gaxdnoqxr.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gikwojpks.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gfbahpwoz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gtjrptbkz.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gdxpeijhg.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gavocgaue.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gwankhrra.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gnxvluuvi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/ggsgnekvh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/ggcztjdas.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gorileeii.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gpbsefmce.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/ghkfrudtm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gvbounttd.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gmszhhubv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/ganobfquf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gywkkisba.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gfdzbyyjh.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gppunaidd.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gprjswtvs.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gtjfxnrbu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gzumyjvxe.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gbjzqkbho.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gniymtiau.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/ggismyeyd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/guaydbmei.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gcyrfmeoh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gocihlvkn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gmutccwgn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjbtkpwt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gsmzieivc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gnqzbnpop.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gidmadglm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gknurhmlg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gkpygjndu.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gemvaatxz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gpvyftgfr.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gnwwopgpg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gplfgvxfq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gapxtipax.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gihrkqxav.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gmfvyxwrq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gaovfdanx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/guwmtalvn.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/glduwlxdt.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gghyfpbfe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gawaxhyhr.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gupfabjaa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxcuuhbph.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gwcayznom.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gnazheojz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gnphtrejq.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gdqnlofsd.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gkzbxlcmr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnkqokmhw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/guszqvrxm.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gvmdqeqls.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gumlqmfml.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gmfcdcasj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gwxqnwytm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gjcynlpem.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/ghqyrneqz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gmezcqxoz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gxzuaiijl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gcdvpqiif.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/ggmkztxuz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gnqcgcaeo.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gahzxcjki.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gvekvqsfx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gbjgdrzoh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gwqnvdhil.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gzjwqqwrh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gcncrohvv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gastiqwqd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gtpaspjry.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/giffxttrm.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gmyzjmraw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gytrwmhep.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gvxpfirhc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/ghppzjgmv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gmxntpgsv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gfnbizban.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gvkwgqzhy.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gnqzglbaq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/grvhposll.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gpdxnpqac.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gseqrkmdt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gzbxueohs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/ghjgupxnv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gkcsbifug.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gbdgoofqp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gsqrydldt.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gcemboazu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/grcdytool.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gxpddhdge.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gldcgkrva.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/glyfkqezv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/ggdfqgkay.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gfxcfitjv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gkuhtxjvi.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gkztupzcu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gwhmrhdgo.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gvgafdtkz.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gcmunrlfb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/giouuggkz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gjqspfswr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gzlfezkow.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/ggdadeqye.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gntfcbvus.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gxifdqshm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gdzgiadlf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gghxggfur.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gvxttmyev.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gxfxuwsjw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/ghgtuzwxp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gckuodkjr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/ghzquwbsn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gxgmnqsho.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gqytudicj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/glcuhycbv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gskrpthua.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geomaqhth.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gmsacuodq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkkoldyic.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gomdsrjnu.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gmtpswkuk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gjdpyqqnk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gbhbucwxt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gojvhkzxt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/goomegzxy.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gzrmdcutw.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/geajhzfcs.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gawwnakzm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/genpyinay.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gffyiyxmg.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gtnlstqsq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/grcjebfvm.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gczcfitby.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gbweklsbj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gmcgawtpn.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gwkusztgm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gyuqxijfv.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gkblupiks.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gwqkneiod.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gxajofriu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gvywlkexk.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gljuqjflx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gtbshkdno.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gnqawyjbw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gxdccqbgc.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gbddpzdsf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/glbwwewrr.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gmdpmpnzi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gehjigdzi.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gorzfiahm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gwhrzsfyo.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gzjsdunqn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gzsltirrx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gevkmvqxv.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gsbeirzim.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gbheijuor.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gqmzqjqah.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gpqnoeruf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gecqfigfe.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gxijvfjts.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/geefkqstd.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gwrjopwcy.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpcuukman.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gbobjdenw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvbeabtxa.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gwifegiin.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gkclnmria.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gvfdtzzbb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gsmtnerxw.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gqortazur.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gyaleytui.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gxvbyniil.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gerbcdohu.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gcbncdagw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gfsyrwfju.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gvjsyykub.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gpxqxqxgm.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gpymttyaz.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdoizarrj.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gwprwdcno.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/grkxzwxdv.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gawvmydzv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gynxzmtfq.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/ggwoinvvh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbsohuzte.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/ghkkzkckl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gnpnytylu.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/ggpmsszib.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gzhyohpat.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gqyczcwan.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gjkztkewy.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gwqseuhzx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gcjisacdz.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gzclxgopu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/ghfksuzar.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gcwnezvew.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gmgzhdtue.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/grdplprxm.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/giyvtrzpa.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gmaufiyzt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gqmzgsypd.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gjqlriylj.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gjdoqlsxh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gojysvglf.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gbfwdzzwg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gwotbiimf.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/giexhohyv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gkncbqizw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gukyzkicd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gmemgjevb.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gvyuzzjsv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gkiifleck.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gcltbbgee.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gqmhwjkvy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/ggfuvngvm.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/giyvkanme.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gycslycrh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gumdkerkt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gabsdphzu.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gjwebayqn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/glzfzquta.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gkpwwcirh.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gmtdzlesb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gwviagznf.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gqipabbsi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/guzxxbswm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/ghdcgefso.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gtsprhmdk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gwhhafjhn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gebfmyogk.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gdktxsfzb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gnnrqedhk.sHtML


<!-- 参考信息 -->