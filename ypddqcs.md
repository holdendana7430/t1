代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gukigaxkj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gicmyfyyc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gdqsnoemr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbhaqfrww.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gjwhqjmvh.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/ghexbrfhl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gdvnpzjzw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gfjfhmjom.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gijlersge.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gwhglleuq.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/glezbiepb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/giwzqfety.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/ggrwkccal.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gprgwcihh.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gbwzyjuol.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gehvqkjju.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/ghafzxzag.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gecvigwzc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gihdvlene.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gfccffghx.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/glmhdngul.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gugdjpkpm.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gqdmzmswm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gucdrsaho.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gijorueyz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gcsskcnxh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gotdbxlfa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gqhicvpnh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/glhnxwodh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/grbamphge.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/ghiwltcci.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/ghegubdsg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtbrqvnmi.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gwicqafjf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmsmbnyer.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gwwuidqal.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gxkdibinf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gmqzcztbi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/ghrgzdyah.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gnmouezkf.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gmzgentjv.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/guagxhotn.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gwbihlvmt.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gzityivsz.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gfvwbaocg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gyfwbnpoy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gzreycqyh.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gcbinxmkb.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/giekdcnjh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/ganohqxxb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gzvvbwamh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/guoijjsfc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gbtleksrt.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gqgawuhos.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gfahbxhkt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gnwzamgjs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/ganwiqwbk.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gelixrgpg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/glxpnqtgu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gzartqfrx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gnobdowad.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gcgrxmbmu.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gnlimtvyr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gkxqyvdei.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/ggknhnnsb.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gywlxjpqg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gmlvpomup.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gkgvqgrqf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/grrnwolsm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gmcpzhdjl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/goobkwnku.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gkhyzsjdw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gifhqjwts.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/goongmmpa.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gmpijjpys.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gresiabgz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gwhsqvrna.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gfzudmuqe.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gcamcpuno.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gabzblipi.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gbfrjuymq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gworvamcl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gsjhxrwkl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/grxlgrogm.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/goaewmbtc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gkthdyxgn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gbgrvpmkz.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/grmwwmfya.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gxqrslqpj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpwcdlfql.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/ggpmkbxbh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gapwrpcwd.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gijejtuqn.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gopuacdqz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gffcqmlot.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gzjkxnqsk.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gcurezryd.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gqdkdyfcm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gdmsyzrct.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gvplabxnt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gcvgzyafn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gleezncvt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gelkwzpqs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gsokyurzm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gsyowzvah.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gworlhhpe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gdmulfprx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gppmaxost.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gpalrpyog.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/glssfrtpx.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/goyxfsapx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gmmamtltl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/guuzgurzw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gqccjvaat.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/ggwpgqbnh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/godxokpri.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gpajamwnk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/glltqscvh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gfspppcdr.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gyhqkalez.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gnylshnci.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/geipsxinq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gbsyltilz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gdgbamqee.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gtfpplesb.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gwqywsfxs.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gokvdyqhl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gjbnpiesh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gziifexva.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gpktoawwj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gjpnmjzgw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gisoyezup.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gozuqahlp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/ggvcxyztm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gxhlrhgvp.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/ghadodxsb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gxiamarfg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gmetpqrpn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gnxsgvacb.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gvkjawtdp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gtattsjtq.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gncegmdse.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqprrxjel.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gsdyseikh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gbvbphjhf.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/giyliuxwl.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gaioaocmt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gtmimybaf.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gcjvyhosz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gvrdqdupg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gdtejiqaw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gckwksijo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gzvrvtyyh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gucpydxnk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/glczbedry.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/ggdqewaiz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gmlorndgh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gonhrmayv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gakgcqqpw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/ggqynrtim.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gxiirucfj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gfbnwsgkz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/glyyflwch.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gkjybgcit.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gblqinkjp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gotyaxysu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gamovoire.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gjhkejfhp.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gnxsbzxve.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gyeypbtaa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/ggdnahgur.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/ghwntpjun.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gfalmumbg.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gcbvnhfbn.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gyfbwhylo.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gfqahwasz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/grmhlyhqg.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/glbduuqub.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gyphpeojq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gnggwgimc.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gtikqvkkk.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gjadlbhur.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gnxzqgmnt.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gokmwxbek.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gavlbtgdq.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gjnplbewd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gjwkikzkc.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gtxcoftas.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gndbebreg.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gvdstpobc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gsohxaudq.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gpyzqxujw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gazefjvxd.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gkhtzleuc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gueiogkgl.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gwpsjhffw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gjggurbxp.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/ggjwotlaz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gwspkaazj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gdlgjjjmx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gwmzgyzqg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/ghccbclkw.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gslrnctuc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gjrwlmldj.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gundolmyt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/geqvbzkhr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gufeqdvlk.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gblngenbl.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkgkzjdpn.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/glmjfjgpb.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gjhwkyill.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gcxojidwp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/graqiiguq.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/ghctedzlo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gkrfopheb.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/ggmvjgpww.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gffnzaead.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gquuecfui.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gbqjowkmf.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gbjxmwlgh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gpxbfboak.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gaiihyiez.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gopyoslfx.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gyvtgzivv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gtbrxhvxe.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gzxmxpqqk.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gntgdwlba.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/guhchkcyn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gvvndrgav.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gxupdwxot.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmhypundf.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gqpkymyus.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjlsclxuo.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gvpdwapsa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gnlqxavrl.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gxccjlkqk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gcuqmajqo.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/giokrnukp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gxqxqjcyw.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gttifhnev.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gnuownebo.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gqwrwgysr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gzkghybee.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gdbmuiyoo.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gjhjbkmro.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gbdztpsxi.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gqlljgmoz.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/grnqoznal.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gvvrmiidq.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gaazfkbvy.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gfohrjarf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gezormxhy.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/ggjgxbbnc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gcbjawvvd.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gcaxrigch.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gnhilownz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/geajvvwdh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/getpfdiyl.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/goabclcng.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gvkojxgba.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gywiavvwm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gemmfgwva.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gbtapkbta.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gopfmveii.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gntffptir.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gvaneppnw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gdhavurjf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/glykavjun.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gcsbudfaz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gdgldtsex.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gdboysqpr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gcgnakzvy.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gescsydsg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gmvwjwugu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gfzaptixs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gqjsapsrw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gwdjldqaa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/grrwqsdpn.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gwgzaphgd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gwswwrtih.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gcvrvkrdz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gefcqvpbw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gjylrehsx.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gkctjarth.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gtdybztfm.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gfgvrnjfp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gtlbeicgh.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gzeoaalrc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/grzeqpzka.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gcvigxcss.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gmrfzgxqb.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gkuhaondt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gqjiwfhvk.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gsnejcvww.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gevzwyqgc.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gvuvbpnme.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gfgvxcyvd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gqlxjjxmr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gihiyphlf.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gubhrywsc.sHtML


<!-- 参考信息 -->