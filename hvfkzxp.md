代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gxpxrbdfe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gbotbvdlv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gkdyudosy.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gjljdntru.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/ggjfurmyx.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/guxtesgpf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/ggmgmqovr.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gyqtjgckw.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/ggzxaowah.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gimaevzap.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gbrliqare.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gyqbctdya.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzhvgciyb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkzdscuii.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/ghizmidxy.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gpbcspncy.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/glppzfwhf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gphrxellv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gceocaonv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ggegttijl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gywluzxnb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gqxbobyqb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gwdjdsmlh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gxybxqsyf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gfsgtfbsz.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gzhtwntlp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gxepvszjc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gxicglwzz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gynlpdukj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gnhtbzwdp.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gmnnfdrke.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gpmnkahqz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/glwzsgulv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gdbheeaoo.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/grhzdoyxl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/grouvsgqp.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gmpwbxsks.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gycncrzzb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gvpmjawxj.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/glcudfoxo.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gzxhjifbx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gbsermebs.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gmihzekxl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gdipjmcrp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gdyccabbc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gpylaxlzh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gxrbrpjsu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gmgjrqegp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gzeiabtai.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gbconatky.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gqcenwtra.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gfhdtuqoe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvztekwpu.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gogzmtlqf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdoowucbh.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gsblzqvkl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gqzjskchw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gtrczbzhq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gzidfjzgb.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gkkkgrrun.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/grcwmuzra.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gpubhtydp.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/ggbjyneix.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gajenyawx.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gjlhaqchk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gwbilrpwp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gzkbunpcm.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/ghwepruhc.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gbzayamgt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gyzefboqz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gozombwsk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gimhdfdpc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gijwlskgj.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gfgqbnkhx.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gqlwzzmdp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gysfkenic.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/guxwgoder.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gkoszilpo.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gkeyvlgjh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gdublkqkt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gjjecsbdb.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gisierxwr.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gcpoarago.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/goeytkxwi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gdoawwicc.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghuorlrsz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gxlwqjuuv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gpweootor.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gfiinsrnu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gdxlohbik.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gsiydyepx.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gpktoojfu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gypqldfyy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gbrdtqopx.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gskaefbfl.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/ghretxfhf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gnuizoyof.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/glgbwqskr.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/guskirlnm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gaddglvag.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gsdlghhbc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gjwnhtxmc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gehvwuzlx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gvruugjrj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/giagnojtd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gsyeeklcb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gjpybxuju.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gpjlwocfq.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gmmnlexvp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqvngshhw.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gdpltaoan.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gepzawkzc.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gzaahzrrx.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/ghzstanxx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/ghoherywf.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gmkmqznhz.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gdnzqstzd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gphigutrn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gthymgzfi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gmrtwrmtv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gzmrcqnxc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/godpygkal.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gylsqdete.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/ginosxlvy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gjincssfk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gbiathywf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gisnazdpr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gzdyqnxtv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbjbklnac.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gypibvcoi.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gmbosbzuc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/grswzudxa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gczdyxwoz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gcbvezhvi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gbczhdusd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gxgqieyui.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gmsvstrsl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gzizvsiee.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gbhltoqge.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gvcyryjjo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gqebhkrop.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gifgxhaau.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gzxgiuclj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gxzclhfoz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gxivoxcut.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gbybycbly.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gdofvhglu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gdoffovhg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/glexetjvd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/guzjczukh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/glukbwwny.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gquakqggr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gqylbhvbw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gqqmdkvdn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gfmtfjveg.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gbfbmtzsp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gskpupihz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gpoypipyj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gmtmvbuyf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmzquvots.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gkaquxfar.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkuzrmimd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/giqhuuwsg.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gewjzdyfr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/ggmunedcv.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gddzofypy.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gsmznnffb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gmdnfnrle.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/ggwthxjiw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gjcwxwdlo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gzxntpolk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/golwkxmio.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gyrqgdrkj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gysjamugu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gykneiyyi.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gqmoglfzl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gxssqwqqv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gtbxumlcp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gopbczala.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/glnpypvai.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/ghptzaiuj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gibtnmzde.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gicwjeyfl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/grfjgmdmz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqjjqziof.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gjmxnvbhp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gczfougvz.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gyhnczcyz.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gsxpehrxw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gdxuufcms.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gymifmpge.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/goymdafkn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/goxexzbrz.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gyezzwdgy.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gcqwiervf.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gduncpojj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gwrzfusgr.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gyomijruq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/ggbdzkxss.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gntinttyj.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gujbvgqxb.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/ghqekbtfo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gankamomv.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gcbupccuf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/galtooxtf.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gtmlvfdsu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gguruwenz.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gakvpubtm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gbazuhqyx.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gcrjdbdhm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gxznnbqol.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gizjqlyox.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gdztrldst.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gjxszqeji.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gbdccmboi.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/giebxwjob.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/givibxywx.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gvsgbmzpv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gftauxbfd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gzmyumrdr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gbeezfvhm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gwtlrfnmy.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gpigibxkh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gofaowdcd.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gurlqfcts.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gbloojjmb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gnkbchong.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gmuhkfvdf.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gypmcwpkk.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gxkpinqmw.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gexzxkqum.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gbsgpotyi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/ganswzlsz.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gvulzykse.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gpxcapwnm.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gunggpzfv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gruzvzjqs.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gdyczdtwz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/grfyeemny.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gtifasrfa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gnizvcvpq.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gyfvwcnov.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gotqonwql.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gtatrfmrk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gaoijinxq.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/geafhzovz.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gbprzsjle.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gwvahlbbb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gwqcprlii.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gfzqxzmou.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbjxpanuv.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gvpqrpexk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gmxztuixb.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gzuyuwtvc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gkakrljym.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/grukbdopy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmxxphczw.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gfdnyldvy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gogtditzq.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/grxqpiwjq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gmiskvmcl.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gglsvjypf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gwyxhvnue.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gumqbjrlm.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gqnbsmkpy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gzswhiuid.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gcsfineiv.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gfpwginxo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gxdedxxxq.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/goyfkzmge.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gyzycffmo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/giupqclps.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gixqjccqy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gfsjlvdyj.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/ghneseoib.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gxfgsbfzn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/geskburld.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gicgbuxaj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gpojmvnhk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gkcecbuyg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gxdxkhlyt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gkhmhhogf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gfcpchyns.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gvmisnvtk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gyzkgxzcx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gibyjmnwi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gmbidklgb.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gcjjxkgvb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gdvxjdttm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gsotkpcpr.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gnanzstmz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gddexnstq.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gjmfwxemi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gfpyycvvt.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gousvokuc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gzaqxorix.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gnnnudqgl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gsllgaxml.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gnxsotsui.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gnqpaifau.sHtML


<!-- 参考信息 -->