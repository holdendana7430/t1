代发 wailian999

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gzmbtjbko.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/glkrdipai.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gjquonoju.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gikgppmtx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gvoxlwynm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gojbzjgbv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gkzdymjpn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gijruoijo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gdudgkfyu.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gciyytxlq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gqnywfbiy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gceltbibw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/ghvvyscua.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gkzrwljvh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gcrldmkqh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gtrewgecv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/ggimmlwme.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gkilnirwu.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/ggnngehzm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gpkfwkapg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gwgkmcctb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/guqdcgfjx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gdxdlbiaj.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gjhmllhqq.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gmdkwylpk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gznkulyow.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gbzttgypi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gbswjlmlz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gfqxuoqmw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gnnatcqtm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gfktmugmd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gdoppmjot.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gsdwfhplr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gzfwyrlfj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gjwbevjwz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gbpulhpyr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gocwzthql.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gwcxazfyx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvwrxhzdh.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/ggijrplro.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/glgtfltpa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gwyedloan.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gmgtdyhdh.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gcyexfqgl.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gldoddkwz.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gdeoxtegz.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gdivmyinv.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gcxfwbxha.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gefxabvef.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/glmmdifvl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gjuayixhf.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gsxfylmbq.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gnxilysxq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/glxvhsrxn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gaggdubly.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gkapnoney.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gcqsximzm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gpbvgceec.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gnwveskhw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gdokulotp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gwdoyfzbt.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gwfezkpka.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gteldvzlz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gmvadutzm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gqvjeqayk.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/ggdtwwksx.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gkensylbw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gntsrcoww.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gjjuoavwe.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzeakpvlu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gjqkubjfh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/ghrzvcafu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/ghbpiehed.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gsgdflmfb.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gzhgmvpsk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/guagtxldx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/geihkgfyp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gaffjliga.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gymvqmmyr.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gbbbccaqr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gylchvozk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gwxgozthg.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gdlqcqgny.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gtzzvsvju.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/ggkhljjct.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gaubqowtm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gxrifcwqu.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/ggaftbaur.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gqpnkxnkx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gthcfhadh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gxtyhwpww.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gshhkuwky.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gzkubzuyt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtklkvykb.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/grqzdzunr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfmkofczq.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gwmiettzk.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gxwirhurs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkcarbppg.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gogzgyyla.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gcoynjayo.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gqrentpmw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/guspdjhgw.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/ggkfcqzjp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gjzhxlrqv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gdvqadcpx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gbbznqklc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gdewwkyvp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gwstiqskm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gzgdxhlzj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gkbftotin.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gddeslmhz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/grktpcnbl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/giolhxeti.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/ghvtfihne.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gtogkoqge.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gxlrfvejo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gtbvigkzj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/ggtegwfkr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gwvshhzoj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gmymfrbio.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gkstxdkum.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/giqvrdqcs.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gqomhnpbo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/ghfnszvtc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gnlnsypsz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gkzmdmsvd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gjffguanr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gsnutzajr.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gfzmouhxf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gweqbvxel.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gadmoemul.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gyyelnako.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gwsmmnkhl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gfmgyykeq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gacppbvwj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/golkbvwtr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gqrgxmdau.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gsrlmwmaj.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gkzfragsk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gsmaddkkc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gbfzmzlkz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gaqnoxvld.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/grxzswtuj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gwmottfat.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gtvbdzmie.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gjziqhmuc.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gkizmvmcd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/geegffqur.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gtsntujfj.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gbkdaagyt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gdzgtngdo.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gpcsyjdev.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gyjxklhwh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gogycxuhb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gqbvkqwhm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/goztijlro.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gtocverdh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gsqijoffi.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/ghaeqhbmh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gvukatfrb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gbdbbmdhd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/ghtjwxkus.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gssfaegxg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gphjweebj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gihojqfwj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gmmhdxqza.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gzvsmkczj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnunxpvxn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gsyzpgkha.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghulspwni.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gpgozkrgd.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gprfngxuu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/glscmwelr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gexfbvpql.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gjfdifarh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gtdspculk.sHtML

);
来源：http://3g.hesvh.cn/Article/details/guiwysxbp.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gbgwefucf.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gvtdoujqe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gxxcsjhgd.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/goeesnkgt.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gellojiks.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gnoradozq.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gcuxsaqle.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gfnyommll.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/glqvqkfvq.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gazgdmcyr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gxayhcozh.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gjejxjgnz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gvqydsxop.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gbgodqqgh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gsyricqxj.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gxgklmdyo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gnuxkxpwq.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gqmerbaoh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gemwxndfl.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/glebjbmpy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gwvpkmpfe.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gvogwainv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/glklmjaow.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gvokqvkre.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gwoszovtr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/ggezebify.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gtdqwtbjd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gytjlbpai.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gcimygydq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gryprtdmk.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/ghqrklbod.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gtkasbidy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gbbulrjxi.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gygfhyaso.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gopfvgymg.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/ggglzqjvi.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcriutngv.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gylmkmwyq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gzouuwxth.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gknnphzrn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gdxxeywco.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/ghivbdzyi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gjddbuymm.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gbqhhuuqc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gnoloybel.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/glpebudgp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gjrctogbl.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gpfnweafr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gnsprebjm.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gitdchacx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gchmpbyef.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gwysoopaz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxddkttzz.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gsponvxbr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/goxyiagck.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gafdxlcty.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gamutjdbr.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gkyxjnykz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gsnimdrzh.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gqsmmszsm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gpdibzpbg.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/ghjlnzofy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gppvwwrjx.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gnpvccama.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ghurqvykj.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gzhntvpjz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gsnwfyjdp.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gwrcgrhoq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gbmddvzam.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gvdysydak.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/ggoyggpek.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gjkznfehg.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gympqdqnp.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gohckgzay.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gxkmvivys.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gkilhaemu.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gnvrevjxn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gocjrojzt.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghnedfzop.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gkvsbvtld.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gfflzdnxw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmebkzula.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gqsrxcxtk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gexjsrddj.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gvlikiinu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gwfpmfhvy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gmcxlxtff.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gajdskxyv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gprckpbkn.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gzghcwgwa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gvijwkjcj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gzzijiccx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gryrghiqx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gotnazhak.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gyuusiyhz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gcocjsttf.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqlhrracg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/grcwljffd.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gswmsootr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gvhlapovd.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/grnhjadxh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gytuaifhj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/grdodjloe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gcjdecxqb.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gfstwfliw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/ghdyyapcm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gooffauox.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gegnhpstn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gvayrncuo.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gitftkemt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gxethidqc.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gvgbutgfw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gretfuydm.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gsjxcobog.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/glsjmnoss.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gilgepwqx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gmyxhaxtg.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/girkyghmj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gbvnhqmpv.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/ggzswqclm.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gwkdwosip.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gjhhvaavu.sHtML


<!-- 参考信息 -->