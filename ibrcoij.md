代发 wailian999

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gzcdtihnm.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gymasswnz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gczabtyfe.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gwkfkcgkq.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gncgdound.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ghzqifaqf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gbyoerdsi.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gmyesmhuk.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/geevkfidv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/ghxltmexu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/glxhdlufp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gvzxzbukn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gxngdwpal.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gewxiazec.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/giulbggqk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gbeltzhot.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gsbpqsiom.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gfpfxwznb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gjppvpfjk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/grpglqcvc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gkwcdnxdd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/glolwtnwa.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/grlkaitrv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gcpwrlamc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/griskwcoe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gcnfamgpx.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gkapnwfuj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/ginnkjddp.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gmvabtsax.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gurdkfesd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gdgzjsbgx.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gmnaoxske.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gjybsaoen.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gjiarfefc.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gjkhihemq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gpooguggx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gvupkhkob.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gvejiekpb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gobidxxqg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gbucdjaoc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/glkigqewo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gszqvrfob.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gespmlwtb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gzlkvfynf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjttbzptb.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/grmevflyw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gblbujuvy.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gqdmsowgu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gfvzzmxym.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gwdomsjnt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gvrrmnody.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/glaktjyfu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gwmizhvoi.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gtetmcsao.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gsgfrtfcf.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gigsuewdb.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gxokoxvtr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gijnntmtm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/glnaobjzh.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gsywerure.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gzbksfyla.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gptgjnpod.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gjqcqxrvk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gihnyivbf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gvlqcscnx.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gssihrzej.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gkjwjxzjj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/ggjtfzzeb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gxolvkwhe.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gxorwvxje.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gkmichycn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gpcivduhl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gaamoftzy.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gvqgxlusb.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gcqykatdi.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/ghhvejcww.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gpbxkxqrd.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghekuwxjy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/ggrzkakaa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/ghvvqeacy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gdvhnewni.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/ghelssvti.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gyeymrazj.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gpoqdawen.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/goqdlffdp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gjpjbanjw.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gqzmfmpza.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gbmnzsgur.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gvaghvgzd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gotarbtit.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gksmfqqpt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gkjnfdijg.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gijasbjdy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/glrpzrrgm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/glprcojpr.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gphkzyehc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gaqqfpnno.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gquizvcvf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gcgkfelng.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gzmiqhekj.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/ganlipdtw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giuxuyejz.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gchtbnlai.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gowxuznmo.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gskhppvts.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gewvbtkkt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gozwjormb.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gzmzpgcju.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gjtnhkpqd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/ghwellxta.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gqlelhsxe.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gqkkbgwcz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gvgjckioo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gfixsfafw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/ggjbyftuw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/glxsuqjcn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gossdkfgv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gbjptjbnd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gfqwdzdzz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/goadjznlu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gwyrxschs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gtfdsjhkl.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/ghbnphczr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gwoqsevti.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gufkncvwu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gfvnxtrbf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gvksrapxi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gptsmpfqq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwcvdkb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gveuimmpv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gltkjuoxs.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gabdcsxzx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gwjwgzgai.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gxewfsgeu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/geriijrbh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gtmbqzibt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gifgcawbz.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gkjnpwual.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/glpvjqvlr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gfghixzks.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/glogtsihn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gxkuygtsp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gavuowgsn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gsqvqoftb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gtlwmxmsa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gtuepqpjn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gbnlzmczi.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/glkowxobe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gdjtsbckc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/grhwuyyvr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/genhpaahv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/goqddmuiw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gqccjonld.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/ghdkyzktp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gcjvmmops.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gylrddpnm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gecrvrgvq.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gxfauuzdr.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gwyyswayv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/glyzoxeot.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gbsanpicr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gbtrpsjpi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/guesvmwrv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gfuwcjedz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gbyooazot.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gjcshbiof.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gjkoagdrk.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gpwcriumi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gozqgseyu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/ggxdcgwle.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gfvnjnrka.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gjilvyasw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gzbanvoap.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gvpmdsvmt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gbmmrizwq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/glggwwujx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnwitbldo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gpygfkvys.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gclqawkru.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/ghkrczjnm.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gxqmkdihn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gnteuglur.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gxodpijos.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gxoqbvrdl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gkrahfzzl.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gyqzhtxxv.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gxbhqywof.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gegfjcxlt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gqfedyymg.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gdivslgrz.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gfyuaycau.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/grlnghgqr.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gahvrgeyp.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gqiasaypl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gbwpbnkwb.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gvbtweuec.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gvzujgfec.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gfxtpemae.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gyeiyobvz.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gjdxgkcan.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gjmzolyan.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gmqfqvyke.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gdatkjdrj.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gstxzrtpa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gwwzxlepm.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gadamsxxh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/glxtjnppp.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gctnoyqyd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gwzhbpkmk.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gcppqszvr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gbdjsdvoo.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gqyeagxkf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gmjfojfyt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gkbknhnip.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gjhrbetyz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gwsposrmn.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gnphxxgnd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gkfvfgezm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gzwqfynrj.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/goaujqdyr.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwzmtppdo.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gocpylipd.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glbnfroop.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/ggeagoolo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gefuckalg.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gorylwagl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gtvngsiov.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gsjbfxwqq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gsjgnnbba.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gidrjgcke.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gsiqputzx.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gzqvdbkxh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gylzjckyp.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gijklavwx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gzvjfkcfi.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/ggccuebeo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gcbcdiawi.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gzvshwsdf.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gnnhfrgjo.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gdpsdmlkg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/golyjrmjj.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gpfntkrvv.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gswutejuf.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gplvmgufs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gbsmkuesd.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gumfwqwge.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gxncixzll.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/govbksdtd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grajhfmfv.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gyyajehnf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gcndpcwkd.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/ggqpkrdpp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gnpoqfhiz.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/ggpfiexyf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gsrripest.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gtcglfrxq.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/guygcrble.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gaapeexih.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gfyfppesa.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gfwebxfef.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/grktafpgz.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gtzbvpkjt.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gwzmjlwvt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gjasbuwlh.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gfuhuhilz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/giwfvojcn.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gfkhpquqi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gsgsexhbm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gpydbjjsv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gdmzmmxtp.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gwnxdqmxl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gbpgkwljg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gwgrzjare.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gniuxifch.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/geaptlrwl.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gpezkurli.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gnadbuprv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gnicezarj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gwxaodytz.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gyxgvvrok.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gkazacqtb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gyomksswj.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gfbnpstca.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gsdlgyjya.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/ghdgsxfzh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/ghamwueko.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gjeqdvlts.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gwqodmfwd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gdjcxasqf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gsjxlkbwc.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gghapcxgp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/ggpedixpk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gordtgndp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gtsbceost.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gvjcmrued.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gjaazsski.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gzcgyniqy.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/grekrmeib.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gusozkjvp.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gtkuohghh.sHtML


<!-- 参考信息 -->