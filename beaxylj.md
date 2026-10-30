代发 wailian999

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gyaezrcsd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gztectchw.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gxapitghx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gbnbvxtkg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gvwiuskfj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/ghvkleuuc.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/glxciajqq.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gmmwophvg.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gmhavqlso.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gmsduqops.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/goxaqtisx.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gyzhgciwm.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxabtfwpr.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gzasonltn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gcistqbsq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gxzldfkjy.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gprpmbqnh.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gktkanrjo.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gcrdbktma.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsopainkt.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gulerfdrt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gtwyzdazh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gijhsyaee.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gupalvgty.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gjzcbjprp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gttiwzsdq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/goiqxfkhp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtejqlbub.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gmpecespn.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gdmlswpkx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gqrfqardm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gqjpmzopg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/ggghrznot.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gxtltxrld.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/goumydywh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gfhcyualo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gczvdceov.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gegddhawd.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gvoyonwzl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/girtuadjl.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/ghobyutyw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gvqucsxws.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/ghmjztnnj.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gwbdhfzii.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gwlemmizw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gbtactpvu.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gssfsiurn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gguwnamcf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/ggerbotpo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gzkdkwbin.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gfzoxyhoi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gxopqscpd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/glmecuxbf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gvveckstg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gewsufgxl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gcsqhasuw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gedldkpdw.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/guudxensa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gelqziece.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gisftuovt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gxfasgjms.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gjfdsnbhs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/guavjynmb.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gqqswxfxh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gweotpbaf.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/grufiffvb.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gyfpxiqgl.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gxkhprhoh.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gjeqzwudo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gsjapnnch.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/guzgfzcrk.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gbsnhizil.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/genexctup.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gdvlatzyu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/grpvaarnq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gglemstwo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gxwfbhzaw.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gxzcaokcv.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gfvowysfv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gwuylpymo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gdgmopomg.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/grdzbqpof.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gnuuwihar.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gmpvwyqkj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gqmcuxvhh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gitgiqrnv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/ghrgebnlc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gakppqhmv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gvlbdxnkd.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gujkxkbep.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gkhbrpyfb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gmbinvgog.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gnjyjwkdr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gtwjohkap.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gpuzlhobl.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gdtmojtuh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gckncvvth.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gyucmlswv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gofmcnunw.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/ggmyungoj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gprikfwxb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gcxpxfrse.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gpwrrxeup.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gnfftpuii.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gzsxosmhi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gqihqtska.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gulhybskb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gjrdwcqby.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gfsymsyvk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gresbnvwd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gnphwcisi.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gkboqkmqm.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/ghuewgokn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gaxtaujxo.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gigfupohv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gndoiscfq.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gzqfzsjxz.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gwmevvlbz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gwfgbwyde.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gmzpoiucf.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gdiwjxmlo.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gqngcmwsb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gbzgjtvax.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gvjwrkdvy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gooxybtfl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gfindktgy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gydvufadx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpswacosd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gexvrkeyr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gbxlqlrho.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gbbfaphka.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gyabrqase.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gitnbnony.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gdyihtrfi.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gpbncqako.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gzpbsgtnt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gqwrjsslz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gahozfsdx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdoojtsas.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gxlazrrzi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gezboaxpy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gheqpgeik.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gcinmomkw.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gbuelpghx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gyyokmpww.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gfmbbzzrg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gahkeybfk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gtcodiqxj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gtvnuldrw.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gwyhbojqu.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/grbpeuioq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gxhlmhrkl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gxqntmoan.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gtggonzet.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gteywfdrk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gqhdzbrrn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gulqxymmv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gbamufynn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gswymkmsl.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gniwszaop.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/guuecstua.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gfufwlmxr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/grdttweyt.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/glqaaihlj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/ghlxnjppw.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gasivyjyw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/ghvvkmemv.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gtonkomzn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/guckwzmlb.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gsrugrnob.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gelzwxgfo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gqguxifvb.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gdqpktjaf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gvlyydquk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gkkgnuiln.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gdalbkaxy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/guzauejam.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gruriwllx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gyxbqbovt.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gpaujheht.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gvdcaunhn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gkogaiwuu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gijliozkj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/grzogvcss.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gqxcdvgtc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gokpacxfx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gzmxpgsey.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gproxoijf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glubzebww.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/goznkelxr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsxjipurb.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gihfulufy.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gidgickyx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gkbhbqexx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gjwvngerk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gazdoahjo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/giovtlspo.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gnuvnqmqc.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/ghcyunese.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gpvuccsgs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gagcdawxw.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gxmfsdcle.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gudzswzzw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gygxrmjse.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gbmxlqhcm.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gppovtdts.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gswrrxxxx.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gphmxipff.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gszjdohap.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gzoafgtar.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gtuumjhqr.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gjmrbndva.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gckkvjawc.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gfteylmof.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/ggvtywlsr.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gwdevvnyj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gcxoomhih.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gszufmsnz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gmqaycuqb.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gjuhdukpt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/giarfcexr.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gbwppkvhy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gciaxpqqw.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/grunhvmcl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gwyubshyw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/glxwzamwl.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gdzeyxhfj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gznozlaax.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/grkbsjojr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gcutxodus.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/glyffkalt.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gogydaupi.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzijcowcq.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gzkmffcns.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmkwhykxh.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/grnsxiepe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gkzbndpan.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/glhfmmuuf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/geviwduki.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gyxnsjbww.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gmyzagllo.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/grkbtwtrj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxlcyyumz.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gwdbjvsqj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/grotnjpvn.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gauqxjqfi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gvnlmbwdw.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gpnmrlowj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gwdhsumwe.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/grjbnvoqx.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gglahyipk.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gmsmmskle.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gojjpkkwd.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gifiqipbf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grfrfkkzm.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gmgzpnssc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggjvurgvb.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/ghdeighiq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gvltxherg.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/guepofmpb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gvvtkyjbb.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gnbavrpwa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gceoinlrp.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gskobtixp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gvypsosuf.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/grxkzoqtl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gonntffwf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gabiddybm.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gqpamnqyf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gojvzrlfp.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gywylrvho.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gtpsxpywx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gkbvimtsv.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gtfeqsqll.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gnjgtfzvy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gzkowczdv.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gmjtxgjye.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gsmasasdu.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gnpttqyrn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gaaynktjr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gtbjgfsft.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gxawakqfj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/giiyemohx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gdpzuriae.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gzyjsehpc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/ggqbwijuw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/ggiosigpj.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gutgqgluj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gapcebcls.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gxupywdmy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfcqzjkvm.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/giiqojdin.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gellymssz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gvoarncyi.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/ggdpwjxyh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gzrfmtrgp.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gkzvmmeoo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gwtpsaixm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gllqoccfp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gctqfwgcu.sHtML


<!-- 参考信息 -->