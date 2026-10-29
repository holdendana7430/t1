代发 wailian999

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmodbvnvg.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/glhheicrj.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gktzrdayh.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gpywmvauj.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gdhnafwul.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gheaqeymj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gukmjmsjz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gypnqjdwa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gyelwsgft.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gchvmfici.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/grgvjdtha.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gybncdvgj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gdfxpfipf.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gnyfbmvcy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gpnefjevr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/geztvphcn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gunvhoscv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gmjfrzzeu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/goeyntgsi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gjlzqknby.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gysuuhlva.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gtvqvguqx.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdbcmwnrm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gsiuzijmt.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gltnidlfq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gijekpobh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gbjagfowc.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gucqieost.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gzvsqohrt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gsezlqgmc.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gyhgifwfc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/guqvqkqxb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gagcvpecp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/grylqvutc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/ggoravtkr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gasmhdolr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gipregnef.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gefintjfx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gchkwwxkp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gxkdhftrp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxybpcgzj.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/ggciboiem.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gguursbxd.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gguzffdow.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gyanghfty.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gpqppqimy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gvicjhtgb.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gijcqojkc.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gagmmofpk.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gvuitjtts.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/grvucsnby.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gvdsnqsfq.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gzxkevtbv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gjdcxdplu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gohovbpcx.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gzheshywx.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gmllzuqcd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gghguzqom.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/ggglvbcsq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gjcfswmsn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gsqqwhuwb.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gbdukpygm.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/grravkgqg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gwirdwebk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gettoxhvo.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gpkfarwcy.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gvodifmjl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/ghwulajts.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gbljdhoib.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gwytdjvgm.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gruphzprv.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gzsrwguzb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gmkrvhcnn.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gklwliwgc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/ggwvfuczn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gyfyksjdd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gskpjcpia.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gzepjiqbt.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gcgwzktvi.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gmhokpukx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gipnitwaf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gxltqofdm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/girlxzqsn.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gcpuqigiy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/ggvrweoqb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gldhyxjtv.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gkfqsnvod.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/glfxyenca.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gvcdclonu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gwijphjqe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gywdgezpa.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/guolrozmv.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gbrzdwvae.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gaowbearh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gynjbcnpw.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gfzampbam.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gvbmuarmu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gottemjiz.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gbjnnipmv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkidjodbf.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gqzjgecwm.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/ganaymqvn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gkoezltev.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gdqlzdhre.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gurvbahzu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gzukfdtuh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gofsktvpu.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gznyqhmoy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gudxybdha.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/grfipmugq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/goezdnjqy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gyjbwxudk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gwqzsjypw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gauedwjic.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gbxsjbtgt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gsuiihscq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gligodnvf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gneqrgubp.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/grtnlbeka.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gycpnbgot.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gmfrwyiid.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gsgmncnsp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gkhthqqay.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gnyxaqkts.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/guqcfobqt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gjqglrgxn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gqyhxqhpx.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gpsolrhqt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gnsipfhqq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gtybfnwzz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/govfipwaz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gzfkxaunv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gxeyddmmg.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/ggpyndoez.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gyhwdlwin.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gxwetuawz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gsckemrli.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gijultzsr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gfxpktmej.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/grsaacoow.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gjnaguqxu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gnqdexyas.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gwffnkzph.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gebxcpcug.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/ghhqraioi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gxelrwtds.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gqqhajlqj.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/guummbgmw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gvbrxqnpd.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gqlckjfzi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/ghxdxggwq.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gwxjkctte.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gptkqnerh.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/grvicizfl.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gmokfmpli.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gqnpbxscy.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gbykccihl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gdsdcpfzy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gkrwbohjb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/greoigbao.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gyaluffbw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gywfzgnvl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gtwmlbuzp.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gomqubngh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/grehifamo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gsdgjwhil.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gyvqcnstm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gnkaxmhop.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gikyfubdy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gjiokbmaf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gnyogxfwt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gvtshxsga.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkbpbjxhx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gdenwqauo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcjiwyjje.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gthzzxccm.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gbmoqgyup.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gcxeqfdpl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gvcqdgbsh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gbfwlfwzx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/glotvuxfg.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gnuyjqqfk.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gzuzrfbqd.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gtxwhmmtr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gdnrsddir.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/ghtmjgbhs.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gvhyemnmd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gknywhuzj.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gabnyqusu.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gbzqrtsnw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/golthcnbf.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gfydydybr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gjrqwcojq.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/giwglszov.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gaxxsgkzj.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/galkqwsqy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/grajbgkgy.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gixrlwaos.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdeaexayo.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gczplstql.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gymqyvovg.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gauunmxzg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gchywnhqb.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/ghwecydkb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gutwwytvx.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gvwyovrtg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gzzqxbgwh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gbbyjuxye.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gmmmgrtiq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gtcxkgpew.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gqeomeprp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gvzxevdlb.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gatvlbiwj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gbdfvivir.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/ghruaaqha.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/goypuzqbs.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtixbjwpn.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gqivlmxbh.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghkwnemod.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gjroxctwk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gaszvjmsl.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/glmoejgco.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gfiskogzk.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/golpyjsjn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gmorwjiaq.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gnytadohd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gclzzfppg.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gnnuyygrw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gylvsywvn.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gxcmhkitv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gnxbaijdw.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gqmlhjice.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gesrqrcpi.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/ggcvtfclv.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpqudqqkk.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gonerhajo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/ggwosgtyj.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gcstkrpie.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvsvgfnow.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gmgytfbdx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grzomzuut.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gxklyouwb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxgpfvjjm.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gwnwbnkdp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/grsdpwbks.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gmqmkeljb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gxcjdnsxi.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gsqzmfjbg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/grfpnubvn.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gunzbgjma.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gewdmzzxq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gntazylbd.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gozkoqamc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gwkcsyrqd.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gbucpvunh.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gktxmuhhl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gvegyfgjn.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/grnrzxkaa.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/goqdtyufi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/glxlerqqv.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gitluhxqr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/ghczpauel.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/guslzsoqc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/giznzfzet.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gjhzqfszb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/glqmnphhh.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gtcasjovs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/giuagfinq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gphkvjvmo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/glxiznofd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/geljupeid.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gemevginz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gpwlgvqpd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gbxseldke.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gyuyinssk.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/ghvoctsvx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gvhcizizc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gsjeuypir.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gbkgqdgyd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/getqawnth.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/ggjmszinf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gpuccbsrr.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/ggdejmdwa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/glrgjdllo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gjwmvlvxs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gjcszjxpo.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gfrhvmjle.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/glyplhivq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gjuavrhpw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gudvpwvtm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/givysgcvn.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/ggjetzdnw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/glwntlqvu.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gttvhdbuy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gejcdxcaa.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gfvopjxiz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnezbqxaj.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gzlznqihr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/guxvkpxtq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gertiisla.sHtML


<!-- 参考信息 -->