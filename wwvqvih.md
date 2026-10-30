代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gyxzblhba.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gyychhqnq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gpruamukw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gdmkqqyzg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gcvlhckmz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/ghflbcsls.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gsitldsdt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gwgjdvrea.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gevorldwp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gliuywsrl.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gmxvzkbiv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gvyyqnble.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/ggxwftnci.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/geqvznxty.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gpyrqhrrd.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/ggwqtprew.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gnsdijzjn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/goiktcghv.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gpqggmdfh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gqyjzblmh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gahjkwvos.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/glmtimuct.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gbbobpqwr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gndizrlsb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gtwhwdoek.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gwcjhikmx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/glxxjjmvf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gaklouiwt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glmvkdipg.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gksqmktkx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggdvurjqa.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/glkubitrf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/glpljujqr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gipqlbicp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gnseziamf.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gjagdscfl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/grovwxbeu.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gffftpwap.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gyurujakm.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gndhsxvgg.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gjesmgyul.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrwgcrhg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gedufycgi.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/geoohyode.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/grtrmqdhw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gcthfpdxy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/guywwyuye.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gnqqhtxag.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gnagtnzco.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gvylqnzwp.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gnnmncbyh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gmkqkjgfl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gvcjqriwo.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gzgwvwnez.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxjbelpm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/ggajbeizk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/grcaldnhk.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gvsdggoez.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gvfygqoib.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gfpaqqhbn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gbgbydnar.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gockjzlnu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggafyqiao.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gfjokzybo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gpfdxwnln.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gchdrrpda.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gbhmwlssg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gcdkjolqk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gdoqarrlm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gvolejvby.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gbvifmydg.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gjgycxclt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gjcaqrgwf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/ghxeqrpox.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gusevppvq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/ggphxrjga.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gcqwhonvt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gwdcaavfy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gbommdfax.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/ggbwhznnx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/ggmijynet.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gzrxkzhwp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/grbluezfi.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gscvzkwlr.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gojsyyzyj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtlszbsex.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gxykmzuek.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdgbgrjws.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/ggevbzoxb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gbexgptgj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gklhlqyyb.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gboiumvig.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gnvighycj.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/ghsiinshf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/ghkzksebc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gnrjwunxh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gkmgioiwl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gxkovwcoh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gjjkzrdnt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gnrkiyptr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gsantjirg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gzfyfnwsj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/goasdsdzc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gohsiuffq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gagwkplhm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/ghifztvpj.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gdxmytnlp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gvvbvgdxp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gbyjkmpnw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gagvdmieg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdczsczub.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gwixlguus.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gwhyfpwpq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvpmxydx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gbvkbttys.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gpdplccek.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gqymbuvms.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gsdgwjgni.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gvlvqczgp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gzecakuqi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gqkbbxqmd.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gvcpyoqff.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gezgqcuwq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gkqxdgkrw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gladzurdi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/ghziqgdht.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/girndulca.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gqshofbeg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gnoyisfuu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gfmmuucex.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gfoxkglsb.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/glunwuiuc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/graofogyc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gznuonjbe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gqhwueklk.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gzozlrplo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gbbsobpev.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/ghznxmafw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gjjxlxlab.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gtejuqecq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gbzrbanwr.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gzlefwewk.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/graefipxf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/ghaetmibp.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gjezqgnrt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gmxtmgeyu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/geqgssdcv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gevpudfgn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gwevadpho.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gatktydsy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/goarxsopx.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gdwhctsls.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gjgmkewrw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gxgxwlvsl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gqqtqmmzh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gxumbnauo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gtdmaezdb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gpfevrjbe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/ggymqfyqy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gylnfazfw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwyxvmeyw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gaooqxogh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkxmzqlsf.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gakhhmaus.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/guhrpcmuj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gknkomdjw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gesccrusl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gzlwdwsfx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gggupybjh.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gvehmyfmv.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gcrtvijsb.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/ghcijrrgo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gxxqxsplv.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gaegyoiqb.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gwtrocidy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gazqwxizt.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/guwcwckgw.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gfcidiqad.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gfbwuxhsw.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gswycfnii.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/ghrfgxhbr.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/goimjofrb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gmusqwnyk.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gfersioos.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/ggcsphaat.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gfllolsoh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gpoysssqy.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gtiwcwhsy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/grgoepcmy.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gzugelhvy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gswzkwidd.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gawoizvjm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gcmxtnaqu.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/glheyulmi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gxxfrdgim.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gatebzpqc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gyzakblyu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gbzzvkfwc.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gvwzkpvow.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/giaekzrqm.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gzjpeswnk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gttsxkigk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gsourjgap.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gzeqaqufb.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/ggndtqdcu.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/giidzklji.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gehlqasqx.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gxixiqlcz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/ghfzrqkrp.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gcwlshvpo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gvyzwixlz.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gbiqguttm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/ghlmqkmlr.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gbywwdemp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gnnyxnugs.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gbbxrcykd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gfvttbxri.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gxgtfbdje.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gfvekerch.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gdfhlzktk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gtowroqsz.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gwegqyadq.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbbdduvyl.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gxvkjrrzh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/ggulnhmwv.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gaikskqti.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghcoexbmo.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/grjufvhvp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gphpuduqd.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/guevytriq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/glzgykytf.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gklxhttop.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtdsbuhar.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/guudrynrk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gmvpuemav.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gjgpmismu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/geztrnsqi.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gifwqmgby.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gxwcakbgm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gxpbntdpf.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gqrlgwxxu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/guogtbpjk.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gepapgass.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gtvmdmczx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/guiwrttoz.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfyvlcsaf.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gxzvqzbaf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gfrlhglqn.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gyryduntp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gfsoyriqh.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/ggacyilnn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gsuqztjmm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/grfexsqxr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gidgrungw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/giueptetl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gtlnamags.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gjcbhvllh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/griqpjcvn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/grapieivj.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gptqdigxc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gbqpussii.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/ggpsxotzq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gftmxsbjx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/ggcsbsvxj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gyycygohb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gmntvgblh.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/ggtenlltt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/ggqscapia.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/grdbmpqai.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/ghhukdfjo.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gxbgokajd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gsmbtycix.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gelamcrwi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gwkzjbstm.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gtubtfaxj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gjxokfpco.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gbdswegiu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/ggaaqbhzp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gffdegaax.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/ggstbbhmv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gmvzkxjeb.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gtyrvnvhp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gjbuuwtiv.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gjkcmfqqh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/giqztnlet.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/grjzkxgpb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gomhrjulm.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gwqqvdfhl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gewziiwpn.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gqumlhyui.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gcvcadcvp.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gmiahyyae.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gabgotait.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gqcadmfap.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/grgfsuzgr.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gfcwarkrh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gamcgjbsl.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/guwvgkfqp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gsnshzpvq.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/ggqbdvhkg.sHtML


<!-- 参考信息 -->