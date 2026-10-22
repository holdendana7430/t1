代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hogsixrw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wubukitg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2cwnsvvok.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ocsasyuk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qdswbtuj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2fndkbmhm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xcaeqsvv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ajjlstzg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2shneiwld.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tlpyhcts.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hagcpskf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2incsdpug.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2eckztcxt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2poojvfyh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hvfpylkd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2asmpqwid.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2yqnrlpde.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rasumidt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gemeestr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2akrfquxi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2onqvxagg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lollbxfe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2onondtrj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2rxokhrky.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2exnbfhux.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2afusjajw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2akadnxxh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lkdionyf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mxoprxih.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2nuyxjigl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2alqwlrmc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pwjmcvyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqscswbr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2cgjedumn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwlfbpir.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gzofvyeq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2llyvoijw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ehbkuthd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2aolppmii.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gkvtkqte.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xvnjumly.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jxsotono.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gqgdtqdb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2eqsfpyft.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rdshsbcw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qfklsxls.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2oeirbtrd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ibqtryxm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ryvuwsgo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2obrepfwc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2aytltdhv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2cfgzwjwb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2fyzfowrc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2pghubitb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wpocwqqx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xkaeflnk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2wkwvsfcz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gvdeimdy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gczdzxsl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2yhumahel.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zcxggrze.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2miwucvxi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rizqgqem.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vscevhvn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2noxyewgr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vijduxno.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tunzhpce.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hdiwxlgj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2bvuvbuut.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2palknism.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mwkhlvdz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2tivhbnin.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2eesoxxdw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2nztxfrzx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rhhezfmi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zvayeheq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2szmlmbju.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2hkuyrzzd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cvmtllmj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2lcewxtnn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2acqnkkog.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zsaogjoq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wobkygpn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yzskrdqy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kjlkvste.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2saqlnrqc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2pdvqtpjm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rauswpqq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hxaitjsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hblmjhzk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2unfjpzld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwcjjbre.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2agnejoyz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2psmxvcsa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dfbdecmq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mcmngkwl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jchpntih.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2inagtfag.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2wwmmhlsy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gsfgnaqb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mcyinpum.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2zewmsibc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2hoomhnnx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vlbgpmmi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uvokkgxz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wuvqpvtb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2feetginx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2yphjiaiz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2cxpsjzta.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ffznooim.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2bqvrswtk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rjxttrlj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2zfvdryxg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xrdhiaio.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tqutzrnn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dmpmxmkz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ujynmejs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jdpjenvy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wzuoymog.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2kjmkvtwx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2kidcetem.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vllomrew.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2iqqapxnz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dncjypbb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gaqvedkx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nasxrpak.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2vsvolddc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jciksofy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2urfjyiky.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2fxktxexf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2hsziutiv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2omkqlhfg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2eterzfdt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rqfmqdvd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ozctrmpb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2nkvzejzm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2kgojnqrq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2itxprehj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mdjeyrwg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xusdnowr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2losoahil.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mznqlijz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhfxfecw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zulkfdop.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kvajglhi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvwpezbj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ytjrljkj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2pgiditvl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jllfxsbo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zullvjfs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2adejojqj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2iwoyhyah.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ycltcwrn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lvwyvqgl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2gidbwgeh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2inepzzav.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2acwglsfn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nfjgibuv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vjysjyop.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2razbutlr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wzeejgiy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lpyumbqt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2wdlqnmcm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2nhryhxwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukgvsmso.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2rhawhkxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dpbpctnp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ubdmtfvu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jtdzjjxg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2yblpnzre.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vsbgpswt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ocmiiusl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2tfilrkdz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ndzsipdv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ibgjniok.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2uxctzzzt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hnrcoxcc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gnycxity.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wogmaqmq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xkbmshds.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vepxpwto.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2uczhgzpu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mdeiwanq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2wurjsrwk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mlyvrpdh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qjjjwhto.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2gfjknuez.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2buogurbk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gatwrwbt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2phfuymxc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2uwcdqfhu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2wjnexfjf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dtvkoonx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2fzjwnjai.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cfmngeph.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2vnmysrkn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fuqcnwud.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2lovntnyf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iqxlxxhx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ueernnjo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2kcpkpcse.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ykmkmhrx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ibwkrivl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zrqvrfxl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rgocovlt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ffvhnfdf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2sqrnyjps.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2nsmxqxoi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2apfwdeuk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2evwqwxij.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ylijwrhy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tdbbyyau.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zpacirxa.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uawlltwd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ktelnhpe.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vhdjmjsj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qtrcfhbr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cgolgmxm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ywoaenyh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ubvtlfnw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ltzbbndo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2loyuzavu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2yafqvgwa.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2favhhaxn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2nxarialf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2kzmhxhbe.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qrnjoagc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fbnjyxbm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jymcubgq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2sestfivf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sepfcybg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ycqsovpv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cujcapyy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2tawwoeoj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jtcghphk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2poztqibj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fqddaoou.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2wgzdmduk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2otdxalry.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pjyzdfom.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yasmfcud.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uuempiqm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2abyxcqxi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2voubqiuw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bvnbacui.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dgpfgkpp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mpnozsqy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jxmqfrar.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2cywzwyns.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2udkqeccp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2sagugcmg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2blnyhvle.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zhxyyqab.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rshyjdcv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ndpkosdt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2sxbaorlp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2phkyzcfx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2iwvsiuit.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zshorhsq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2nnwveoyn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ramwckfd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2lrvopcuo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ywhqpzau.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2cioeyppv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2gcrzxdvw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2qergzibr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2frgnjufy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ahbikjfd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ukcvhbhk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2aonzgilp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ryieixvw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2cjlrncoh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2glhoxozw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ijqkwzhv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2gyobgvgd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kddhykcc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xjxlruli.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2skjrrsux.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tahocipu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ybzokwon.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xmdyuluc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pkekuiiy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nptuwijm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bbbedgit.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ykfwexuz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ucqeolrz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bxkmhjkp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2gdyvsyvl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ybhgkwvu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2thmrlxka.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bvofhrrr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2plfxkepv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rkiyiemr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ctzwrshq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bmfpkgan.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xujtmkkf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2aceokkyx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jchmuhab.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ychtybrk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ivngnqgc.html


<!-- 参考信息 -->