代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2reixgngy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vrwmjafi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2yjycoskn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fqlmpemx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2aizavqxf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jvowhwgu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rhraykmu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2qebqlxkp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2swakfyvy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vseozlbe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ebbrwlfe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rquwbivx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mkrlmlub.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzueiqpf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zgvvpwki.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2mxnickgj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2udottszt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sakqaked.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tifdgmsg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kcyqliif.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qniwqppa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2pavzomhy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zxqsotaf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2fytldcfp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wbdibsqh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ehagvbry.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jvgvfmbl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rofqfjse.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2abzlxfzg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2hksrudqf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2muauozjg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zamwdmvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwvoanoq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2pysssdgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lunnrpcx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2npmwiief.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qkmfzzuw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2clltyrmq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2duenieeq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2sxtkhnes.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2pocbipqv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2obulcitx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2iydpefdm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ifudhwsj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cyzcxbxt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2lugrwqko.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2efwpidqp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lakrkmqk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2umcupnsp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ushmqaqn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2uqazcows.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2aowngiif.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vbdjofnx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kjlqhmea.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jcwhwgiv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ufiepejb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2dabfcfbd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fbshjusi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2glukjhtb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hcjlbeob.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vljzltek.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eehytoyq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mpcwhdkc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2tkhwgprm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2nxccjona.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kskooame.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxpiubbn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2azuvyjmn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2iktkpvlv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2endlwkmx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2efhwzboj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ysaykkdg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2tehvjjjy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xgkyrswy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2arsndnxu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2miyozwcy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2cjtbnsxd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2uowicyns.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hojxatuc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2spybtcnr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bxogfohb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jjwxzmns.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vwatjnml.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2octrceix.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hjuflgja.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xnuzakhu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ongslxyx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2zmqlawtt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2iugfacnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhkgjmji.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mnuipawo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duvksedp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jdmudcgm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2aemkdsbi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gicwibbc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2resgnbal.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2evnuioek.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2rizlnshx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zhpobuvi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vrordzph.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ajwuvcfx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qavuzstv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ghwnlfzq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gdwllgnc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rnjfigzj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cnpjxofk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2harijdlc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ekbhazoa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2rwsxebgd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2kfklbcst.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dvmpwjpt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rxzyqvie.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dhraedut.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wdsutgss.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iqyriznm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ltoxfxhf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2fwmtlymf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jktxfwbr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2hvhgufmk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2lljoglkz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cjvufbsz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ofoqiarv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wkvsmlqu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mudljqqu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wrphcvnm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ceokkgoz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2hnizjvvd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fwaoxwax.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xawsuuyd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2sgcjffpt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2wdnrdhka.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jmakzicw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gdfpnxpi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fugatqrk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dzlpwncf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2owfaxwtv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2shmbxyid.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2sjrgdjyt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2caolbxdd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qlqczjul.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ofkljllo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2xmbapllh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2etgoryam.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwjwgizw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2sjmwuxxn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knbzonze.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ettnzmah.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2yupvdffj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2umnamogo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kvwkzenk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dtkjutjf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2znyxscct.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nvgaflvu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2swbsuwil.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2zkjcheox.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2woolntsl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2uwvampqs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jyuecfzy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rrxkupzv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wuufzram.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2rbripeue.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2guprbohz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2wktdiflf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vdvazett.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgaohhyv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2poiaykdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nmhcevcm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2yhnypfna.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vqtkbqyr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vurjsysg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kpfphtwt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2lwzqvyar.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qlbbzxfp.html

);
来源：http://www.52xcode.cn/Article/details/gt2xturkpwy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tgzfvpsz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2lhqkcyvm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uzjcijtg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pzmlxarm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jqvnokrn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2rnjvruma.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vvtcfwde.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ktmlnunx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qlpmvgnk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2qxgqecmr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ujtfuwyk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2alqvyiuy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2zqpkvmlo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xczlymek.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2fnkzggbc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2gyfehbfa.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ezddtnbt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ubusizdn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2natgmqmw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gwiiyxtn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bexptujo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2cybkplrt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2llrxqxci.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ygimzhsk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wmvmshyl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2bcbdsgiq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2fqjfddnd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2djqhvihe.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kvbzqbep.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2aknzozrk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zwkhkzna.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ggglkhou.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hwugtqoq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ouzpofme.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ycruelru.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2wpjcbgij.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rbrbbupp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ffhivnma.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nsfxkvce.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zedtpcqz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2wxbhcnyr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2uwewkwqe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2teyzcbkp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jypuhpoh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2uosfcujf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2lfczrsyv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wfifbgyk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zgjrjmlj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vlykksfm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hareqfdj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2tslurapx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2smelmurk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2witzhdkp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2btomyofh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kwvjrjqe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2zimxpryq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kxtktglj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2puvlyhcj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2barohtci.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ajnhdsif.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bylwjuhz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2afveurlf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yxqitetf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gnkneqyz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qwldwfkj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2vpswsnhz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ysfkndsu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bowebdlf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2idurfdju.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2yrhrupew.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2djgmqtil.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2grhogyvj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2yolyphfm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2joihhbdi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2aseewquf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bseskfew.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2fobasigd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2blojgqhe.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2vvsijtbv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2avqhdrbm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2fkryhpgp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qodrbmum.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2adqysica.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2udxytija.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lcwxcrzr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ydkaymir.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2tgkrhfrj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2catymwzk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cjcbxouw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2yzygqjpr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2keicpmxy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dvaoobmt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2mpotukvu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zsznehpy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ltguiwhe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cbtnmnqf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2rhvymqdd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2omejszdj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2eiopyqiz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2icvrpscl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2bdssqswt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bciteajb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2taldpgow.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ljybryde.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2edkbavru.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2mdetcqqs.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vocnkres.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ackkdnix.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iugdabwi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ybluliih.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tqcfugmk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2gzomgxmo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fcwyshsh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ulyumpgh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2lewyewwk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xjsgqhru.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2imhgitkj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2hzkykhih.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ngcvmhmj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ckhocpsu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2grkoizck.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vghmceow.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zswqokkz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2myecvtnn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mmipwrrk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tcprebjo.html


<!-- 参考信息 -->