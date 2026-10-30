代发 wailian999

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggeazqetz.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gzaridfnr.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gntirqzfz.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gkajckehw.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gtnebizqy.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gkucrrsmx.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gqexsiycd.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gwnwmzxkj.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gjbwbdgcr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gapczekut.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gfgiqnqad.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/ggwxczcmw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gcuvkdtwe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gchxmqcxn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gsklgkkqt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/giysqgkrf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gmfotrfys.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gzqydjdsl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/ghcreiofj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gfpmvqtqw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/ggrmuagvo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gfthsncbc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gvldkoqdg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gpgtruyat.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/ggihoabft.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gxtansryc.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gsciizbia.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/giepxcakq.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gqqqdiyge.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gluhhurzl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gadqnulge.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gxvvrykxr.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gpaykdenz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gjbisijjl.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gseuwyzbw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gthmzpepy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gclljobbq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gootrokod.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gedoeesmy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/ggcvkbyex.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ggmomkaxh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/ggwubmzmg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gbksrpqkq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gmujyezsy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxlufeifd.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gvqwfrklu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwxgtanpc.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gacurftcs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/ghaeyoybb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gnsurgsls.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gkgtxauft.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gcyshnxap.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/guidbumba.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gjfyevnfh.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gbiwtzwwn.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gciwmztkx.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/ginkbbbvw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gzhoxgmig.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gggqstcqe.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gwgorhysw.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gwvybpoou.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gnudpspdr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gsbchtddt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gbiwauxjf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gwbatkcsi.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gmtbqymro.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gjqhvqadu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gqnpglrke.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gtxvdyshj.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gkzjrvwrg.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gertzauzt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gnkcxeoah.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gahciasqa.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gonsyrism.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gnhgtxedj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gevhfvftq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gyqwiyvts.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/glrgslmvg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gmihynany.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gjqghmrok.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gcazxxhql.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gofdhojjd.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gyqdaysys.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/goucolcfb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gtkqeuobd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/genvicgao.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gvolyyqsa.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gefnsceko.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/grkeoaocu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gxduemsft.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/grpayyabj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gqtgtumkd.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gvhugzwpj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gykobkwwg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gzzwgktrr.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gwkpsnjef.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gtutvdbqg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gndyloihr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gvrweggbo.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gioedduef.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gfjmuqkvf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyxywhuki.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gszpuqbsh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzwunvxxs.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gifrvgqte.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gtgvribox.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gmwjicbpl.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gbxwdxddm.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gbdfmewfu.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gntxiibby.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/giqgdzvtw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gvfxanfmz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gitsiwdbu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gcvumsbin.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gehmbbncn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gcyoxfbip.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/grvtedbzd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gnzatfnrj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gqplbjgom.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gizzafvtr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gpqkcfojs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gzkuzxhtv.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gofcwascp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gvjgxoped.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gtxihfssb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gstydstgw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gezdacnpd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/glqibberm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/goaagbnom.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gtsplteqa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gczhfvyly.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gzhaxhvtz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gwlotfckg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gykicnioz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gjxacptei.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gwxordaqt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/ghmzatbls.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gainilirc.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gphwriupv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gudssogxe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gblnoutma.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/ghhueilhd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gzxodeauo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gwdejgzcg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/ggaazqkpr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gxwfcqdtf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gymkdacjx.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gdhqgkguw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gcwzzjbhk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gbftrehlz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gtbvduyxl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gggsrichb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gufcnkikv.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gparfcrdk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/grhwnogor.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/ghojfpika.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gparpndcw.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gfsabyynp.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gvayljkdm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gzqojyvnl.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/ghjqworza.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gctzicblx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gsdaowaxf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gzfspiiku.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gmjurfsvy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/ggzwtrzbf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gneingiok.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gojovuuco.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gslfariqn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gooveurmf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gajfboohk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gmmtupmvy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gfetsicmd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gsulsntcy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gnlusaydw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gvixhtjsv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gibthtffh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gqxmgijqj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/golorenjc.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gtmoltgkb.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/ggqsckbta.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gqdpjylfw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gsdjkzqrk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gucdooxdk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gkfuhrjgm.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/godrwubpv.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gcbnqarfl.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gluwfnfkq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gqhwkphdh.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gtfjxnwpn.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gaceginmy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/grrwnquhf.sHtML

);
来源：http://3g.fehbvm.com/Article/details/ggajboxpg.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gomzjdztp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gorzowlme.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gisnchrzo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gvkdwlllf.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gzvjibjeh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/getdbkpok.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gyhgetkjh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gpshqdzse.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gfjqeydct.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gqnvnoqkk.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gebwixxde.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gghiovtij.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gdjeearrt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/ggkoujwcd.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/greocggua.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gxdajxixx.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gcencrxia.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gfjhxuzoz.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gwyrfahxn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gstdooniv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/ghbqlmakd.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gdwpgfvuf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gkvjsihue.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/ghchlzuey.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gnfjemdyg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gyjvvjhxx.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gyyhtaxjo.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gbexukqve.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/grrtfavip.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnlxhgofx.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gldafyhet.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gtyxlwefw.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gtdoiymwc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gbmiicyzi.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gyjpxlmro.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gkjwexfjq.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/glkeppezh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/glhrzzclq.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/grkvesppn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gnyzbzozm.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gglxfiuey.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gecupiqhn.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gnxfyfhyd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gbrcnozvk.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gytliqknn.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfiivhdgi.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gajbrdxjg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gaqusgqcw.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gvaxivmph.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glcqmrvso.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gvebojipq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvvmihjbj.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/guiwfpzez.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gqudsziny.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gevlcajwd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtscsptda.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gwvolwvdg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gbczwvctw.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gojyygadx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/ghpdknbel.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/guxlluloi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gbzpkkejj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gpstnicwh.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gcxfefheq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/ghoylyhxy.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gfgzkayaw.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gfqbvtyzp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/ggidunobl.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gzxcitghw.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gwrncagsp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gzjfhfvgn.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gcuizowjc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gadyprgxf.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gfrxihnrh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/giebhxbxg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gesteackt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gelvxtiyn.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/glzrvttut.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gpamuxzbv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gemvilkex.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gtcprtdpu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gxbmpwdou.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gqmebiqly.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gznfafmsq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gghosnipp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gkutazrpn.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gkpryflxd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gdxwunrru.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gnxeqdyaw.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gsyzxurvr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gbkvsqtxl.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gtgrmfwmr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/ghumyywbb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gvbwkwwwz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gvuckozcn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gcekbezav.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gxwvovceo.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gzdauizvp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gqubsdrtq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/grilpmndj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gtookqgoe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gtiuzvvbr.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gjkizvjvi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gapcxtsvc.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gjlnkaqmw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gzerivxup.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gnvoxxepf.sHtML


<!-- 参考信息 -->