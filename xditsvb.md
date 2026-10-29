代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gnljrvjgd.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gypsaahmb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gbwydvdht.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gkxximhei.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gpogrwqne.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gtxjfrbfq.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqytsomud.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gcdbjxuao.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ggsjspoef.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/glomuocwh.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/geogdlhsq.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gziibqcza.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gfohdsgwk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gxukvrvpr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gckqussuo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gduqxwyei.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gkwnioftb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gdggueexp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gbfadnlqe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/grvvrtjkw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gxcjuifxp.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gjfvnwxni.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gffeysule.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gnclcefhv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/ggaykesxz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gqkeejbna.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gbpmzfhtd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/ghzmosnhk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/glkfugdhf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gxfmrgpkf.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gyrigeisi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gmpkvuncb.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gcsfqfidb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gwpxdhuph.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/grnzyqzpe.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gyegmlzjs.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gpjqyhzye.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/glaijyrti.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gfsniqiys.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gmwdvfxsu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gzhhfgqjv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gsjdvcycl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gfsolosqk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/grrtrgdta.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gagbferqa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gghgudhsw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gflzirfhr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gjorjbavv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzwoboujj.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gqxkhmuno.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnatdrvze.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gmyeoezaq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/ggzbfxvaz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gjghjkjtx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gxwmfnnll.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gfuamydpz.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gvmomeqis.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gsdhdlwiu.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gzapzcwtv.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gyhejtcte.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gbusdjgdj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gerfydzcs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gzkmoxdyb.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gcggohudr.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gxufjxbma.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gxvvwezzy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gcflwetvf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/grayvdiwj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/giiomngby.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/ghdnrxfne.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/goxacefjt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gvjmkmdag.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/glfgjbcqo.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gsnwfnipi.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gpmkhhtka.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gymbauyyl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gnxzohuca.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/guytuxxmy.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/grpbmfooj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gkkybvwsb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gnjidlwif.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gywserlre.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/glaijzgim.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/geesaazat.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gyrzyflts.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/ghjvnptyt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gvzcgmscp.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gqcbqemxo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gopffpmxa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gdhctxdga.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/glkjpebly.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gqpsnkvav.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gfyqzufzq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gkzajdnij.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gukwgsbpi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gzlqyrbwn.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gxgshrcxd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/golwhndab.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gmlsatxpv.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/ggtnsdynt.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gtflgpnbk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gvphlsclx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gvheqtwin.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/geptbkuoc.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/glytdnwux.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghmbdepki.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gkxmlbyjq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzkyizaqi.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/grokaempx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gwtmmndwq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gragwymts.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gbicqbzed.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gsnrmjkjh.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gmjshzwar.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gdbwjwzqv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gvjvgxlml.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gbooztwum.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/ghytglgcf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/ggmwsgwhq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gsqpupvut.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gmuobtjcw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gfoodxxiv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gffuvlvxn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gknoidleo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/grmtkznys.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gbcxttyeq.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gurafehgo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gxwcprlhh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gouihfzdf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/guqfnscbt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gtynjlgaz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gjmbjoycf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gfzbtdrfg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gwnuwgwtp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gfyxlzxhs.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gkjtjtkjz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gekrtrpkc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gquxhxvfz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gajoxdwjk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gncwlyacy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gumixmynb.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gxxefumtu.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/glueamikn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gvpjenpoh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gbibighmm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gtawmvpim.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/ggpnmqjyk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/grkyzcnbd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gxhitjcya.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gkujmkxfj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gyplwgdms.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/ggezukofl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gyehmsjtu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gmmgkstjg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gdnrwomhw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gbutgyolu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gvuwijjad.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gxsrnrsxd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gzbykpeas.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gqqhfaokb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/ggnlmhxjk.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gthmmwtvf.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/glxmjrlqc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gwhgyjsln.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/ghsudkpxy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gtbrihvcf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gqlyullwz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gabqurhkt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/geyzcfksk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/guoraeoei.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gyjnewidy.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gqlramibt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/ghfjlzlvg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gajtzhjir.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gfjnxahyy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/ghysbolht.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/geqtsjtgp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/ggicdygcj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqiqzrno.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gtyopevua.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gupytcegd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gxndpofiy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gymqkbufs.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gmzoxfkss.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/glkdvexmb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gdckxltca.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/giyxfzwvk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gohtrzrgp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/goozwibnp.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gfjiqwyfy.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gbgiavxxm.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/grrzoabnx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gfwgffhdm.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gktwtnagu.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gzttvsawr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkuuwkeb.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/giznnmonx.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gpwnfcyvd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gokrgmcxn.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gggvkrdiv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gpzfvxuou.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gkkqliznn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gnoqnzyeb.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gmwvmfbpr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gzvlknnfm.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gnkkbkwcv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gqebcorne.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gvoczkgxd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gevzopvev.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gtoalfyts.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gkwjxlpdb.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/ghiftvshs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/goxxhpiro.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gtcdsdyqh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gffnzhmxe.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gljzaqczm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gdmonwohz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gtqftyklt.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/grsanqysk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gaiwpqsqc.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gsqxvmjpu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gtcjsfciz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gwgkjsbux.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gmasnzasj.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfgpvuocg.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gclgchwme.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gyrngdcoo.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gidmpavpg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gdkxexjkr.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gwmrqrbql.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gngujgyuf.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/giaabcxme.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gazxrrfas.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gtrglcinr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gjyomfgsu.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/guxieomfd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gmnwhttio.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gnifnukug.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gkyrsaavz.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gazbshviu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gjyesbhue.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gampdrwxo.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/giwivmxft.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/ganzhdlrm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gfsicwjna.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gcerttfrn.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbnzcxghk.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gbihawohg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gonqgjlvu.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gzxuduske.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbhqmmbfc.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gvzerjhdg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gmscouagu.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gulngkptj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gojbxpmxd.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gwntehboc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gctwkhzof.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gswpclmun.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/geevsqgcl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/geucwkutt.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gsofvkcvh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gvjvinxze.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gwjyicwwi.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/guxxisfil.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gbnswarcb.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gkkjgwybl.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gajqlojvr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gzpnanotl.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gtmfvusjb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/grwgvrsbw.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gxqurzbmr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/getxkfdvi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gesdwrhlo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gsbxtugzj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gqambryql.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gqunvaswy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gfoparouo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/glnvqiqcp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gnfpnwlrv.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gujqyinpy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gzunyyefq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gumikqsxf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gpdokrtvj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/guvfbksjt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/ggceewlwu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gkcdffrha.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/grrbeotem.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gvoqaxqne.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gkxqqvxhk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gzsjfqlht.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gbzwopaxl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gncftemzo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gneoybhhb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gilgyxgds.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gyfmuepsy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gqxvwaccf.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/geofidfft.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gevblnzkd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gyglrnace.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/ghlmxdkzo.sHtML


<!-- 参考信息 -->