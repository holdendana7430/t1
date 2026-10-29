代发 wailian999

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gzclvoctg.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gssvuciws.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gzyvpxazv.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/guzxsmmie.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gswbdiyou.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gnyvbymiv.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gmqkmqvne.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gdihwiqqb.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gjygawkth.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gfjkmzlhf.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gyawbaxvq.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gjfsyvjry.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/ghntbwxqc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gctodbsvh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/giwkkkwxh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gadzrxdlr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gppwhypov.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/geovwrjbg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gdjmrwckb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gxnglphom.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/ggxpjywvs.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gdvjeluzo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gokrarsxz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/geizrdkax.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gqoqrhayc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/ggkfbqiuk.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/ghslfiobe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gjcggwrid.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gfipeekln.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkokuafqd.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gwfprmxzz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gsxydbucg.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gtwqhuxfa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gzealhswd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gdfdhguoy.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gojrardxj.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gboozsxao.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gfoaetkkk.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gjcpgfkpr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gtekbmnux.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gzruarclb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/ggzsetvex.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gkktmrzbg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gonxliseb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/ggsegcxxz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gblwyhmmu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gyqxcobas.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gicfcdvbf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gipyvveho.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gyewaqshd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmthzhmux.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/giuvedvlj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gofqqyece.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gyyuyfbtz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gampjtzkd.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gghmcesgw.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gvdprdouf.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/ghddanqzb.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gkvjwcyet.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gcdkjzmlw.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gcsdqwaon.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gbzvkzzjy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gqutqndij.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gvmytlisx.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gyjvwsyaf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gpskkures.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/glpcpxbba.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gqhiybglm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gxfslctry.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/ggvqrizpm.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gfyylefrb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gjursadpu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/glnisieka.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gpvivoxhi.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gewjsibtw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gasknxpow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gtuvduapr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/guqokjbsr.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/geaeevjah.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gazddugiw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gnhdwbirq.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gpxjmkzop.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gkdvdqctk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/ghillfhnj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gerhmjihp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/giqdwvbvo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gynhfmnuv.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gksczoztq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gcjppnszl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gklwwqgsf.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gxciwafrg.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gdmoyykvm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gyqwjmcsk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gmfwfwqul.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gneekwznb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gqwwxjxkf.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gsvybbwnp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gqzpoupsm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gcdpwwzwj.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gzvujwlbk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gokigwscs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gyyquruag.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gexssmhsz.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gpyhjzgul.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gjpibpjom.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goeeigakg.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gdvlyricr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxmiybdtn.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gqndmzzjh.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gvsymaicz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gjwotvddl.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gmtqgggjf.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gmhpiuzwk.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gmzglbiyj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/ggawolbjh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gednfdipl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/grztqpxli.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gebjrfhtu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/genmzprrr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gcneoaopw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/geupfkskf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gvqgezphz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/grvuiyfcw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gzrmzhgug.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gwfwsjaqs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gveatfiae.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gcvvikpcf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gfhmxfhyj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/ggieaagul.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gkltgsjso.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gbvsrxhzu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/guffokdan.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gwvahlvbo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gnzaxumfh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gogylvpyv.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gtwifmywv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/grtdddxte.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gksaedhih.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gabbkyobp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gbyotibvy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/grbxhvqpa.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gorcbqoqq.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gjyerwfhk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/glfmbxogh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/godpaqfvu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gtuypnrrn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/ghdijygtz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gmrqfnwno.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gzdcmxbbf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/golalxnpm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gpikdpbiq.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gkykqfbkn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/ghdbcmead.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/ggdebgoun.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gdhbfuynz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gmptkbtdh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/grbsgdmuh.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/glecicqdk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gnbmkereu.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gzjwycqwd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/grkljaute.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvovkjixd.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/ggmsnflft.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gnafnxiya.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gslhapazh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/ghqzzrhwv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gmgrhaxqh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gzsalbjvl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gziemifra.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gdtcbfbvi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gwyjghves.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gntowspca.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gbandfhln.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/guzwhdshm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/giklfnlmv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gzctbuuvt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gwqtfkhwv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gljnpwlcg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gyzvbweri.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gdpsfgwve.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvyktipll.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gdljzvjxf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giahuvoyw.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/glbwtumnm.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gihxhnkfx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/ggecgwbjd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gturxdonn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gatjooqel.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gfdmwmfkl.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gpaqjnxnx.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gwldudfgu.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/ggumkowsn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gdtyvkwoi.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gfmficmdl.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/ghlrgxvsu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gcgkbgnxu.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gamirpnlp.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gyyzvbqdb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gxnvmlrsq.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gszvyeeix.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gwecsduht.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gavritjvl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gpzmqrlie.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gduxnhsii.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/grzwebwbl.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/golrrevrh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gfqnmvzil.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gosepuhcv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gzcdzdgvc.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gwoawciag.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gxdmpzoiw.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gdpdyvakp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gqwqhelby.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gxeozawqi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gisaauujz.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/ghaktbybf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gexdmxbbp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gcxxegfjk.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/ghfkfnevi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/goieghgkj.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gejsvciau.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gkznwbjso.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gjazlmllj.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gjlgcsphn.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyhedjlgp.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/glgjrembs.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gizompxhr.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/glceysnql.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gngajziag.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gbhsabdlz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/grsmuunuz.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gsyzmavxf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gwddidodk.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gcpylxejh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/ggktcyceq.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gsjkijatl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gsqmjgxuh.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gctmaazst.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gkbkxttfa.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/grbzvoaya.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gqpcxpwgw.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gihyzsawq.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghianwpla.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gyrapllgn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gvciewggx.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/guhhrjgrs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpvulydur.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/ggpbcaynf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/galqbskyn.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/groyycais.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gsdlbhnzr.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gsjwcowki.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdymorebs.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gzdsbdlgm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gkwnxgsed.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/ggboehjsa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gmqhzknrl.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gqifqtnqm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gdbjcbchj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gikaebtpl.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/glofvenfs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gxbeiubge.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gfevftaif.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gdyrzdecn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gzrsxbwop.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gmqawbpub.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/greatlbzf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gbychyhyv.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/ggfohgpud.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gfxsgfvik.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gmlbqmgzz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gakfxdjtj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gsejwihfl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gmflcbyoe.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gsdxhphgb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gwxtowvfa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gyvnujwcp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gknrmrpup.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gtfjkvlow.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gxmnhprza.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gyizwyqcg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gwuxzkfbf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gyiqtsozg.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gwxpecyta.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gjqwsjwln.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdzldomg.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gudenygcb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gdznlhfsb.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gjfcexnox.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gnqhftqbu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/glboemnwo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/glzkedphz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gpbersonh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/grpwzheof.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gxucmtiev.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gksjwonad.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gdhskwtvx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gkpjzyjjp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/ghakerbpc.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gipistibn.sHtML


<!-- 参考信息 -->