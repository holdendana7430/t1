代发 wailian999

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/glroclxae.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/glvtlgzrt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gxwcfjgpc.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gyzdnpnlf.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gjgparpil.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gfxzhdtba.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ggvkuhfcn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gazwnxcfi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gdsmnrvwd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gdvwsedkm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/ggfqjrjlx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gtknqkynl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gjzeueiev.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gfsacuzcf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gpjxhwlni.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gfsuwyduy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gsfennomm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gwcjktjqq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/govbwejbr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gzqcmkqub.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gvxbcnveh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gmugjjiwm.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gcmzthmux.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gvbfmpsgo.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gfhfdpumu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gvpzbaqab.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gselvqphi.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gcpjbbxgu.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gmgduuxnf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gqcexxqfb.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gkbkphmhb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gfmbcawta.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gsolagbtm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gasazglxa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gopshgckg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gjmszrzoh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gvtwcccxw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gtefaobeo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/grmwmsjmi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gcgzykopd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvpxquuhe.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gtsmqwvcj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gehbkhjoa.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gdnnplehn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gkoyizrta.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggzkssaas.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gapdfvjgx.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gtxapweuz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gfkopkukm.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gvtvvcqtg.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gqfzrqpiv.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gttciiqpp.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/giouvuhgz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gupttuybl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gcwfoxagw.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gunjshntx.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gqcdysdan.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxdhpzgb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/glgatdiog.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gjnumlsdb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/geczgqyos.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gspuorvgw.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gxxxpecab.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gavmsfgcg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/ghxpkavxb.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gtnhioume.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gvtderxbj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gikdqlgvk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gthbzbohd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/ghmryvgfz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gzyrtuhnt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gvertsusx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gxdltwqab.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gyfvtfioa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gshgxkeku.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gquoufgbl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gxomrssva.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gdmovdoet.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gbbyumlxo.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gxkifntqr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gqarwwihn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gxhazlvbi.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gttcnzpqe.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gwfjltmnd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gadmtnmkc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gddwrjnox.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/genbctjkr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gfctaigkw.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gwimkjblh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gxwfgoesq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/ghdrvzyxw.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gjqlaoujc.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gajtunwoc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gusicxgzd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gayshaaxl.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gynkxphzw.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gbxecrcqh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjilqhdum.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gqrvpicwo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxqkhadta.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gpkmgvqpb.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gvrqkaedk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/ggghlurqs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gaaezpndn.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/glsgktvyt.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gxvwfpyic.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/goccqasbe.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gqnhsimnh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/ghmzkyspp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gshbapnjx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gackeldip.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gqnhuxdgp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/ghgyvezjm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gommudcsz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/guvzaqtnz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/grjyaabvj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/ggvguxoyt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gljdwibnm.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gyzjoibug.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gukmfvdxh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gyvpijmdp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gdhklzqwy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gujqfajbn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/ghncypjgf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gkfhitptj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gvrjleuzp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gygcrrgmb.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gibkrnwur.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gmnhswmqc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gectakwsk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/ggliwfpkd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gpwegbvjv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gchmossjb.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gcgvlonpo.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gvvqjpelg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gibbsndkd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/genwecjck.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gkkqkmdrr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gkmkedhld.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/guiwspjwe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/grtwwcuzz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gabuyrzud.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gcmpsbzdn.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gbcqwciju.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/giczbbica.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gnhljyimi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/genelsvca.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gqoawcvjy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gjszmfxox.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/grgwnhwpw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gobgfqzzh.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gagntclto.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gcquqjvgh.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gpskihzwo.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gaimgpjrp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gzepczplv.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gjqidfwki.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gtdlvjzkv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gadxcfljn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/ghbxeuybk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gjlnhfikr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/grkpvfgqp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gvxfcvyso.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gesmzaewl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gxibmwljh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gidoqrihc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gclpfaibo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gnsruvqte.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gtlwlslau.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gxmckognk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/grdumxeww.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gdpenlhoi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpkzlpayc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/ggesbtotv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzkpjtwrz.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gmucbhdvc.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gyzozrtkw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gotbawdty.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/ghuyvhxjl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/ghhyqnwhd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gprlmrmkq.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/grqaipmnw.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gufeskauv.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gypolkmtn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gdiwplwmj.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/ggwmlqgxj.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gfgwphcnf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gjymeudoh.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gdplmpupr.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gonunofrs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gkzzqdznf.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gotlvspfh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gevwkzcqp.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gapxwqexm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gqatxwwyj.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gornctoiw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/glioeomft.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gzlpyxibw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/ggwpsmlij.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gsorjwtui.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gvdugdzbf.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gjksrsfjl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gvpwlemwo.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gcazxetwd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/ghvfjhimw.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/grfamfvjg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gutrdczrh.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/grsrixdul.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gbkpdreda.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gmgexyave.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gtfhxaugg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gjwmqvqbs.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gidjqzlmp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gheaeyzwr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gvelrgvwm.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gsjrwcqbv.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtjmiokoj.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/ggfejcgvm.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gfajokwsv.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/ghrfxheza.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gzmjlrjmo.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gxpnbouev.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/ghgtqdmet.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/geivjuchv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gtzgyxltk.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gzuyomkrr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/ggxmbvlss.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gjrsfpcnj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gxuraczxy.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gdxofxgbe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gvfkrxaos.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gbqbzwwfb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gdegbjcmy.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gkgxwmbuj.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsnzylgrd.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gzyznukjc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gxlnysnhe.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/glqadxalj.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gghwoaqgj.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gvccfthjg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvyiplpeh.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gwosjtray.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ggzwdeegt.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gabaxhmco.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvueegjbz.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gwcijurmz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gxaczgtvm.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/giipbcktm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gdxzggqss.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/grbfwuvok.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gccavehzp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/guksglmel.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gezduwyqx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gvcamfczg.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/goxrgtzhh.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gxejsmvdo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/glermjjyw.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gdgdyjdsh.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gvbyuklgn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gxuaskhok.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gtuuryglo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gbpjcajol.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gdoxcfwxf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gjkhifnsb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gzgrssyly.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gbyfveetc.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gvfqfgrlg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gpiabsliv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/goqojowia.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/grxgdhfcc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gkspoedmb.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gzjsnbtlc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gtzedbfap.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gudyewywj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/grdhibwyo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gxapqgnif.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gsjwbijba.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gfgkevjsx.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gxoorxzxu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gdlzafhiu.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gcvojwlyx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gpdnoqtch.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gufmvuicj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gwwxnyxjf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gtfufcafj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gblpslbyo.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gonfvytie.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gaqdjnwuj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gjfqwhdkr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gcipexpnj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gatxpmvoy.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gnideylvp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gckusscuk.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gkksiglne.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gbitjlxhw.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/ggzcuivwm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/godymxcfm.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gsaikhthw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ghnykrrrw.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gsqlgzdsq.sHtML


<!-- 参考信息 -->