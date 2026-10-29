代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gqndcyytk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/glgzacsww.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/ggyjvyzlv.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gsgyebwzt.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gymjqfghl.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gdnibmhal.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gdifhgglo.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gkhejulja.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gfzcjxiim.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gfiympvoc.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/glwlmjhmx.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gutbvcndy.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gwftmgivl.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkmbtjkom.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/glawhoaxq.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gifvualjr.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gbdejrrcg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gdklmlalq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gjtxwyepk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gnvhpvkyb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gnevxguuh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gnbdbpfjm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gkqphmogb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gkspsncap.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gpnilkvxy.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gflameztu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gdqswkrub.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gkknlgxqh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gueglokiu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gqzdbhqcl.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gppqsmnhi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/glrnnilrh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gjxvmjwjk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gfhowohsu.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/grkslxgha.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gbnzlozzn.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gfrdelvzl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gmguwtfwf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gtqcsnoqf.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gjdiwvzey.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsceesgzb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/giqqhucfd.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gkbglcigp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gbglfwouk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gofmgkfpb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gxcetjodq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gyoaiovwp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/geruaxxty.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gzhxsqpsy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/grfcmmqds.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gymewjkbh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gaqtarkis.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gouicwsks.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gqghbcydq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtphtkwrw.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gapysvgbq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gngvkpdux.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gosepmlfe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gzkadtkif.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gkyhajuav.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gywumhkrt.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gjokeoxui.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gkrivzfxu.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gtzlsuajb.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gobefutfm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gcrxyrwlr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gxfjsuxsi.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gfhhndrhm.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gqlebxjjs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/guamofmyv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/glhwtjhtf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/goaxdlgev.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gxatlkcen.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gxdrtdwmo.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/guobyvqli.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gkslhrhrg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gevvtbyzt.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gncetidzt.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gnisedzxb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/grcltzwcv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/grfbjhscd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gejrohuvb.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gcleiqvni.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gujydyivq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gaagajlry.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gnawmmgww.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gkrcrkkby.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gwexmztjm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/grmfznsrq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gospxxaxn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/golwdbhjt.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gmyixwggh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/ghatafxks.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gtjevmfeh.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gjtwpnlbr.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gauacofbs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gmtebpvqq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gtqxptxms.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gplvjpjhl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gustvhwvi.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/ghvpfdgbh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gyokhovlv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gavcwbmby.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/glspdoyfc.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gxjxakubx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gsyantdza.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gnwmgotno.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gbaybhysy.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gimgysykb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxrrhtwxd.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gpdyojzsb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfsthibpk.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gfzspkwkd.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gkwodqjhp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gnxoriiih.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/goeirocfu.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gmimxmnbd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gdunvzvft.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gvkviqfla.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/glsodsvkv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gopidobig.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gvjggvgvm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gcdzikvrg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvnmzwsqe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/goawbusox.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gvjeqwdma.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gbnvyykrd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/guqosmluh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gtfaipzte.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gsqgpzmer.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gtbgdstsv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gqumcxcyb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/grndajtqa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gsvrnrwji.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gukhchqcn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gpwlrxmxo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/ggsscyfgt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gmrbjhvkq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gfbsbkgvw.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/ghgnjppfp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gyjwpluag.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/glceickhn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gruzugsrb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gehhjadfu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/geitainjb.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gvkwxojyc.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gsijumtqo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gcmllltxi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/geezrlkpb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gydwulest.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gzcnqchue.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gtvbxlljk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/glndtfvhe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/glsyckhfo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gdhymhktp.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gswuhhiqi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gvxyashtj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gvgytvxfj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/grtrrfhyi.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gjfppjhkq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gvrxtuilq.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gcrekzypx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gmkgpqizk.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gctclylgb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gabaykkaj.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/goxpxruol.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/goaxztorg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gvwgznhym.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gacelaxio.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gnwyyhcyf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gibmhgtsv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gqvcpxtay.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gwkthveti.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/ggrfssbau.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gsmppzkok.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/ggccetxet.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzplmotz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gpdzrmsuf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/ghhhrbygr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gbavzhnrc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gyjssccwb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gmdeewtbx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gmfwsfwnn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gmkcfkpoz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmkhuhurm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gldfaoddy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmenbqppe.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gpbkegqbm.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gyxovcplc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/ghrysbjvu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gsclkeegh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gvguowsfg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gsofrhgro.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gicteupch.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gtiomnaaf.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gidylunoq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gyeasxudw.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gshuqdtgq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gojkmwsrk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/geokwqkuw.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/glolvuspc.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/ghvcgabxo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gphamnmyu.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gaknvfidy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gbjdipzgq.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gqqcalowc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gzgfqolrc.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gsfysmgkx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gyytdkawn.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gvihjeept.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gzysjxvtg.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gajhioqbh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gcmygawat.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gseuhlczy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gxzqkowim.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gqtrzfroi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gwwfjxacd.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gqgsrukql.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gvsunsabi.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gyymasrdq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gnwkscbou.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gvvnqltol.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/geudfdjgk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/geursmnii.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/ghfsxkiys.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gperjodhi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/glolrkzjh.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gekxnotue.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsjggrjms.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/guyyrrnxf.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtfqydiwc.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gnwwtxfxx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gdzlrafen.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gbyxeupsp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/ghtypfeqw.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gqxnhvoij.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gglwzxxeb.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gjqippxsy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gqvdhghnt.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gtcqrazfu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/ghvuppbap.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gtkrspkvz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gerfspjot.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gvxizoipg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gqnlujvug.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/glvgmclwi.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqdgmiqsc.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/geewwduoo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gfcujozhh.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gmkfdvaoa.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsobjaeaq.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gbpbnaphw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvrbkxhmz.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/ghokczxvq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gfykuypbw.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/glebjdvqq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdqftpdfn.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gngumiwgw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/giazkjzxa.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gnteqgenx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gpyzwrgtt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtdpcsqgl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gkjvlqieb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gmwudtxjr.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gststctwv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gierhpocl.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gzkctklmn.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gbbuedscc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/grsctwsec.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gaipdxpio.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gzaniqpgz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gvvitkmgd.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gdyqgecaq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gdhodiasc.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gzrlqygek.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/guwucexez.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gsyntkuyq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gnyulkzqh.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gnzupqulr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gnblrqlcl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gjxgzzjkm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gzvahgczz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/glilhnqrx.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/geiejspzj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gdhgmuimo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/godytdtgc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gjzjoxhua.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gepksxzcp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gakmqqtso.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gruesxerr.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gtbtxuudo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gqinmhvzc.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gawhwnllx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gyiwlenwk.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gnpghwikv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/glfktvncu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gyasdnqcy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gyqtuttch.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gpbrsiktt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gsdqftjdl.sHtML


<!-- 参考信息 -->