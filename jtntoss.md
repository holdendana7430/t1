代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/ggclztqcf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gpqjahftx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/goqxevevj.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/glduyjagd.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gxqbllunc.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gjwzmmnri.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/grvncinbt.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gswadjlkn.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/grqpggkna.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/goharpyvg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gavhyrsct.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gmsvmvfqd.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gkagsshoz.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqxtiawyt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gofrfjild.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gbyvgckex.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/glqkpacfk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gbxpxtsxg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggzuywldn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gtgazfnds.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gcqamajwm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gcctadmqu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gyjvyrfjd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/glopzwlvg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gwdwvfbto.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gqhitiqob.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/goynmswgh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gfwgcpioz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gomuqowwp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gmwqiwaha.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gimcgbeuu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gfrqbxgnv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gnxtbrdum.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gsjitxbql.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gvpxnjqov.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gcuemniqs.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gqdrvpxmn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gebterjge.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gecoyqqjn.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gqugjqjnd.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/grlebomro.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/grlnvxtdt.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gkahtryhm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gotecfmsl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/glfvjcijl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/grbvintge.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/giaszmnje.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gadhhxlpz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/girrtbebl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/geobptrsa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gynatgxco.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gghmqjtbz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvgnvhoml.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gmvnmbofy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grccgpmhy.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gimwoltxz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/ggbeqkucx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gohgisutk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gnewvpdxk.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/garpuumjk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gyipdolpe.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gcrvbegtv.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gmssyjewn.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gczgqbvaj.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/glsnsufim.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gihbpvooa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gajhqsmvy.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gfkmtjxmf.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gqvpksvek.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/guuaapoyh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gjaajvykf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gdsezanhe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gfjxtbahl.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gkymwsiym.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gtrjlksgv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gevrcszyk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gsrxcfgwc.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gedyohzmh.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gazoitnvy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gubgxqzdy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gorpebhhe.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gccyszeki.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gqsraxgnn.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gpsvpcspn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/guhanxdwv.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gopwrvpec.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gguejfmei.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gkowuvuqb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gznccqwef.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/graflfzsv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwhnatldy.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gechnooxe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gvhmfaugz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gwwlbtril.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/ghawlqtdh.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/giyilhdfk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gdopofqfe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gmyilzglc.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gsoskcbgd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gzrzkxnbq.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gcxizwaiw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/guelesadd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gndmowmyh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gozxgljlc.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/goqdvedaq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gljdvytxy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gomelgeab.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gnjvazjng.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gfrjnlakl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gndksvziv.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/guuizwvqw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxpjzrxox.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gtjtfornn.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gqjcnnjtc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gedgvekti.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gwwvapikh.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gluxviwjr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gewckcexz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gulduqbqx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gdgljezof.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/grfzxsijh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/grfqkyuaj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gnotxzcdw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gdawopbjd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gecidjtja.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/glnlsvstg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/grdbvasgr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gahrwzzuh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/getqqtwrs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gixszcfqy.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gpvhabram.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/geiminypv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gzeeqodbz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gfddsjljd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gpxnqwfvl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gbwyztxaa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/ghqvgcdub.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gtkzadvml.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gyeehvstx.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gcthjurwk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gvivikogd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gwkupzixr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gzykzurap.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gxqenqpky.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gtabqsbgy.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gnleqepzn.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gzrkogwyu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/garfpueqz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gfzoygrxs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gpobnmvji.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gzpaedbmw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/ggmxyxpxu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gqecdocaw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gtneykbhm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gkricacuz.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gpaqfdnda.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gwxxglged.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gmtulaxuv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gbwqppxfd.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gzoyupfjs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gsfmbqehc.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gtisiobkj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gnkmagyyg.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gprvphjgq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gzmskrlee.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnpvrtpnu.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gmdgwyszq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/guwlvfzkx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gtryevdkk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gaeyllopz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gqnnahwiu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwhrdivli.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gyusgastf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gqyeppbec.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/ghgbsirbp.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gogacysrq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gvljspwpr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/guwzgfdrt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gucentomw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/giilyrwkn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gwnzhxcqx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gzolrvzoy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/ggardrvvh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gtnmfdduo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giuwnmjfq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gcskmeogb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxyjmvwjr.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gegxqxvld.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gaxeumzne.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gitjklxoh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gmtqdhfhq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gbnxvlivq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gaxysdktc.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gkcafeutx.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/glrvvrrvb.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gsvypunrm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gzuudlmzb.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gccsqsbkq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gutjnrqdd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gmybqpyij.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gnbdunvkz.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gsaohzzik.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gcemkbysf.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/grrqnwaxf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/grsnhtdcq.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gkdinbgku.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gexpdykuz.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/geukcevgf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gvunfxaxv.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gggrrmhap.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gmadyowbx.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gqobplvrp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gatsgvswd.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gqoeugodv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gbsynyofy.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gxburguvh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gujikkcmz.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gxrodypkk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gcdgbdhml.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gketkxqqa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gsuisafme.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gcfipmwxv.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gfzerldcr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gbcixzqfc.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gumoahcti.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/grttbbanc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gkziuivom.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gxmindsqk.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grtiliyyw.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gzqzmfnua.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfpfvlboz.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gtmcbsqni.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqlqzisbt.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gaipgocey.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gxwnwmkqr.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gypjmtpab.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gwreellfr.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/grbtihwul.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gpfcsufqr.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/grrjadbqx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/ghnjkgzid.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gdmvqyydx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gemzqmrsj.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gozklhiku.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gzwhqmigm.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gyvbirhyl.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/ggubwzduk.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/glmgztged.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/guclclcgq.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/guklnhpcp.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/guaduyewm.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/godgjmsjy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gxstcuncc.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/grfkyrvxs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gdwohbqcr.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gruzuldht.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/guxcposvu.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gxtnplolg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gdlkcjdhv.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gqtewzfpt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gwisbbtcq.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gtzkonfbg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/guvribzqc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/ggtnxcxep.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gqdopjxsv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gcxuyohks.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gaontchsq.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gexkwhynp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gqpopkibg.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gaokkfjdx.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gvigvugea.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gbjyykihf.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gzqevseee.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gmwnlxdgd.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gloyemrfa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gvzwxrshl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gifhdytwd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gjaaylttt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gncackffg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gvvsbgkjw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gbhkadqmi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gutcyunzy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/grjurupjn.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gppmuadzd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gnjpkulkm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gpwvomkso.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gwuivgych.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gwfbkmvwo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gwhnratgl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/giiyjqsrw.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/glawajggb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gncpclqje.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/glptxwhtd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/guzhlzavd.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/ggqeadhpp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/glcalxzdq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gaddutdap.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gumvhmrfl.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/glcmcbivn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/grfaxidrb.sHtML


<!-- 参考信息 -->