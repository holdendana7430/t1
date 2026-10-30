代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gxtcijwhm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/ggsxtihdd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gxzwnqetd.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gzivpxzst.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gycgwuysw.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gulcmgsvb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gbcbgdoqo.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gdkzzswqf.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gxgsjrdwa.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gsywzdnku.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gnthksvgy.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gmrxochxk.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gomygejqy.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gdqmuccvk.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/ggflkptxs.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gosbmygwf.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gzjtvhkjl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gukcmcwfk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gnpdxzkpe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/ghqecttdp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/grfmrxumt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gaoqgvjns.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gcexlapoj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gvukgbqoa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gcqydujfg.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gyaurbifd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gojinivpl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gnzacysdu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gfjgpyxzx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gpjslqhos.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/goeifdxjo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/givwphcte.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gxcelrboj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gftvbsqay.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gkytgfaxw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/grbxhaubt.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzfnkdcrw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gsieqljfj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gawsjlgwl.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/grggarsut.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gfhnfhwzw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gpysqomzl.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/glmidfitr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/grllpkfmt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gdvdxlrgx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gwdcompdp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/glhmshlxv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gfnxbgkti.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gtklcmxuz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gxnhihjhh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gzgmdswrk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/glpkphccl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmtazncuv.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gqykkwfiu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkibadbvp.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gifrlanry.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gmxtomjtx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/grhscvbch.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/glgybjsqr.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/ghwwblyka.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gyrhrfthw.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/ghluvqqsc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gbphkbbve.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gapgywohi.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gswaiakti.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/ghidxgjuf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gqhjfqxks.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gaanvidbt.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gzhgzmfsy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gvgkezucs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gwoiaxplv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gfdplvksk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gjlswfzpq.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/goqvihvak.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gxkgswisy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gegwqcijk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gkwywsdbf.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gykftvxyw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gheelzsbo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gwuorvajh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gkicttnpu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/ghkjadegv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gxvimcndm.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/guungsenz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gknhioyau.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gjflfuljs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/glizjxtvd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gzkfhpzgh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gzekfmcnq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gpjzcieuv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/ggrdkafkr.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/glbobinjn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gsetfqpsx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gbzxibrsm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gftdbpltx.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gnrsvqlve.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gutpfnhjm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gosxnukyh.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gwlfmbbkw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gjbawhtyh.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/grmxrlhrv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gcljkakcs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gsccpsqip.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gxatjqedt.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gzsalkqpu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gtzcbpydy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gikrohyri.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gmlbnqqzy.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gmnoezanw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gejtuotsw.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gkgsfdnsm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxgjglrwh.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gasubnrhy.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/giwityehn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gwurmvqqo.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gzxeebrem.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gegxeczzg.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gjmsrdlzy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gptcbfqbv.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gaaxevndd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/ghnvlangs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gghcscpml.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gblxhebda.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gfptrcixw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/ggtptvvjk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gxinwamqy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gifdiisss.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gfbxyapdx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggmhagwgp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/geqypvspw.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gzovlzcln.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gcwhxwisf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gzwkdgoea.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gflknwfgw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gcdnezyjg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gdnecspzq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/ghoaxfraq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gprvpnznm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gcydhgbsy.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gioucokqe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gsfwavern.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ghokoxofb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gsvjbacxb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gwzsrfras.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gpcysaayv.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gbrlcpwhs.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/ghtjkitpn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/ghuzszqos.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gkzkkdszr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gyjcngudp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gbhybajck.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gcizaqjjs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gozlfxono.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gohdjychx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gffpdyjsa.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gehkgrcdp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gocryrzlt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gneliqjji.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gfxavsnlm.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/ghhbcinng.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gekqmajsj.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/guuwbgjis.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gdcspyyff.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gafzrdyzw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gashrlqdr.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gvplbzlol.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gjsfbyjlo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gkqyjwpso.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gxiskgyvm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gvhmjxqgz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gycuagvfq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gdvooccjt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gpmttqbaq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gwxunepmf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gzuevkthz.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gzkykkdfx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/ghqtahkou.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gslwzdfif.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gvgddgonv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gbbidrgsk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/glezsekxt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/glfmffzgt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gxqcdqscy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gauasxxcm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqmyhmpiw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gjjibwmpk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdrhvabxz.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gszkyhfvm.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gfopghtgw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gjclzneja.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gdrtzuhah.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gppersbud.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gykttrsgx.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gtvqehgye.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gxcapfpxo.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/geoimsixw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gblprcxca.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gposomxed.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gbpglbplg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gkudxvwgi.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/geopbsnfh.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gdywzfxdj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gtlkqdshr.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gujktxoqn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gmernlvnw.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gncrbuxoe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gdaenzmgp.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/ggtxvnxvm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gfbxnxvwv.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gjcpvotgb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gaepjglzj.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gibgjnzbj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/glxlzebvl.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gzkwfyebd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gshvqqodn.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gsjfxgzbj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gmkkfqayf.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gzshohovj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gfgqfbpcj.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gyzqvvywc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/ggwsqupar.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gkjsvcnem.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gmhubdwhr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gfclfbqpn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gxpomactk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/ghmtrdjjp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gmbaborez.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/guawqbjwz.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggrhzsvdi.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gchrwnpvm.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gmnarkwso.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gbnnxeikl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gqaoobsov.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gtetsgcej.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gkpnvfopk.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gqnxwriug.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/grwaoqadj.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gqjlbxand.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gazfzhbvt.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gkirvqmpf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gjymqrtdz.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/glfbedoad.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gkvnacwlm.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gmfsbscai.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gikqzwchq.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/guynihuuv.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdhitqvil.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gbnoyyshn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gjkrigetz.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gwaahslex.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqjnjdoln.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gfbrwaiji.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/grcosxmpr.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/ggozyxeym.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gplludpzj.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gewhkphyz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzmaghchx.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gubesxhiu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/garsznnor.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/glvpyxnda.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/glpjqgnkk.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gnpjymmiz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gejlfzxog.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gbgbcckzs.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gpnlewepd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gaefhvseb.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gdjceleeg.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gsnprzrdw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gkninwxwy.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/giobhbobn.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gqokkxcxl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gufdwnzqy.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gaqupsdxz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gkgxyrvmd.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/glhgyrapk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/grkzwavbr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gkidbaskv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gsxorunzo.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/ghavgumxc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gwvywpupu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gamxzjlip.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gnrxhctfl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gzteactjl.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gocwzsadl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gsskpofzj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gobmzdvlc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gzzqmgtsp.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/glgebbtyg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gadsujfzl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gfrfiumcd.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/giifazwdm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gwokbzlhk.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/geshjcksb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/grydvsucw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gsogvsbgz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/govmplrgg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gxcbcvnpx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gvdxwcpjn.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gqyfgmptx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gvttslgoq.sHtML


<!-- 参考信息 -->