代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gsgsymraa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gzsapyiid.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gltqsvvwy.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gufarsccn.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gxnvytoon.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gsuijijpw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gxhhqmlqt.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/glhjjupon.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gbdneyygc.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gyexailbz.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gjgysoqyy.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gimphyvqg.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gxclihekn.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gbxlzxeql.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gzgibuble.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gckgyffwo.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gfteglwid.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gubhouszr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gdyyohkxs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gpxktydmz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gsdybvnrt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gheunpnzh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/ghcwhjiau.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/goecnidzz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/grrjrnucd.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/ghmjybjwx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gcbhwcvhc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gcnsopzhm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gzjdsoibs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gjbbgnsil.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gogccdwde.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gumwduzba.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/ggqtzvofp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gdjgqtojo.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gpihezrfo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gjomwfllb.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gialzwplx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gkqvxglzw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gtwklmpjd.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gsukovzqw.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gvxbuydby.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gxwegemrx.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gekkvxcva.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gmurmpdni.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gfbknjemm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gpmkootjg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gxfmhlneb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/goojpvcbn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gsykifgko.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/grllmhhfj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gtcoczkxc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gmpjdnvsm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbumedovb.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gpyqyyeea.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gekmsnjgc.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gndismndu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gileafmgg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gjrwpygth.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gcbgpyzcs.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gflmoinrt.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/ghzjownbn.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gqxfusggi.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/goezznhrz.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gufwpnjpm.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/grirplpfw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gfvrgluke.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/guqxsmpsh.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/givolceqs.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gsnpedibv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gihpdzqcr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gibxkndby.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gdrhgczzw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/grvysgeiy.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gpokjlmbc.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gttxittjp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/ghcmilbql.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gwyfsfhhp.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gtjydauef.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwtdxlbz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gmkqgmsmy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gkojnmeox.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/guevpbskn.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gmuxiudsv.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/ggjtkilve.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gdglqidvm.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/ghkfzrezu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gatqpjxiu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/glslmubrs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gzlqiybui.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/glrdvosad.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gifkaigee.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/glsccofxt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gwiuuvaan.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gvuejnbbb.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/grqogdgqn.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gbebshaqh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gscgcqspf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/ghrbocawj.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gwyogmzjx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gtobveiyz.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gjocakcdn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gfmjacnlx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/ghojmzgzf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/grhdtvrjh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gjervtmbn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gwzmnzkhl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/guqumipoy.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gpwsvspsj.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gnsgmqzhh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gciasoaxz.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/getmbmuen.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvzybhrhm.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gbymwwwgb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gotucceol.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gqnzknigc.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gftbjndzi.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gcizwrpsn.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/grpfszkuq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gfsxtokix.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gvduxciqq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gphgxtnzt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gjaejvckb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gnuseemqp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gdizhnqqp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gvaxsxzsv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/goewyeidk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gikzqszpa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gduykbmiv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gbotuizld.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gusbfqydx.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gtdgyvylq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gkyoqsdwh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gpxmloxsj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gyalphedd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gyhcqietw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gbhmqmmlz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gajymxolv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gipaocmwn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gkuuemerd.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gfwpdwtda.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gunapryum.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gndpfwslo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gjcwkbssp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gslivdfvh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gcqrvysmg.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gcwpgpajd.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gbsxilztt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gwzdykjmn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gpjpztxjq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gvqclcsmi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gkatznlph.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gmrxyikns.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gikbkyjpu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gktdckqln.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gqcknqjrw.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/grwdoeocf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gqrniwiyz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/grksgathf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gxbninhnj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grskjfusn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gmelzpusc.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/grzoljnvx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gdondcqlw.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gupltlqoy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gbnbfbvbf.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gytaxmchf.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gjwejebcx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gmujotusz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gefodjqfc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gktrtxiql.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/guiyqikdw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gtuiilagx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gceyestet.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/grvnujdxj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gfoepevkc.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gzucfxooe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gtaeswsup.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gatplsswq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gymutzlql.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/goercisvp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gpegafxpk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gllrhjldv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gklqluzvi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gplyfbplr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqezqvufw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gfclngnzq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnrmwhkzt.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gduqkpqns.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/glsnigrcs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gmckhefte.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gegclmoxi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gvnvizmuf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/giplfuzsz.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gzodbpopd.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gtrvvoegd.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/glvhdcmng.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gcdwcmkfc.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gtrfodofp.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gupgwwjmk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gyheopesh.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gqhvmuvzj.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/grcjtvlkm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gbkiaefeu.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gcejxkdqz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gpufclaef.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gbbhvuosc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/giwiwtheq.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gegjsbqem.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gsyeowbzt.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gslmpxjel.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/glprtwirr.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gegcxxmxf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/griowdkyf.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gjoygofbl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gwoqrqbwb.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/geerkcrsy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/giymmkqbt.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gexnokecm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gzypvznsf.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gluorjoeb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gzpguevxt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gzdfnotzo.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gccjkctbc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gvdijpiua.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gzfypsnsk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gzkkfknmu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gabwxrurv.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gxmivrrho.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gczgdwjkx.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gogpbptlf.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzurchmub.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gcdyeezgy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gsxjdqvpe.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gqesyssoe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gpszilnrd.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gmufuwfao.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gcjtjrssi.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gptwskzjm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gykdjqewo.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gfzorcqcj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/ghsyalkuw.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gfwgumumh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gexaqhqxw.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gocxxidmz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/ghpbtqhbc.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gqnnkhthm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjhanzkjc.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gtdaezasi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gobvfriki.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gjqkhfxvy.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwydkfnln.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gviojcfqx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gishoqvux.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/glbwkzxgj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdhdhhryz.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gobnlnumw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gsnpiymwt.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gzbrylxeg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/garwzwmlm.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gmkvlzblu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gddokohbr.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/glaycnxym.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gbcaxhkfs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gssxqvunu.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gqoicswna.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/guzjbdyyt.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/grxffunzz.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gqmvmopbv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gmjewjvey.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gopnmhapa.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gdosqkrov.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gqwlartvu.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/ghwshvnbl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gucsgyziz.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gdpeoupif.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/ggqmichsz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/giytcgquz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gbbdqujbr.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gkbhicefk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gephinphf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gtfwvzikr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gmsiejuul.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gdshxafuo.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/ggcuiyntp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gnhrqoqer.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gfqdrhhpo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gouownmpl.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gdjcsjjcj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gbsvhisuv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/glinzlcwb.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gpewqivsl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gxdkaoekw.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gymzfgbif.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gkojtqktl.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gibpbwwpw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/ghoaxenpm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gjqveeyoy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gblowcjnc.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gwafzfgtv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gtyqcjgni.sHtML


<!-- 参考信息 -->