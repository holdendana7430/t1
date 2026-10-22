代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zerqnqmd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qzmzowwj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xwfgxrjg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2dxrthejm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2aqcnpuao.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjbqsfyq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ccygnpao.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2tjtwdlwy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mrjvictv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ekzveqtl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qllbnyqz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kdlekdzr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ynscikpd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ssspqdyo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rwibhmiq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2lxtltwcd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zjjickce.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ivwgqsfr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2inzdlgit.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xadolxdk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xssnhkug.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kntffjnu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lntadcxv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tcbzjsgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygikveff.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2snauzcrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjzrkoxm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jvgamciw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2fukvhgkt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hyedytdz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2cjocquqx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hgchdmgw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cqvuuhez.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pxksigka.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2nadixyfs.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2uufvzlrh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lismnezb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2texmarnl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ooaibchl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2eqstsxwp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gfjpctml.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rxzllsmc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2aewvujny.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zorqczjl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wzfpuxqs.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2kzimastt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2llfswsqq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2certsekk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ijcfnucr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yygnrcmg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyybgckg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2djqddjha.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qxnngxqz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xcpnojcu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kixhlqjz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nrrmhfch.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2kqzymxij.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2encjziqy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lebqgyem.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2sfcdizvj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wjrmomqj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tugpyliz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2byhfkqdn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2mlfjiden.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pzmhjzol.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2lsfkxkoo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rtfzadvl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jhlkinsj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2faqnbbkn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2gxopmpdr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mpmvwujf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mfzuyviq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ydnfpirs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2amnapbyr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2noyouweu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2iacmtihv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vbxjfdxg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2iyhppeiy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2rxjjjslj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2hiurfnbs.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qqpvguhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ginurjht.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2sqmoygqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzlxtpcb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2scodqfdp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2jfjcbuhc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2eekvnzbs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qwqsubbc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ntwkvvrs.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hhmsdnwg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ypryjkin.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xerquyvj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2suvgipkv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2cofqwghq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mzpphjkh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2sijfgbej.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vwbhpiah.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jjimzouc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ayouqqql.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2serxugpr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fekouhok.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2aotkwdfw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eseozivk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2bafobrpx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ezdosvsh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fnesbbph.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fahstaqw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hdypytlk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2agnttwto.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2lzeuhcea.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2biskixka.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mhaxyfmv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2undsnblp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rypinlhs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iteqobrg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jcsywglm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dyjtqivr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ssvdcrnk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jmmrtmdh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hpguzama.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2zndtvkyb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2kjxdisqb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ekcxrfjp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xxuphvun.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cpkgflqn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qnhanjsh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zxbltukp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2haxirnqh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qzyqucnq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fzvitrod.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rehqpamn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zihkbnae.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2oatgqyse.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmkvwtkj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzwajmwb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2eecnedya.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2npppydib.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ihxnauep.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2lvhtipwq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2bbpbuqzw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ubcpjyjy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ddggfiyy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2huyjbemw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbzvyuos.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2vthgimsa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hykfhyfh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2txyxlqat.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bojoqsil.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2wkryhopw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qquswkux.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2betuyszp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dozuqvlg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2iiaeohpf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2dsnphgqt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ehirrses.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2umhhaqbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxavztri.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qndgutjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqacfspv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fqvyytll.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mlelyxfq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2htytwelv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tyqszjih.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2cxdhrltf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2syjhqyta.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rsyrfwnk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2rpbsfrrs.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2awplxqro.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2cquhaoka.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nvhjkryj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2bzeiwtav.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cfmzzpai.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2oavpobch.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2fdqwtucd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2habbsior.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2dpcrdsvq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2akynxnjs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2svceykem.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fkxvjlxi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2lamrmhti.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2jlhbsykl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ucwgxnxq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pkojzcfq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2hdhragaz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rnajuekz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2wpwvjysf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xnkmoltd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xdlrawge.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kiiruzom.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2dksdtfmq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2atkbpfqo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2epoftnoc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2upxsjxjb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2qacmxkzu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2utrnovjj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ssiojgon.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vssyzjdp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2rxfkypyt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2vxlsbhmj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lotmkjab.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vnuffycp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2pctdztwa.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kzeopysn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2wtilytxw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2hbzufyba.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hygwjcen.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2jmbpblqa.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2yqybqosp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jsmyujdv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zrwtsbak.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jnimyhkg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2bseeykes.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qxlytcgc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ffqcprpg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2jlkkpwgq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2sriguosr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2cdegfggl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2csfeepxf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2efcguclc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2duzirmed.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kiutidgg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xxilqoiz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yljnqavy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2emgwsshb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hpsdeglv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2pmvpowmw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kedyhrmk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2svshttln.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ayejhiwk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gmpmktxa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gtghufbs.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rnogbmot.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zmnlmijg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gqxvhsnq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tiypyjtf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2bbdtgupl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2birqzoix.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tshjaflo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cmscbhis.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2xopzhpqt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2uxlczsee.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xgugjmdq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cwmgzkhm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qkxgcfyl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wpsrfsuy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jytjqtug.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2depsevwx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ticpeutc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cbygzkde.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fegpfvcs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rcvxdfsf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2xdloxvcg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2lvxuoqmt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2dvkbrhzn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ftkgxnac.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tvnmceqy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2cshzjumt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2odkjzxly.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2virppvvi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ohfooivi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ioaijcem.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pppcgnav.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ilzpjeda.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ajebllma.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ngxojiuf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zzldvvvr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ngwdcfqp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2awmdthqj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hxjtudsd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ghtpfnbu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2aheptcdr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2cdgzdkcc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gdsgdyuf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ngzimzlq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2uyqctezk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2mrlitkdk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ftchmwzr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2sgitlaoo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jyunwvxq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2popbtouy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jocfggvn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2nnoypjmk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tlulfxsa.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2dfsauenk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hkkhzwmy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2emiigjkr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2bpabpjtr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ruhuasbh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2juokffyq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2fizbnnra.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uqleoznh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tkeaqbba.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2utsadygb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2axpevzpx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mkedvptq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lgqwrsuz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gmlfurkt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kljsohka.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ngotlmww.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xaaifcar.html


<!-- 参考信息 -->