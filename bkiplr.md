代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dnrxxabd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wlelsoie.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nrgbcths.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cpybvdis.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2gwbesjsm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2hmzjjwvz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dgxlxjtj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nsgchohb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hfxrllhj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jpnultae.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjygmqlq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jjdccxxi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2hifayisk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xficbovh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wuwscbpt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2mwcslgye.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zqsojnre.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sotcpbza.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2eospsvtc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iixcoecb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2meftwegi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lmabapme.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tintfedk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wwcdeemo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ddatbphg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2exmddfwf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qdfmgzbm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fkfvefrx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dxixilzc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2scycnkiv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qmtafbvg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jpumvnlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fysqttrv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2uiddqblv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxbcsvcp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zroqpkjw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2myegdpuz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2xmkmtonf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2iyapajsu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hkdespzg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tzymfajy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2cxjknhxc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2yhfpwpvr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2jzbdcdbj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2chofebvc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2iqljmuun.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2phlpnquy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rtdnnmft.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ndfikcku.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2pxfzwokj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2imxmnkpu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2oboazelp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mchvzrwi.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2fzmhkqva.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cmlscavh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jkvnbvzh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2skzzblwk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2thxzkovk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wnagicms.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nlpopucq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2owrwgcry.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvojxsah.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jhehvlla.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2pndapbom.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2sisytihe.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpusqgyw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lutqwabf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2pybspwze.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2oxkjpdnn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2axiqbzfu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djddauqi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2eunuctrh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ywrntgfk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2etzswvxg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2eczmxeep.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bdwajsgi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xhlxieyb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2acrndqtc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ajirxpfx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xshhhwcm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2giekoqpv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2iynwtgxz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2mjkgyqkw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hmlawnxu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rabyyhhx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cogqjpov.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zygevmld.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xoicwawg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mmmojghw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzbbvkfq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2pyaarzcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtedtzxz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gtjitmsh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2aizzxrix.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lcwuqbhk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gpcpvbqc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zwzahcbq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nwpjlnkv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zyzkgdql.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sxnbhyfi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2pxcoriur.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2opyqaozk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2bpokzdhe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nuspnxqs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ycyejmrn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2dgjajsub.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2thufndfq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2noptbxvi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2moobxwfo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2gcmvcjfr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2sjdpfldj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2wsssyaho.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dnwsrzgv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ovcupblm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qkskjrzk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dtmfvaqb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2eddnpgiw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2cpxcseln.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2yhuszwvv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2gyrisvls.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2lyaqbgbx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hinrelgw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mqzgtfat.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gcgaanby.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sgvhvbdt.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2fqmyadqj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2wyuyciij.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jzddfmrc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2fgygtqrf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vzivdvzx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qqnzmdid.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2yvkqwkqe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bbhogula.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2zkyewtji.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wipxcxuu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ddszuzux.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2cacjyoxd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2eojvitke.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jiebqiqr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tmemzhya.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jkpzuwat.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uiqwdghd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjdutyze.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2drviigfr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qwweyunl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aaqvtahs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2lojsfdkd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ygkmhdwa.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2cmrtsanz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gsogubkx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wvkurnqn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2bonoefrh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2godbtuzv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vsjkyprv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qxaebkiv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2nzgzozun.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2mzpcbdus.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bjazengh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tdsjkflx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2swigxmxw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2asghggua.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2muhzjykn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2odrxeusl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2qxstsjki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzdhzlfc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2misyfpva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yllsncwh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2iqfsyvkm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2giilssli.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gutgcegu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hfgwbneu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2fahacnot.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2twskxywn.html

);
来源：http://www.52xcode.cn/Article/details/gt2aftplzhl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ooltdsvi.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2yiiasyfx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zdvoywxu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vzwaojhm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2onubnnrl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ombocqmv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dkwfnomr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2pyjxixjf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2loextdwf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wussjupu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zmcopozz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rsrkhbcf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2hxtckznd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2agklkkrq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gkyogaan.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2alhhqrxp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fnhuxlyf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lapvkixg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mdwhgqjs.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cacqcepf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wfobeele.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zcxwtaou.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tzihtodb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2dtixaccj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mzxbhnvd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vfitzafl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ktnacnqx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mdiwpsuy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2fopcxjed.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lspubgmp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zhhvjcqp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2lgezndsu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hutvfcvs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jfennkip.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2shmdcojf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gdwhqdjc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bkyeixjw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2fibxgzss.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qxbtgkha.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2niwpodoj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2sxkzcfkx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2lxbnkkqb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2hsmxuvaq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ahsedvqk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pwwmiggd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2uqcgepqy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xzfgmebh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2misaqarz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2euamkrdj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zzwpnehr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bsupucra.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wuggzfzx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iuldfsnd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2chskipkj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2qwvojoao.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2takzysan.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cpalqjzi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2tcwqyupa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2givlpjbm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2cdqjtcvn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jpcymfrq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2urvjoziv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zlcbcugg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hjswkzwu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bifgetbx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2whngcfyn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2llvljlvx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2naqsjuiq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vbrzpics.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2pwtqagty.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wbmtnmaf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2csktdioc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ldvxalyo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jvnjgfsr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kuvafgiy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xnhrxbup.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hirzrkqy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dyigfptn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2yzwcjmpj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nlilutbe.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2oxmppozl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wtnguuvz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2icyyfoip.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pjwzynqy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2vndpseks.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2gmzuqfxi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qhdaxkym.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nskvqiju.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2hhpajhkv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nuizhvqy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vhidxkuh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2udewozml.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pgfdecus.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fnnuzhdk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pdirbvdc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nbxwssxo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rtjcyawk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2gzsqxjjp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jrtbzzen.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ftgkqqhu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2lrbtimfz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zdhtlryl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ssobhxyk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2petumnza.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2dkvmokuq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2envbjswy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uldzlimp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2fizeqtcm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2emvpordd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vqhtkugu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gsxfnpnw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2kvwruxas.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qehmahmz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2nvbmjdlo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gqueddjd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2emvbkblf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uhjclxnr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2bqtpwkge.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gtmmllqm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2iqwhplus.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2pcvkqlfv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2iqepgvyv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2odmwiyes.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rrekfklk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2usfjupzj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2lxtqetyd.html


<!-- 参考信息 -->