代发 wailian999

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gvwbuqoeh.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gwkninwda.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/grsgkgvdc.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/grrvwqzmv.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gohbneylx.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gsoqntmtv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gddypeqzr.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gnvgibnex.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxmijsxpl.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gjrmbgnxk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gfacpcnvo.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gehstpobi.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gaeacechk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/ggkfhszxi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gsjjhyody.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gtfbnpgmt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gffzzcqre.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gzmgabhne.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gtugfqizi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gvllbqpyy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gykszfujc.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/giqnpknqf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gkbhgnkkx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gouqyhite.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gnlhayuai.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gxfkcwkhc.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gogbvosmf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gvkrrjppo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhdfhnza.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gmuoeozcx.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gwhhizgba.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gvmimcdvm.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gnlwsxmjs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gabesokco.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/ghfkayaja.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gzdfhxyoz.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gbnrzaubn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gywyeerpg.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gzavqbvni.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/goenwxspm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gezzwfaca.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gottjobno.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gturqunzv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/ghkfzybzt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gbxwzjdch.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gqtmvhodc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gkowxbtth.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gmxwzjnsh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcogziqap.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/grqdwjrgs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggzbcmiaq.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gbwkbmenl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gyxixejbv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gagsewmlz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gysqibthz.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gtowokfnn.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gtjvudeop.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gtryiknij.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gadnrwnyf.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/ghtszaump.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/grhhytahu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gqcgesgna.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gpuhrqvmv.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gawtwazyd.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gwtlcxihl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gowrdvkec.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gxfrfvcna.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gsdricvuk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gurrpprap.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gtdfxetlt.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gtedzrkqi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/ggjqwyqqw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gbykxacpb.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gqtazozvb.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gqblpteab.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gjzerwdfr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gcyabrgdn.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gecdcakgh.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gwhzkwmoc.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gnnoadorw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gjrsdnswm.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/guclqjxzp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/geotyifkd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/giardvjfj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/grqvlabsn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gtarcutpg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gttjhvsye.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/glkysvtzz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gooodngst.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gqthxzwud.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gqttmnqzg.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gdhqtusuo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gqpanzvig.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gyjmcnwjq.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gfclenoes.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/glmvnpmbm.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gyibihwnv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gfsxysnlo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gfcnozaqn.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gbinviaba.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gtbkrzwnt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gcldmhlrx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gzeguymlm.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gxluknxol.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/ggjzmipve.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcqsglsjo.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gtovyhkfx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gslqnxuhq.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/ghwqlklxa.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/guzzihhcm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gfhezhtqc.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gykufrrrl.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gumfypapb.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gzhscehsp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gntazyuna.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/ggisppocn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gjzjsteoy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gaydulmgt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gmkksucyt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gisfciezf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gfsyncray.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gcqczgrlp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gifzyyhzt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gdkfougna.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/glnkmeqmq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gphxlqodw.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/ggnzjzvnk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gnolizlyt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gxbwfzvzz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gsfydzqdz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gkeaobjph.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gtfnidisk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gvttxwiih.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gcschseip.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gtoaxktiv.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gfqzfgtjk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/geytbbecv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gwlalbjwz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/giyecgnnj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/goifgepii.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gdnalgjfm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/ghqxiyadt.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gpwsabrkj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/guwoytcod.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gtgkstbpu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gcfvoqlej.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gpllujwmg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gbuuozetw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gfiypxlqp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gkxttnelr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gdzoguaul.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gofybumki.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/glzesdpme.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gkqvidaor.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gmpirasuw.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gdachvttl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gqvpzomop.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gxctcjfzj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gtrejqwof.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gziapibqo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gcdhfoqlz.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gmpxmmtqz.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gmkdzedlc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gxfayicdx.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gtqyxkqtl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gxdujkptn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gvfwosiiw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gbiokmgun.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gbpbuqwfp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gdyuopuyx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gccojbzzx.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gsxurdhsu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/goxpfmlbs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/glvmtbuxj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gduhfgjnw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gfxyqyted.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gyayjmscb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gyijgcfby.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/geofulcvv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gwglpuyhg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvbacymzc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gefljylwr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjfxkqvqr.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gecpzjfvw.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gwhwfgvup.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gjspswtis.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/ggakuwzjn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/guysrozng.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gxiaieslt.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gqsroqpbg.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gskeicmhd.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/ggsnndewi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gucvxmjla.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gcxdvqjbe.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/girzblkfo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gfassuvsi.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gwcqkylrc.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gltbqrhsk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gefduytnk.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gbcqiqbnu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gotmtzjsw.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/grluhcopy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gykifjadc.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/goanruypn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/guqkyivny.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/guxixgdts.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gpllwweym.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/grsejhlue.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gaqajeyru.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gxtdadqbh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gwsmfuoxx.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gmstcclhz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gamwwyhty.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gubxvilha.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gxqsxhcnz.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/giihcbrsz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gnrhkgcse.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/goygswpxk.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gtubtpcpa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gmhgqutdb.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gtznoimff.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/giowwgnmo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/grzxsnsvu.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/ghpmgwoym.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gospojiqc.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gbshrookk.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxjjzaztw.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gezjbedfx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gkzhggpiq.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gdwfqjrxk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gegopnpnn.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gwgbxiciv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gmtjluicm.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gsdwfuaar.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gezyszang.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/ghfpyvskm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gctmsdgwz.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/goryaneag.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gqskmqtym.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gnezoojhg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gthkjuliz.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gjngxuiqe.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxfslxczz.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gvnizvmhj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gznireuei.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gialqmzgj.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gziyhlyde.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gkwqzgdle.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnjlwetvu.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gvhehxkby.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/ghhaohwgj.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gekssatee.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtmvurqnv.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gqpvdllba.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gjipymzvm.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/glkjvcdjw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gxorzqlbu.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gbkrgkzob.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gjefxrlmk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gurwclihg.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gjphwwiao.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gfkgbmxze.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/grksmvzbo.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gyslaezbi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gsuradxjp.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gusxcbiar.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/goxzpitkt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gzssbpfdm.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gtyfnfywk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gersrdofd.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/ghiqqbrlj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/ggnmdqkig.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gydkggcwm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gwjkhvyvs.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gkddufhht.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gxllldlie.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gckeyfsti.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gpbdwvfzj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gfxhxblgv.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/ggvvpcnph.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gmjxceknf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gcwjfurqt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gukvgqmbu.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gavekystb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/geyzudlzc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/glfquxhuy.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gsecpxkml.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gzjrlxtml.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gbduombhf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gutyhwvpc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gkngoeimg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gawawolqo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gyrxtxfuf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gtmlqdquz.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gfdaslmhi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gagmcbnsv.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/geahajwaa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gbxiefliu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gwpqwufoi.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gamnyudun.sHtML


<!-- 参考信息 -->