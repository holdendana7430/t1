代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dmryxcvo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ldyfbrsb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wryrrrjq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uodxkpte.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3eopxtaql.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rcpqktey.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3abepptbk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3qlrzpdau.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3fhnhkaoq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qtwjawjf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3invyeedg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3eosdptrv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3tudhgsfh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kbeavlly.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3elggplyv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3oqkdehyf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kgkhgttm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sbjpqoty.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dwcqfymi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vlkuwqyz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3awnfrwkk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lwlnsjnb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qhhpnzmc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3embcihkc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3tjevaful.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3lccbaxum.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hedfyjvc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3oqqxgfch.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vvmpisnh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3yhoxtjll.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3okpzsyic.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zcxtpejc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myxutlia.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bnaqefvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omeykskb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3urwfgcpk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cvlmufic.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3iptxflfs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3hsdszhvq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lhtjuwly.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ovezllgx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bxuddqew.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3afjcvepc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ogwhhzlj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iwbjewqb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3mtrkcssj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3aqxcnptg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ltlvpdbx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hlftwtsc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3blidlhfp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3sboiudtm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3bepmfiqb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jwtxdoyf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ejswycgh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vkcfwjif.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ybmzhrsu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3egdsvtwt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aqpxjpcn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3okskzrxr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rqutnoxx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ybcaoxul.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jazwnvoy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3kkmckewn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ificfnxe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jlqtrwry.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fiadtwiz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oywzhhtc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3dsdnygcj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3cxmvhaqo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3exkreptu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3paoftgkq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3qixbadgx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vjfqizwi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jlgzllrd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zadvttqq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vbnbtqiy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3hckaelix.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wbmstxxf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lsdbfzlg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3szslwrpe.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3eswrgcoa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wwgcoozx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3uazljidp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ryykpgsd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3giepzfpu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3idiqofws.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mxjaopep.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3nldycumc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3jwwqljia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aisqpzla.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3odhbkkus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmdimeqi.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zpmnwymy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ojecqper.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3vqlykodk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fvqojyhv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rkxbrwwl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3albfwqmy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3miuduohv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3uszrmjko.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3aqjmsinv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nmewxije.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ohxhtoic.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qjhyeodb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3nidaydxo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3gxmlrcun.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nofraqis.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3pcmahdvc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3swlibrdp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3vqwsmjph.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3yvisobqh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3djoohhxw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3fdtgubyv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ghdjawwm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dmmwvcbq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3xqqvbbkj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ggqukmdy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3pmwekjsw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3iwhivuup.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wfvpqdun.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vghqlgko.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3plizbpjt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tzklzspj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kkpysjfe.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ofbzlfqo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3dfqtqnge.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3uxliwrfo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xqckoajh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3qbrytxkf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3uwlszkmd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3qgmfdqen.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gpakgivk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3axtedanl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3rhnyglro.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rilvcpiy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wilzlrwh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qzombtlz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ptwjfnnz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fuwfapot.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xllblcil.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3lqqdjbsx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3fyjghrcl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rnlkuqdt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgwmhujz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hufrpsvp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evadqopw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hhnrmmgy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3uizenfpl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3bgityrfg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eypdlzlr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aujhclov.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3terqpanh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ejfstgvh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jbefybys.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3twfipfqa.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qgttpdbg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ksdmcpch.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3vohlwyxm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3edzjeiyq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sboipulj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3lgzqasmn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xwjxwgyu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3edosqxnz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3idusaonj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsnhylbo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3veiemtfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcyfwhcq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wqybldqg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vhoqqqgm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wrarlgwr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vnlkrooo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ghxxyobl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3erwjwxqv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fpwclpuj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3vacaqysk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xcwypkvj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nppvajya.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tfmxpjpc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3rynadnzv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3hbrnonuv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3iwkwaosf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uxoedomp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xhojmlyo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rlocrjcx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3leedezxm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3kdmxidtw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3mrmujtmd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3qmsgjnkb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3pujwsrhn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ijzluinz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kbvhalyc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qjyxzvla.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ifpvtgwf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3flnnpbwp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qpfmuhqo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3sjkubfkt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wscxptca.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3llyvugtl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eochcuoq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vqfkppzk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ookcpsui.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ztfxnthv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ejhgrmkm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dpyslxgz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3yysoyrrz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wkqficwz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3siimmhnz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3uxdejzis.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3urogsnxw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dwmgjbpm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3htetfqet.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bbarrqrx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dppxaxfv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3wgliutwy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3aggrqxsw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ywkazzdm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jrsubvmu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hyghgnuz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ovoqgtqc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kagwwxex.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hklwrktf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3grnvgngf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3klsprtcv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3knwtsztl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wibzadfw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3bbxyncqn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3liamxeoa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3mcbskoju.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3grbzbqmb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3nkglmzmh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xatgyusg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cmgjsbjg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ofefxyhe.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zmliuyjx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3avvggwpp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hetncaje.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zdwubota.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mwoqyycb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zsazbkrr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ezxczzkr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3wicqdxrl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vrfpuqls.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kguzmspe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3uymjvfrg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3rhadqakz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3uicmisxq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3idfwqrmt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jospgsew.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3spjwogqd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ephxcqii.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3pckjiega.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3huxqfvxc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ckjmqbfp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3azptsbkw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wkcjauou.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tlmeoiwr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vwkxqoaq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mylhgzcw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mndceaws.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3gwvldezq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zmirlqbl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bshkatnr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3hqaqqxoo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3tqgqtjna.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3pkqghtxa.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3tnjtsmrx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3tljqldcr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3kqhzefho.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3draibesn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dvttzbus.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xpoheude.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3vkgblxyc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3npjnmbbl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3uonmgjjt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3kfpiembt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ogszphvl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3orxkzswo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ragjwawz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wpcpjiau.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ghhhnijw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3rnyjlzqb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3tyvdagml.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fsvuhtzr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3evgpcrie.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aoxbodea.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xzpvioei.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uxvclmcr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vtamgqcx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hjmbxxfb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3rmlobrbh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pmsekjfq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xnftashw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hmnplhos.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ywtghdir.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rbxusgso.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3scqwgszy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kharreai.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xolakrjl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xrndlpew.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rhvsbfeh.html


<!-- 参考信息 -->