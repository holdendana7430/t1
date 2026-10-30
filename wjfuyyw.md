代发 wailian999

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gofdpodjh.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gyoexcykp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gkmtibupd.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gosaedryl.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtnavnmah.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gwijsorvd.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gsadhyfdd.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gypjrvyeb.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gyyptpvmp.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gamryrtyl.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gntolfftz.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gyyylyjkk.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gdzjzgyml.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gwzvkhlak.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/glhdknvsq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gvotfpqin.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gajjaqlip.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gcixvitnn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gldijssmi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gwcgasetp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/glrxbshps.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gcmcsozkf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gdxgfvaqb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gyqzaufvq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gzdwskhhl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/giqzdeipp.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gikyphqen.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/ghqpmamjy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/ghyuciyhx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gwefuxyxe.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gyqvsybzq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gnrimsszd.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gehvhccbv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gjipanvhz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gtmptvjvm.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gulewjkwl.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/geoxqkrcs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gahyelvxd.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gqaguvuac.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gpnnfyinc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gzgeoxnen.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gltjtfwid.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/guqcrlsqr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gpbbpnarw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gqfthfkaj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gawcxrcob.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/guygnrylp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gxgyszmrw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggqikgfwm.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gtxunzujk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwuiucphi.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gmbcrompo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/geodcyboo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gajvactqw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gtowajzow.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gcgybqmpu.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gfighpktp.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gqphimznh.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/grhqqewtm.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gqqnciify.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/goiswdtsd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gifpgvupy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gjjunfixp.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gstrxkybs.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gqhpomewx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gaglwrgnd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gliatahrb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gvsidpqgk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gbdswskee.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gaateufjy.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/guagxsuza.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gxirezdul.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gcuptlleb.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gduovegjf.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gbfokpbuu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gteonrtfq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gztxmgzsa.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gidyaoqjb.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/grorbcfhe.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gdvpobyjd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gosjxrzft.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxjuffybf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gczqahmzu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gxwlwkhbw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gcxpbrtgt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gnjepubot.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gxvlclfaq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gzbgukqqd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gvoagqjnl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/grjojrerm.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gasjuumgb.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gouyrzejz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gqjguxwch.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gmzscvffv.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gxauwmhxt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/ggjrrufdr.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gkjwpthys.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gqdllgkab.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gywshyjpq.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gggrgokgz.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gjtukvxbx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gngdniyul.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gqacowmpl.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/guzpoczhf.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gqmccknyp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grwcpltby.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/glleiildv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdtmktzjz.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gppinhhnh.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gchepgjhf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gfpoommno.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gkgmkqksk.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/girxjaavw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/glmpfaqpy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gbhnnbyfc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gnnarhumy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gubomapvu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gfkwuoxwe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gsxtmkgne.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gjqchsyvn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gwltrdaas.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gnvisiyat.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpxrcuil.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gscxphrue.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/ggbsjiouq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gpxpyawcn.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gjhmgrbre.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gvutlvmsn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gurbxdyeh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/golistrfy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gvzhfaghl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gjcbkonic.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gtfrqibxo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gzgxetwhf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/ghffcswoc.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/grpybxyln.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gscucexbc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gwmkxkxtf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gqnukvzon.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ghqwgtoiz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gseycmklt.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/grejyomnd.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gbejqnrzc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/grnndmbia.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gzzjlmrzc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gqmpzhksf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gmvmsxvza.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gvizimudk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gsgzwsvyn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gzxkddofi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gorscdcrd.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gauentywm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/ggxxyrlrf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gtyuuzqgo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/geyumtbvo.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gehdpniyq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gfilzvuxu.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gepqtfjfc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gffuclyvk.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/ggrkfppfe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gbajpeffx.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/grmnsxxfi.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/ghfpkweiu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gbjtqhsni.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gfsmfmhag.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gcbenvuzn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gfqerbkaa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gkzenjgjg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gidltanhp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/geqammott.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/goqthmhgz.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gibpzpbou.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gkzykmsem.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gvhgjzyee.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gbgsvjgaa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gjasunvas.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gefocsmxr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gazqzftmq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gyczczvii.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gpgnyzajk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gikmcdgfl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gdgepgaaq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqkvmuatr.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gclclwvnz.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gzgygtcog.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gdnztlomn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gcgalntaz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gmraouzvn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gyistrjkc.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/glpevcwfh.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gmcvrswim.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gmwizosny.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gzsrqdccj.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gkivlnril.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gdcvztqbj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gqtdxwvsg.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gmsygqmkp.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gsqqxxdoq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/grfacsyxo.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gbwqoytim.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gtvvaefpv.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/glejvrxbm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/glberdluh.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gblywwnkz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gtxykbiuy.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gfolrxbcw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gqqztpeay.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/ghcswqjey.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gzxnucmik.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gnybxgram.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gnqzbefaq.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gfsozjrcy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gwfvoquiy.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gqjlobfuy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gdlxmjgko.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gykttpnyh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gpqwmwpmz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gsrxgxipx.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gyfumcehp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gxatyuvkk.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gjowqpjve.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gmsnshiop.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gfqjjkrhi.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/glrwtzhsl.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gzqyksdqi.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/glpxktgmv.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gyowqeurc.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gfyuggwjm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/geabkcxpz.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gfoetcotc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gnswwjusj.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/grgbzmaek.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/ghdenlbyq.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gyvkcutho.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gzdzvpdqn.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gdwngkvhz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/ghgxbzxsk.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gxoigvlbb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gviqsctmx.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/ggiijikbl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gfosykpda.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/goxghsxmv.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvylaxuxq.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/grhsiocmk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gkvlzgepv.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/grrdjupht.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxekblvlq.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gexdpmeue.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gyznlgdxf.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gxicdrljr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gzocsiirf.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gfmjsazfs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggizcixdm.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gyflqdhci.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gifafgvmn.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/genszezel.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gwpkcqpuz.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gephfjjvr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gxppaqqji.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gtghbpjqd.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gokqmavmn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gjbvpsnse.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gieovaste.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gxhfmwvlq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/ggnkembwq.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gkzhfnnio.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gnfftoctz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gebslczub.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gbscnxrbc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gwmmgvpvy.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gunficdei.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gfcvyzroi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gbfpllzqw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gmwxlqzcq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/ggyvebjpz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gcnwxqdnv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gxaqvyfal.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gzgdfgurc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gyzsgwoqt.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/grrbzvniw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/guokxkxgf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/giglblsxv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/guikweogx.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/grsbsroag.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/golqperhj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gnxyoqcjb.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gnogjdyjn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gpbgepnur.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gsvmlbpqe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/ggrllvykf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gqbvfwgtu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gaecymamb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gtahiawsv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gwojsmtxp.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/ghmpipbgv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gyqkxntlo.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/giojwlzht.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/giwomjuuw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gpdcilrbs.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gbtitljpr.sHtML


<!-- 参考信息 -->