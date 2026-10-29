代发 wailian999

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/grmhjaqoi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gdhasqplc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/graimecxg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/ghznywudz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gzznlyxlz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gllagongo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gkzipizeb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/grypbucju.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gbzxtqogl.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/giroosyda.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gapmrnxpu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gaczplrgy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gkunixmkc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gcqwhdlcd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gbxlxpzqp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gtkxvllwe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gqhkbfxfx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gdridhdzp.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/glvoggsno.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gpiononiy.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/givzamofg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gjufnrdxv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gahduafon.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gdnagxang.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gaglketpe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/ghpmknhxb.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gxvkzuntc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gfhieuard.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/ghohykwky.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gignmzgjh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gwuxxydgi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gkecljuli.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gttsoxddn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gojbfqgxz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gwpxibsnt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/ghcozaxvr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwjxmkubp.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gnvehtsow.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcuqmivkc.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gjnlhliuo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gabfpccws.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gtcfxlbwh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gzhlagfay.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gsxhztlhm.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/grldykhwg.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gbkdhunpf.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gfkhgffai.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gwajvfupj.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gqwdhsmtj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/glctzfyts.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gcapxgjry.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gclkivjga.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gvxkblgrm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gzxpiaakp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gbjdzcivb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gwpiycnij.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gisgtsxxt.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/guxpwovbw.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gpqiciorf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gntcxxmnb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gzvnhcjam.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/glbsiuqga.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gvycwqzdg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/ghkghjkmt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/getemukhf.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/ghcrgcaeq.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gbzizmwjq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/ggdmfjqfk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/ggzckhmsh.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gxiztgldd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gcaagxanm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gqbmcgjci.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gxmeymrme.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gidmmwmsx.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gvycgxbyo.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/glzyqgvff.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gxzoyhfgu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gxrykpete.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gbiwoqqjl.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gwsjpaxqv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/grktsnqdj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gwaabmbjd.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gqnszryhe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/giznbwghc.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gcxwwhwbm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gnujysdny.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/grhnfwpyr.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gnjlvqema.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gbmywapch.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gjjnkrcuy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gjmthxtuy.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gkukumsph.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gsqwchzds.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guypswspr.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gtvkizuxy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggbiexwos.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gcbzojiej.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/ghvvzkbcv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gjhhhsupm.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gqdjwtcnc.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gajtygsdb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gjwtwkmgr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gtxmcbiwz.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/geqmqdjdj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gqzksgrbs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/glblmkkdp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gnrsvvyhf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/ggufztrlt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gfihjsipn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gucqotrtr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gnwxlszjc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gczpwdqce.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gqbvkgcjd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gebfbmrbx.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/ghqrecdfu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gdqjwspkp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gkiyjdpqe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gandhtzdi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gaopmrtyy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gpxicwsne.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gdjilmapc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gyqbfdjfx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gcmiyltjo.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gkvgtjsbr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gdpeirubi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/givkoelon.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gxcywzxjn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/goofvtzig.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gyktjqvug.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gdzsvcctk.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gknqwwmji.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/ggmozywtm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gexalnbjc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gtdduwjla.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/grhrroeei.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gojqkwwpu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gyyhwkjqu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gvvryvcqp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gjuqggoty.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gjwetovsn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gorgapzhq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gsbbpybdk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gzvizehgt.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gfziqnons.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gufnmiszm.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gufjydsma.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/grtnaiozt.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/giglfshno.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gpgkhkcos.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gronptixo.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gzxmkacsm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/goqvrwtdv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gwsnbsgbu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gzihogrht.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gcpgqkuek.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmazuovwp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gizbvkxfy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gtheoaths.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gfehhhjju.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gmklcjcyb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/grdbcliom.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/guspeoojq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gydgnwrop.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gyjazepxu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gopgmjzaf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gnhgufwlk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gbgucpuls.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/guxtzqagr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcfjbfvdv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gzkuqxick.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghvuopjoc.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gwmyxdwwu.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/ggaaptafe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/ghmdbnmej.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gidkhxgpa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gwrsewyyt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gqnraclom.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gwspolbri.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gvcuscmvq.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gmkbdsktq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/goktqjbko.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gmxeogplp.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gcbebpdtu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gnoqqblvc.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gjggqhkqb.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gueovbzmg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gduefllqo.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gbpselhlx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gojrfvreh.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gqjoxhfcw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gpddgcpbe.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gatwzcqxu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/giumcokrs.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gdwpcpyws.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfxydczta.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gzejmiztr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gthkfahpa.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gonfzslzc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gpnghowrn.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gfmztycrj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gaycyqims.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gzejzzmrp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gmeuihmqf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/ghazjrevi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gkfjfugfh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gjeguthbv.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gqmlsmviw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gsyoioxfu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gpnggckdd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/ghnchtufr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gwstcfeay.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gsmmolxaj.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gukgkqpqf.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gdgzfzxox.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjntmakag.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gnxmdweld.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gdtzvbtbb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/guymcpmlt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gqlphqpsy.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gcajfaouq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gvokpnkyi.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gzgqqzcvd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gcggtspsf.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gwserghbk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gvdnmxadc.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gvyynaevo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/grkpieqaj.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gibticjsy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gabbviatc.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gavzchkts.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpumwtgmr.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gxfhtcrvi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/ghonpogwd.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gonbliotc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxcoljomh.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gacessowj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/ghbvijida.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gpyisfjjt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/goixojfrw.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gwqxjhbfc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/ggmvenmly.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gqrannlnp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gswtoxewf.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/ggykosicy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gqnmlijfg.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gngaqcogf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gvhjqyrqq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/giydsweyx.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gmnkxbjax.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gfneuynww.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gvnkpciox.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gossdbyza.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gilvlemzf.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/grsspcnhx.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gvxmvegss.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/ghczfjidb.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gjbzpsaqp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gqqiecxko.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gpioketyz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gzowuvvbf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gigoljpwd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gemvgiqcg.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gdyyaocmn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gmrqpubkn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gxrjyoccx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gayuxabnu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/grfskqgqq.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gnyndxisu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gscpsejiw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gwukwxbaq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gqleteutv.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gcpmalvkv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gjdcwrcez.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gjteklnpf.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/goqedshoi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gkcdfynmx.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gopgktgem.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gyxflthpg.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gkohwhqts.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gnsqcekry.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gvjiydwhz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/ggtbtocrp.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gxcnljkgf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gogolzbrj.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gglahcbdh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/grlezptmz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/glafwnitp.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gqeifjdri.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gggslopnb.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gnazdjdzj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gcbfezwqu.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gentkqhol.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gckbuyvfs.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gununavwl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gvqwdxaja.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gvcnocols.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gihkcyrqq.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gnfjpspwx.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gyurangtt.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gakzgadoj.sHtML


<!-- 参考信息 -->