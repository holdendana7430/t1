代发 wailian999

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/guhunndsg.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gumxrmzoe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/godmslxfi.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gdgaxjbfx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gycxvnbhi.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gqsjuoixq.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gftdlhjgv.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gworflhda.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ggshbfcku.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gmlvbgniw.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/ghmvzpxjq.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gojsdugfa.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gsrfxkalr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gofmqprcm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gmymjtmax.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gbbjlsxkj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gynyfanii.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/geabqxhfz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gzgnomrwh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gmvqknqmt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/grcxftrtp.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gflegnnfz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/ggkgelrhq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/ggpsqwask.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/glkswujon.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gasufqvhf.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gwzbowgop.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gfgothmpx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gnrqdeymd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gxrorihyz.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gmwelofbo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/glnlxivtv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/goeuekpiq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gmxoyjrpb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/ghjnqpkhe.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/giyfxfkph.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gvworvlgw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gdqcrrbna.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gbfkaermq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gpphqtvwf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gbheoypgr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/ggmkctnae.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gmbaozvvk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gsviowxya.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gnxfstint.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/ggjqforvk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gmrmuakaa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gegfgqnlf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gubdmhpdi.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gbpzpbbsj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gogryeyhw.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/ggecuslhw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/grckueeoj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gskcwpgmm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gvgdhszzo.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/giqrfurxu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/guqmvtiyf.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/ggheliwia.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gnuszvodr.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gdhzsmcqt.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gahtyfbjc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gmsembtyn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gnsfunyym.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gsflweodi.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gwwurrpwm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/giaiwpulb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gkatgkzrj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gfukivpfn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gnkgwqhmd.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gweacetvu.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gqrbfrcit.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gjqzalksi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/grcplshoq.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gdefhkqsh.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gpsmfeoqq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/giigdpsep.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gfpnyxtzr.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gdmwkbfih.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gpcbghnbd.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gbltiujmy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gpamalbtn.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gvrucwexx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gwkmmeeqy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gxqdosktr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gwqoixkab.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/ggrheewaa.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gkmdyjtrb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gcrxnrerc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gbkldnyda.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/glxnxsllb.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gljcjiwkx.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gfkbrnwfj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gvijgcsah.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gbgukdpmz.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyfuyqxp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/grxtbiwcn.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gtsfgpjpz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gwtyiczdh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gofivismd.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/glrdhklvh.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gzzjkvkws.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/ggnmeyzyk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gvyhgkime.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gfrfhaumr.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gshsforue.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gehyumqju.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gkmcxxnnp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjyvjmwxw.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/grkcxsjub.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/ggcdqvtcg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/grjgjodii.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gpxjsajmp.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/guskaprrd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/glaqfxajw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/guqhtcebc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/grrkkwucs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gaeajdfhf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gdvopdbtq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gjvmontta.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gbadxmhgq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gxyzgcxfx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gonqidzmo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gscjnqrqo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gbilgfisp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gmeeawwmc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gplglcfbg.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gotvnmqbj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gsmawoegi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/grhvxqmbn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdqcrcsea.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gfdatnnmv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gzvydqhjv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gbkvglftf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gtbwhwhec.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/glyoqlubc.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gizotgzcg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gickxgadl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gpqamzelv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/ggtxazxhd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gjxqgitwz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/grolsjdno.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gpndkhbkx.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gatwzqemo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/ggfldqxzv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gzkhaxzom.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gnjtojayf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gzbondihx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gfjocazbs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/grsknrfav.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gcghzxngk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gyukvciuh.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gbbwfhnop.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gtvdkibqm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gsxudqbgh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/glkamwrfe.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gsljyczja.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/ggubguxat.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gvxmjjups.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gwocugqjk.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gurozmgoe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gruzmfqjo.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gfqynmjoe.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gnefmagba.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gchwjzhah.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/golhcwklx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/glcoehtkb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/giluisyxh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gvolyuehi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gayzctjoi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gtqnicroi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gvlxngcay.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gwrtcnljz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gniuiafhd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmmzijxrm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gaftxuthi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gaabqpaqp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gcvyrvzfk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gpkaiixjc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/grimdpcyg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gbkzjhlpu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gprwjxtlk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gxlflrans.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsyaokijw.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gtowccrhc.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gcorretvn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gdkgiagox.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/ghxlrtoev.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gzdsomtyo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gwwnalpww.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gxpgovmkl.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gdpojnths.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gslhngtwl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gqtujyihs.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gizkwgoyk.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gsqpgushx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gxotipbro.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gookeeawd.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gtwgdwyrb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gywaklkkf.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/glblikdbr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/glgzklxvf.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gftxylsqf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gydryxmfk.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gsfpeyezl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gfzebhrka.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gyzlkiupp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gaoupvrpd.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gptjwrari.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/getjajuhv.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gtucmpmta.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/grjgmlauu.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gpabmavxh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gsxtnogkh.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gvtyljhae.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqsicamqx.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gctpfqfdl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gefnrikaf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gozqecndi.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gnnojltju.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/grdhnkafg.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/guheqpxxm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gjifebauc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gigpwwecg.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gjxkahsha.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gmviibfvr.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gusdxsuqf.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/ggiabjgaj.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gdwgszxpp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/geyjvbjwo.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/goyuxtyhx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gmzkllktj.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gwnrgmcis.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gjyswfrij.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gksqzhusm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gebssukoi.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gftmljits.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/glxvgdvjx.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gdnhvwoyl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gmoazdjiu.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gbihfmouw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gadehitbh.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/ggyhwilua.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/ghxzgtndc.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gwilcjxtu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gqwmuurle.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gsagwhlzt.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gohjfpktz.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gpmgqlrmm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gzgrfmtnz.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gyfbnjwsn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjrnfxhfx.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gxoqnutai.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwklhukst.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gddhjwheu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/ganhsmonl.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gwjjncwdw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gxylzlqec.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gbsydrucl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/govhdbbdx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gacezxapi.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gszvheato.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gcxxyrfuy.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gqfqtvuid.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gfwglafyl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gchugikum.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gvombdbbt.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gmoodfbmr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gidpkskeq.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/ggsduqpdd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gvubcbzoe.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gqzemvcfn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gzamnfgbm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gypnmmdpt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gnkzjinlq.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gjduifnex.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gqhagbkgq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gbwnmoyrn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gzvdbnezr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/goipdvrlx.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gskkdawns.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gaekdcvwf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gzifoexxk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gcjofvpxt.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gdqntnebe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gbaremffv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gwwkiycdf.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gkxfukdgi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gtxuscbvf.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gxqbkgdmq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gvslwjspc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gdkmplczn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gjftybiau.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gdqszyicc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gqynutfkb.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/ghlfhrmtf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/guxyqlfyf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gqpkjppug.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gwmvyyyem.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gnmkhxwpg.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gyacjghdd.sHtML


<!-- 参考信息 -->