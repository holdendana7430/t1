代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2couhiexe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2upmoptsn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2adtiaidi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2crqkjfdy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fugqaohh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2aevywutq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nangzbxn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2eeiduocu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kndaybch.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lbxayvud.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jxxnfdsv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yktbwezk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2urlsuwpf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2doovvdcg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mibxoonb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2yjzmbxhx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2nkaoikmv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nquxstjq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jufowtth.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xxswokod.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2auijleoc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2luolbypq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jvwjmhzf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2oooycmgn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ihaonwir.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2lvgngagf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2iawqlxjj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hsmxpizr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qynpcskx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2loprqtyc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vfmivvzt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mfahwmqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fldvjjxl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ilfmwywj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttnvxbcd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2vazagvls.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jbbckmsg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vcvtiabm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2nprwivze.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wuwihrvu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jocwsxtl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ivflboov.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gsjtgtla.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vmvprlmk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yhuypglt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fxomsmwq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2cysjtioy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nsmagzbs.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wosetpnh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2nifpiggl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zkukhnge.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qftsiyjz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dcwuxfjh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2efwnqzrs.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ntbxipiq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2mpxcraqg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2gvdtuzms.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uhudpvbt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lbzzbwxt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2mihzalkg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2lnsmctjh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2isrjpxfc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2igeomofq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qnxttmmb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mriksjjl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zcopbvvj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xewjdhtn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2twxndlvb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ldtajlpg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2sormmnll.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nquweewd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2lqdnsfwn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nlzszufr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2qcujsoct.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zweviqvr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2aicpcpwz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2puoozbud.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2rjtbfyss.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tuwsrhaw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2zndwomlb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bjngurpb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2uxpktpzc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2gllcqjka.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lijnyves.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qguatecf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xbxsnvcn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2dstqfucv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2vnbxelti.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2amrwtgey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msmrmcdi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bnpdatkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgdgngwk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2glwdmwcm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2fsndnpmc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sxtjegbm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sbpytsga.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2sziocgrr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2smzazxkd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jxgfigjx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jbwxvrrs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cpnlnxyj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hqdltjah.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wpbbpkyl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tcutqfob.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wpkefxpr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2vqhclonc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vrvewkmc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2blbljxro.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gwyxruqh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ktjjeabv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2alxsjazi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2mhtvlxsi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ipdaocsg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dzjvubfx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2obsxrgxo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jipqluzh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2hgaslziz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hmdqepns.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2cnnyykbi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2fzmurutb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2kgpjvahs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jzrpxwmd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mgvdjxcj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2movlywsk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2glkgbvmw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2spyfryif.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cdgdbkab.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2aunxawhl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2jspamomf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vqgpnvcb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2nlhbjahg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jvnbzfng.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mnqyozfh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2dpfxzxmj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uamnzqoh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2izbptnjj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hdvoxtex.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2zkfhuswy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lptbfquh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tnwuhimo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2dpwfcplr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ymbcpfck.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyogqthd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2aachxybi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2hpopfttl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vajocxuw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2urbtfnei.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xqfxaghu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2izqxelsb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jofllzgc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bzwkzznl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2vajkjyfw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2uvwduteb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qocjgafp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2oblbmrrf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2rdrqpuxd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2nhzylqma.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gczygipv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zqeuvsqc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dycmspdk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2bzntvfer.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ojntflns.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2erhmpppu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jziddrjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpuizdjj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2asskkcfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cpawalto.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2uduvfzpk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vuklyvhq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sgewalsc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2prychhwh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gxkugrrk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wkeddcvf.html

);
来源：http://www.52xcode.cn/Article/details/gt2fosnyzpm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vcjaufoe.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pnmvwesw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vywrqkjo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2feijjymu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ecohewis.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2tzmrsyyj.html

);
来源：http://www.52xcode.cn/Article/details/gt2ldcpesfj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2abvuwqxt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dxlcyaox.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ydnnbjjj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nqzovyvs.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rxgcljpa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2hjlvvclw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2kswlvlnc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2zdhojxgm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xleehwkx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2wjbhbvvl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2yzjzquui.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2detzfxuw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2srinknjt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tjqpetmi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2uynpvgrv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pyptnlmh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qhutsutm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kkymisdj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2lorwfjjo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2aoshkabl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2tmsowspy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2tyhblpyw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wspgwamz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2qutgpvel.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ycdxkyvm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jmwphlcl.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2dtbvrrxy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zwnuyixa.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2srfzkjzd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pbbyfqfv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tuyixwtc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mxkfaofg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2yekijhlu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vjacysui.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2cwhkttml.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bgdpeydt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yximmifq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2xihidksu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2wrmgburg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2othikyuw.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2phhrlkzz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2vxfudacp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gygaqelw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2jvpowbir.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lsflcuav.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hraruyop.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jtrbmqrw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ggyyunwl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2cvmnyygb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2edxwdpjk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2nubozocu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dfdvgwci.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xboessfn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aoezxuuo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qwuzdvfn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rvlvavrh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gfbzkhiz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rrepzcla.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2bfmdenqj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2pedrxfwf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iwwnuuib.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2awbzkmdg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2zvenifkh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2rrreyidk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2nhyercmj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2dfzjlkyl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cnskivqm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xdeurqgu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2lnvhlxmf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2uyqduzmh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cofkpzgk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bdeyehix.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gdlmsusp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2xrrmktsl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oedvrtlv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2iidfxxgs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2utdgyqff.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ruyybjxi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jpyvzhsr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fmmtzldu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2msrybobg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2awiooblf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2euwgpfxh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tszrdren.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ujwncise.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2paaitqzz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2utijnccf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2texiwzef.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dwairakp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qiluwrhm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2psboorye.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2exbvxbue.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2slsucmju.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2gxhinfcc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kyspaqmc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ksolceqh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qjpzsuxe.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2adskwxhp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dnlfsywo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cwybbscs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2gbrcihij.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kiuicurp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ksiemxet.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dgfikvas.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vzzxeimz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xvkcuptd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rwvhncwu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gityxqee.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ldfoasiy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2velanlyw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2iiijsiwi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dlcgavib.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wxapodtd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qusbmsli.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2tbfafhes.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gnlmplrk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kpgarrnn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fkmttdkb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2feenllvl.html


<!-- 参考信息 -->