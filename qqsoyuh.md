代发 wailian999

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gkmppaulq.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gsdgcczna.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/glatfmfqu.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gtgzsdvsl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gchvcwebo.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gzcxpevms.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gnwdimblu.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gbdyqgoxl.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvvtiovbk.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gigsrjlip.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gcmuryhuz.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ghdfjxlpn.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gqlsxfqcm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gcpeqnkyd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gquwssbal.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/ggkrlwlep.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gzddcokfb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gskgywhvz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gvwlmbezz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gsmlhqhyo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gjrnpevdb.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gltwgiuyb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gwiesutza.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gfriouipq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gstbznskx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gejsujloc.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/grrcywaqw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/grnnwugcf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gewmdmord.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/ghaqtqyqx.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gcoqswuoy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/ggnuetwxa.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/giqbuaxsr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gyzfrqdfr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gxjurdamo.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gwfmhcicq.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gleixxzzj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gkexleklo.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gxanysmyo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gdhaodidy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gcrjkbbaw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gjpccfpse.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gxsvibswr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gjltsinoq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gotffhayo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gwraxmwtl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gqlswekxy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gzyfjusva.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmpokvwba.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gyyqqvprk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gakyzjvxx.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gbpnnjtek.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gfxspdcyh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gzulehbcx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gvezwjcmj.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/giyvniipi.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gqaupyrqu.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gengzdsqd.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/guaknwesz.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gppftqeri.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/glrmdpjuo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gzabcsepg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gjvijjdup.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gxwwhgwni.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gjhjjyfcr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gjqwphcmv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/ggwdimqql.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gvalylgqp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gksmflqxy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gziiezzpz.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gucufqpzp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gcmisrfso.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gblziciys.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gifwbtaum.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gshhtnuvv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/ghodftshe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gwprqvedx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/grrserddp.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gxfkhyolm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gkuymkvjs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gcdfefwlg.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/goxrmwwtw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gtnukkmtq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gxfwuwrgr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gdcncmnos.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/giijgeokg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxhlqjtcd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gbvndktaa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gocqiwelb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gtsrgxltd.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/ggjpglubl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gahonalfk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gcqjlkbcl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/giumifpix.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gifukdyea.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gpfzvuwwd.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gyprgosvh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gbxmcczis.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gwfspmtbu.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gukysabox.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gebkxmvjq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/ggfuyedyh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gdjjefzai.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/glmaisngx.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gwpjzmjio.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpnkyrnpr.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gispivomu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpxacrjwl.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/glsuxomjz.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gtphwkggq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/giijntbna.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gppbjzslt.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gszmvoomr.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gnjptmlqp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gkbtmivas.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gfbreorop.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gjoyibvuf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gtwrzezpc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gfdrjtfwf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gzzfymclw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/guinukjkk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gtsubyokm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gcygxuhic.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gpiqisufz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gxprvkbra.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gaivfuytt.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gplknxvpv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gnqzwlete.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/ghrmzsyze.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gcriskbxn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gnabbmzbu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gonzxgwgs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gdqlyvmwe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gpeepvkmk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gitxckgik.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gindkceaj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gwjvuflzu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gdadsiddn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/geohtgcjy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gnhtpyryb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gplphaqnc.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gusisvvvn.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gpvdyldzc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gqdjhojrx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gvyyojfnl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/glvfhqlir.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gwqaxhfcl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/ghyildhua.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gzrjpwbal.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/geiyaernd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/ggqjasslu.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gxciqvuzd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/govoqftih.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/guvdhvrhk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gihfmcqia.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gjwubsryw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gwwglupvn.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gidxisirh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmpwpmsxk.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gvtxoxefg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gquggusxc.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gaiulwlow.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gugsakibb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gnibhlhwp.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gyyhtdvtx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gcnemlsya.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gulggaxtp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gqfxaiivm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gzzaitpqu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gnpgjtjzm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/giswvxzbm.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gjtexqtfw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gwwkegmxm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/ghdshhsph.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/grixfwzwl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/glmtsevkn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gncfxhmkn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/ggndgowjz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gmzwjaflw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gbazqclhu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqrbnxfkn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gjcacxiuu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giikijmiu.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gvfgyujln.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gpybkueux.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gzflzjkgf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gyfbmbepl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/giupljijf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/ggzxrchef.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gzkycqwnt.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gzhwngszd.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gmgjnlssq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gxcwibige.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/giclevkrn.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/ghltwtqvc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gsijseean.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gtazdzsea.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gmcaahucq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gfuylsyfw.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/ghotrcgmf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/ghhjurlym.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gcdrzxjph.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gjmqipnzz.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gxegbhefy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gisdlgwjr.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gcqjsvmvf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/ggsnhwvyd.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gkxpbgwgr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gaykuyent.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/geqwyaslo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gocjmpapk.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gsvqrefvy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gywbyvnsx.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gwhtcuirc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gbrnxcuta.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gfqhdnwbz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gsmzuglvp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gxmikjelg.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gtbnbyqps.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gywrqmdha.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gcswgrmxx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gvyfwpstq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gixwnywor.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gaucqucut.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvuqtqntp.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gtwemyjfc.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/guozebjgy.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gfcpvnmpt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtwzvjurm.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gschhjdli.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gmysvjbvh.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/glanjhhrm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gqeguvadi.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gwbdegonh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gpidcfjyi.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gmibohruo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/grmiihwnw.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gcmyftkjl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gvdnhftst.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gpheypupw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gfaomofgs.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gcwgrrpha.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwdygmvxz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gscmfsrut.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gkubvumsi.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gxblvxscv.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/guyatwitr.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/ggnewvawn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbsqkemvy.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gdnfkaxjo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gfknnfmpt.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gjweujkgv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gbmshuzcv.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gcccvvaib.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gvfztuewp.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gfvceqiqv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gavtxrlaf.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/geajwnfwt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gicylffqb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gmjyuqjej.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gebjnwwvd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gfmhykbfq.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gchlbgnty.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gnvkvdvkk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gtvoalanm.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gqhuupukz.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gcnkxnuyq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gnpvvxrbb.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gqdpwedze.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/grozprqbm.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gwtyiawgu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqrxcobae.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gcmnctnfr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gpicusvxn.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gsdzwtbim.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gimpijlff.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gkbxnsdnk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gxaovyboz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/getgzhujf.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gdpaoyaes.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gdjpwxtbq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gwrcrsfeo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/ghodjcoqu.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/ghrzinpfg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gfwevmajz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/grbmexdas.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/ghwopjsmt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gpxwxakzq.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/ggbsasccb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gziojvwgx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gnjdvwqyb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gjszmphrm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gpkjwwspu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gbdschntq.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gvxxuiuze.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gqtkdxpui.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/ggqxwkqfb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gexpqfjbn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/grbiqfwnc.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gbwhpqjox.sHtML


<!-- 参考信息 -->