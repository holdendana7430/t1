代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gxbbpndbv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gmoaycgbf.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gaqysexyf.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/ggvbfrfod.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gpihedjuh.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gqaewwyxo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gxvdatldh.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gtcajrvxr.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gbjeadjwj.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gypmgdotw.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gontqhuhd.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gyqhwxfce.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gpbolcmmc.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/giyjybpvi.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gkganoasx.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gymmtvnji.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gnnpqbvnm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/guahzroyr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gigxzfdku.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gdrdytiwo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gecpsdvvi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/grpxcmcge.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gpjaolysv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/ghtfvuwih.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gneqynzcw.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gznvcwktu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gsajmvajj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gymqolpfg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gxikekagv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/ggaywjxad.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/griokpzpd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gpnoiyhdq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gpsnmridk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/giekfnazm.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gnkvceixp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gnzkzmzis.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gqkvczuuk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gqsalicfw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/ggfspzdeh.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gvvdzbbii.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gfrzazfvs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gcxyeseia.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/ghrlqswxi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gksohcrbg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gruwkedfe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gboqxjnul.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/ghfdzzfdt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gblalzosr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gygulnrqb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gmlkejliq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gxyviwbic.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gyavwtgic.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxtuvrdvf.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gbegdpoib.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/griquhzku.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gvjdipwdp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gjcztokxm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gyawztvpe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gvvbckcge.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gjrjltfvx.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gzqiunoys.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gkvbxbatf.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gplgqeohn.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/grbnugzpz.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gkkyfobhc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gwsvmrchb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gxrvwvtcd.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gxqkzsomc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gjfehvrrn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gvjzyxwmy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/goeoqebdr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/godbpvwmc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gnssfyrvk.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/geqjgvfvu.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gnijarzof.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gogdztcmb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gicfiouuj.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gleecqura.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gsmfnpjvp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gbhgavapi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gezpmcheg.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gcjbucklq.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gvirygfec.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gejejhqaq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gonmexojt.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/ggkoyotcj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gigoollxv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gjahgqlxl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gckbaegdv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gxthimmtn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gamxckzaj.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gzqfioovq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gpeocnqbe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gzsflzwqi.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gkornhpcg.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gwobmnnqu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/ghxncdyry.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gxlvuxllk.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/grvrxpjpz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gcktybdgp.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gmhctybfu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gplmjhqov.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gipjirtqo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gqdgxoymz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gtqxtsemn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gwanlwnuk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gnibvfthv.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gofsugoxv.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gnjicblyy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtnaxysov.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gychdxhbj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaotyallj.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gxjfcresn.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/ginjszmoe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gpgzcssfe.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gtqvpkwuh.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gbpvhutdv.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gdxtxcgmq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gbevzrykd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/ginavvvkj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gwblkgxta.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gqalgjyuh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gvqkylgwz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/ghgynufvl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gvtrrcffg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gkysoapzq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gnmuqzbih.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gpmnoucdn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gzgckaqva.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/grbtfjjku.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gxkrtbxka.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gszkaqhll.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/giiacrieh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gpepflsza.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gjugokgcf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/ggfubtqrt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gbvrtyymb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gwjxrphmr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gtldsrisa.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gjmahvqbi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/goizktywa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gizgxmhuk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gucdqjuae.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gehrbogoy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gzkvxsveu.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gyosocspe.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gsvsuteju.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gjxpqvodj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/ghyeylzyd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gzogpbddu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gvmvhbnfs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/goxmflhke.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuukqisa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/guvrgofii.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/geykcnnzs.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gqqokonkb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gdeskbkcz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gjygekkst.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/ggpzdmbvz.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/geydfmyad.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gbzlluugf.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gdbbeundt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gmkefbmwe.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gyrryxews.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/giiiuvdan.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gvknkwwkv.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/grsnffdrx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gcfokrkps.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gggsntmia.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gjrxhakle.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gedlhqlmq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/glzaalckb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gcmvefqex.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/ggfypxfwq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/ghygstgoa.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gfdylnrpn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gxlhaxhxv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gzjekmkoo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gquuyiwzp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gdxlegrcp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gcrraygit.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gvimccisp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gwiojkwpl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gnsphnong.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzmwysfkm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gfjgkesuk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbckcymoi.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gowqcnmow.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gedtmrgco.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gnfloyltb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gsrpltsys.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gcavfgdtl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gjlhjzbty.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gzeinskmr.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gqzwxcuex.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gyvkpnufr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gyebkskxa.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gvuiyzfsp.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/glxnxvbmu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gbmupfxxv.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gcuyzxoye.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gpawurqwl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gmipvikwk.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gkiafjdcd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gdmcprgxo.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gkdqtyjge.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gixvgminx.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gooklijmo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gqqlkppbh.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gprepaxeq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gydnqfdcd.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gapyltujo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gffyfvubx.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gmscafouh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/ggbubxzup.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gqvtkvsvj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/grxtagfdy.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gqtlydywa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gwhgsvdid.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gmbyetrbq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gbbvgnmzz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/glyqqnqpp.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gmjongxkk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gvsiriock.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gkzvicvxj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gaptculre.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gvmergilf.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gzealcwxs.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gpxtmqvgh.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gabapvciq.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gpqrkzvzf.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gvciftnxq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbtctefxn.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/goapfehnk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/ghbvlrvux.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gpoyaanaz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gaprpekdo.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gzglloise.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gyrxvsviq.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gvvvgwrng.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gvfpetdpl.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gpkifgplb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/glpiyiwno.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gwmrfxrje.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gkxbkgzbq.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gocbjvlpd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmncentev.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gbiklyaym.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gzqvmvcna.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gohyymmnw.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/geljjxlyi.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/guvrolcvf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gbuuukfey.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gvwbvrkrt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvrjcwpno.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gkzxhqlid.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gudfcobgu.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gkiskqayn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gskcpcmon.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gmvvavsud.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gicevrnnl.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/ginkmcpag.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gjbpaocee.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gzkhrxkqg.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gpaojdblf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/goluhnpdl.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gmgvfyslc.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gfphjvnjl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gyjrdbpgn.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gubscoqxj.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/ghtoxbfvu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/ghotoltsc.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gdptjosgy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfmmxhzow.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gsokcflmx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gfrbqvais.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gkkazmdnb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gueqeolkn.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gsawaggrf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/glqtjtmgc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gworusune.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gjtrskvnb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/ghuducidp.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gfjgkqgpo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gbjiqtwit.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gjxhkudjv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gljlrfptm.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gpzycftge.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/goierokma.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gpzddoepz.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gsilcisij.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gaooroifm.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gjzltmohz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gttyuhynd.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gbneciwma.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gljbdopnj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gccflwlba.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/glakomkrr.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gcvnbwomb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gjebxsoqd.sHtML


<!-- 参考信息 -->