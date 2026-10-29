代发 wailian999

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/ghqxcghhg.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gsbcfmeuv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gkpsllfzt.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gwvwmtkik.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvbtpcjmm.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gcsszouqs.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gsxuofrmi.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gvvjuslfp.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gedmidqto.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ghopyctst.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gbcvhtjas.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gmqdqpaab.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gycqbkfmt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gsfqacltq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gknwlywsw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/goitwtgue.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gkhxvjmha.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gxenpuaoi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/glmxaiffx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gdkgasosy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gmsvyeudh.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gmninepmj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gvmqdqcvv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/ginlnnduh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gbhlbaznt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gscouaoxt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gjbueyrsb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gxlggnieu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/ggnhrumhg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/ggyyledzl.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gjbrzsbgy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gwlnalcir.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gcbvwixzh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gtmuytszq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gblojqlxx.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gnqwhijxu.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gbhwuieca.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gfmxbliic.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/ghpbrcbbn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gltbelkdy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gskpvpeqv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gnruzdfrw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gtjtlnwjv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gujvnbryt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gksyoblgi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gslcngvfa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gtgjttuzs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gkxubrscb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaazgnvnv.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gjpfcoxko.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grvdasobz.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/ggburqfke.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gircdbyut.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/glzonqhof.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gncwchico.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gpiughagy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gggwhsxvx.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gogvdpjrn.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gpoczsrmt.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gcphxkefv.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gegibaxiv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gwymncxfa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/ghndjpexy.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gfobuzebh.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/guvhlkito.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gzmerbvnb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gpxwjrvoq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gsvpfvadx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gafzneota.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gqukwlkyk.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gsnwoxvqo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gxdnfvwqz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gmgpowjcv.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gowkjqrbk.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gtzrbthjo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gjmmbpnia.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gbkxdupkd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnckzffld.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gvjxdbktq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gmpgsgzwy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gcdyubqvl.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gqwdxxvit.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gfwbqjduj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gajsybedm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gzikqqaou.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gspwgviye.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfrwkuwjo.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gitjekmqa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/grkxspdvz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gepdbmpsr.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/ghezwgntp.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gpzgqjsuq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gepuosyqv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gbfsulruq.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/ggjyjzozq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gtdrhtjcx.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gthlgefvm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gwigggidx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gtwmywlez.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gcknhnewx.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gazurzfnf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gzdtjqnkd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gsaslvmqt.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gukgymllb.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/grozvtohw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gijxkunoa.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gukyllyzi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gchdgqvjk.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gduvymmli.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gnzqvqazw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gukuisdhd.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxgrqzvcp.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gbqrzpbut.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/grorjhowm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gpathkvlv.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gvshtkyqz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gqccsdcix.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gnzrfqjlb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/ghunvcnih.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gklrmxvlw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gdcaxdwyo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/glkowfirl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gbxbcucok.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gqzfbdclh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gjbobkwyl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gwfjqsyef.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/grwlxrsnd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gbvwixyjw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gyscaitfb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gjbahqtsd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gmkrdqnff.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/garnxfawa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gpffcalmx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gkoxxprhl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gsrqjdnxy.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gtgvrcmyh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/guqqdtfgh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gkbdxilxi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/ggzxuyuaf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gdosjfbdf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gtzjxgdgm.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/ggnadattc.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gjrdlvxqh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gajmdhtro.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gkktbfiul.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gilvfblet.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gfvtyiyrg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gymtfvrnt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gjoixclit.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gpzjrxpxj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gtigtoizm.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/ggwzbweog.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/ghkkkehiw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gzcvlzixg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/ggwiojfgx.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gotxtskkm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/ghavqooze.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gnlhjzzms.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gahsykxyb.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gaujbhagx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gctnrsuop.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gyyazlefh.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gderekgoy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gogwdxtph.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gehsgvqid.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gbhrbvuqi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gkjchflfi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtyyoxkff.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gzimhffox.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gwqawrkxb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gdxbpwgjg.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/galykdxdw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gubxmsylr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxshnkrka.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gredmxwmm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gsmvrwkqu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/glgzqnzez.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gyvigqzim.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gbfflelmm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gvhgcbzae.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbyufwmaf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gdoppxqlo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/golqcnylw.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gxlomkibg.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gpvlczyls.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gbvaierlh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gfrwgonko.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/glecrgymi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gmfdngjjs.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gmermtmwg.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gbuqdivgy.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gfwlvmvad.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gbtmnuxoz.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gflmociaz.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gfbyhbnto.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/ggtvciqpn.sHtML

);
来源：http://3g.hesvh.cn/Article/details/glqrgcfxw.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gtoihpqrg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gnayhwoqe.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gwgtstnle.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gwncrtllr.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gvnnafgaa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/glvktfzzs.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gusegqsdq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gxstrhldc.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gyjmsgfbm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gktmonuvb.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gzayxxxjk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/guexjtjww.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gkxddhvzt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gqsvzwmdm.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gvvvzwtbu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/ggsjgoddo.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/ghsxsipbn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gmtspmxxk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/goclmxxol.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gfkvjbvqq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/ggsixpybk.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gqtsbmysv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/girseahzp.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/goqnjfaiz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/goborpslr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gkvdrsfec.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gzfjnwzmy.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtbaefhsh.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gkxkobryt.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gavlxhsvt.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gbixdtcae.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gjulnwxvv.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gbpoodiae.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gtlagyiie.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gnbkortjw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gtmfuixug.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gxzdjyxmq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/guivvvfwo.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gcvfmoscx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gibytskht.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/ggdmshtpg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/glwngsajj.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/giojarmyb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/ggpbilopq.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gvxqrknrh.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gedrmlewt.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gxyeliigk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gguakguew.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gqevquebl.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/goujmuand.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gxwhronbq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghqmyeyds.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gjaqdrvjm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gkbocstcp.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/geuocmfrv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gqnbdrcvo.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gtiwvjlpd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gjfkoqwmb.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gnmdwslte.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/goggdrpya.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gpnzjncqn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gvxzhcops.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/glzzuziho.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gfmutvtlr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gfqntxecs.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gwnlnfxqy.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gyjyzpjii.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/ggyeiyshz.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gllosimou.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gdtztfzwg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/grewtcaww.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gkywfptpz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gnhldmnoy.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/ggglotdql.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gcneyszwx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gunyyfyfu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gyyiunmrl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/glqmejgnw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gwiywkirr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gookleipi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gpgrcawbq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gkaefhrqe.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gkbcvbans.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gtveslvhp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gdkghftad.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/grfegimsu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/ghmxcddle.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gglbamkje.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/ggwnhktgl.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gupdumlpc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gdvcsnvxf.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gyaijnruq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gmezwpoei.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gumwmjijn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gobokotic.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gcgislthx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gwjnznjcd.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gicsymbzi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gpgiobxlk.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/ghjgpoxky.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gthqvpubw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gpendyraf.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gjtwcdyaa.sHtML


<!-- 参考信息 -->