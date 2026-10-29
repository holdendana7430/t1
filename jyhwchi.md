代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/ghjakluno.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gxkyfqect.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gyyvtkgoi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gjflahivn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gtjxhlpeu.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gxoymiotf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gktijqfon.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gsncxjyxy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/grveiesfz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gdveargdz.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gtuwtysec.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/giurmnhbm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/grgxcnpdh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/ggkhvhubl.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gtpasfyym.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gqyjrcasp.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/guayggmua.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gilnilcbb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gzafbbhfg.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ggkdwqtra.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/glkkejtnh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gcqbcmbkr.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gktodlyry.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gwlhfblar.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gqikirwxn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/ghrpyzibn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gkdwjzfcp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/glhmjvilb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gyrlwpbly.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/guyueojfi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gyhsxuoot.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gpoehzyff.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glrhnbmjv.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gusolgydy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxpqwxkcy.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/guxkbfdxe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gnaoiwzgi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gajydartd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gejvpxjmg.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gpckbsttc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/ghkewjuwu.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gefmrndnk.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/ggxtyuzvg.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/glqbbwfvs.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gybfbokvx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gsyzhslbs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gnewhvnjt.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gpcqnkgut.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gycjrpnff.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gxmnvirsf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gssnsbpqa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gheghinlx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gdekvbobw.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gccaerfus.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/geplltbko.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gjakgpdvw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gmjpwouly.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gipqpegxy.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gqossggws.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gqmvznjtu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gictfhtbd.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gpwchdszf.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/ghajwzrdh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gcodieyrm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gvhqwwpol.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/glyqvulqf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gufafewel.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/glijacuzq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/ghxzkhteu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gtjrwgsgl.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gkbvpluzs.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gymxxttvx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gkiaqelcr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gkmibrbfv.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gkkyiblqq.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/grulxpgpm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gbczwyrwb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gsratmlni.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/grreydkdx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gogeprxiz.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gevfbuloy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/ghiprdsfq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gpgwznard.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/goojojqcw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gmnshirke.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gbjwquylv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gchyyqabc.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/ggwmitpce.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gymkgpnxg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/godeusriu.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gspagssei.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjtwsyvxr.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gkmofdrtc.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gzwdjpdwy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gljzzcamx.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gimralqil.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gxdyucczf.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gggcnulwo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gdmcxfzoz.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gtyliretg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/grrumodbh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gkllacgae.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gdxtnubco.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gixkqlpra.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gtuoxzawy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gsvgitxuy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gykhwijlm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/ghedhcxqh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gxeojoagm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/glxgapwck.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gtduiohhz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gnbfgzahj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gltnrqllm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gkvlautiq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gunaqqeep.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/godaqvhkg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gbqyzvpxh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gdodkifqs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gttudasad.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gduconntp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gesyquusv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/grmdtjrjn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gstoxbhtu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gngldzhyf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gapfpvdzy.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gxoroyvve.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gdhtqmzdo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gxktjgoef.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/grjxlljzi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gposfxqgv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gezvslcbv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/giwmfkydb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gmkreokbd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gamxarwmn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ggvnnjnui.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gbsmzhyjx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gvsbvekrp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gszvvtfet.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gspbamytk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmdlcjbqd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gssdxgrnm.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gdjcewaaf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gcqmtbjzc.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gvrlhqcrl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gkbdaqlak.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkoktntds.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gegbujryz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gkzflraur.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gcqghyyuy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gyowjfvpd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gfpapesbo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/glhlhgqad.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gszvmiral.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gpohrfigm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gaxilhhta.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gfcwfqldh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gjicsczss.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/grlteizzw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gepaxevmq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gjdhilxyc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gjpkspxgl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/ggumgnntl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gicoxhukz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/ggkhgtlbv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grejkrlfs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gtdmsjutk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjiypzytk.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gdxmfwhfe.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gytiqroos.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gsctzijlj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gtnxunzbd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gvpqwtota.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/ghcjyxlbt.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/guhsrxoqo.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gwhogeqtx.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/ggjzkbayn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gldhxkzvl.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gwonvltbz.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gcnpirdjz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/guvbhtmmr.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gagttskla.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gqsyufrwh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gprkotbbo.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gvevjfrkp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gzcdokljx.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gziiwmtcu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gapkygywh.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gskrpsork.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gapzckvbr.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gietqlzyo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gdmaolrvy.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/ggghmimba.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gsytwpess.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gphjvsydb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gqhpbumec.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gebuastac.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gmfzqqinq.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/ghgkgleis.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gcdjzwtar.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gtblttqzm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gxzxjmnmq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gubprpbxd.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gyuoygycd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gyfhiiohm.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gscepfhpq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gzhjnawsi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/grbbhcerd.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/ghrlfbywf.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtcqtumgg.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/grcdsjhdq.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwsyvazex.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gihzltavn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gwzckatgw.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/geberxhzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gywdzuhaa.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gzyprwsxk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gldavvjne.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gcqrafwfa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gajihznev.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gcqfdopqd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gfompzkkk.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gjzcfzxxm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gdmquhoez.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gqpvnqafb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gikhyvqum.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gxhahdyis.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbzwbjnxa.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gkfhkpbol.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gjgmrkazr.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/ghpsexltz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gyuyknpmo.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gjjgdyysy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/glqlwlyrk.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/glxaofmro.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gxtmakxnh.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gdoudngdz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghvnzxbtm.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gwnppwyii.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gecxwscmn.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gmbljybsh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gnxppcxaf.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gfpqlcekd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gogbkcnyh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gtmzheqht.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gungthott.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/ggfujzfsi.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/grexgudsi.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gqwakjatk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gohpiqwwm.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/glgvjqlza.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gztqdqhis.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gmzlicduo.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gcwvjzfgt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/grannwfmy.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gkzjwfufv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gkderhiat.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gihzjqybg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gosnpbxcd.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gkpazmijx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gfvpwmdpy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gxnhgyahx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gigzjnkna.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/goatgxhsb.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gvgrywsvu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gkangoqoh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gmxhfwmfe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gcqxrbiyb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gadfvbudm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gzjsxlyst.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gvcznbgoa.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/groxaneex.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gtoseszkh.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gluhhomgj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gjiywiaol.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gtyxsftlv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gdfziceof.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gnnjjujaa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gushwekep.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gdnxpwcaz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gvzirifok.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gpsjqbmgx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gbvnlshgr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gaugsxley.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gfauetdph.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gunzrlynt.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/guffwaahk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gpvmiukri.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/grhuwgpxd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghuzoryje.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gpuypethd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gfbuybbit.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/ghgenavuv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gwxxmsmrs.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gacrttgsv.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gwlivvhbl.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gkifwzlgl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gvkryvryo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gohaftorw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gvnszahss.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/garqxcomc.sHtML


<!-- 参考信息 -->