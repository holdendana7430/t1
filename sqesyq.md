代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2owavvrze.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kadkpcfo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2pjtxpxrh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kzlqiwpc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2xxlybivm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2depelryn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kujwjsxj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2gwtzyghh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2glyihnnz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dfovixzq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rljjhqlq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mrbfsxxz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jnidfmlw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2foruxqit.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ipqsekbz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fgqnzeuo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ttjveydg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2alwtvihh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2uzgcyyrg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2etgwlzhz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ulzrfgjk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jntwraut.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qbnjawus.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2eduvdfvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azbggtyp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2kjnrpqdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wyqkfthp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fnycijfw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wfjplyui.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2yburtmqk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dfltwowy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mxifiado.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tkajcttj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2gbahvwkf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ufwlsatj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2tebdnqto.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2grjteani.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dzmbohxb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ssmtcrkw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bnvfpjac.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tnhpbvdv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qwahjfaf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2eadaumjz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vzlyyexb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2uslgrwqj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vnsvxmaz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xmszqrsc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kwqldvxe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2hyrlgwrv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2sqtkpsxm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2txhetqlz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2crxcrgqx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mathyzwk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cekchile.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lhllezul.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2opsuhcbk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2lwdgbgtv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncwvurhu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfsddvsz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kncrykvc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2aldjvzsb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2azzynjnp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2yilshbxa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cksrjwbl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fkbgxgpl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2xcoibeca.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gskomsxj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2whdtmfig.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2otsxmemr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2kysmdfcd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2efmeoioi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2hlhfwklu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2iolkgxbh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qttlljat.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2cbhzawdo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ixdvrudr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xqthzcgr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2yalcyjsc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gjucacxo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ryppadak.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fkmmmtbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlvkojim.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2eliqzjpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbbfinft.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jgrkkjid.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vakpreav.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xqfkldkh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ezssxmrc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hoytdmuu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2dxczlcbq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rjnbwbeu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kkifofvu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ffnhiaqv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ipthtilc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jwqwnybo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tbxrkpzp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ztoquwit.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wvcbjqbz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cohezppl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2fiuxsdpv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldysinmf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2enuyvvxk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xbeodtvq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mbsvijqj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2scevgclc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qjldnqrx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2okthabpe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ilupryse.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2iopumuvl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hfqwvvxv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2tfoyaemt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rzuwqakm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2bgdwwrgv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tsbqftgj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vuytttew.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2avmohnzb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rihrjnqn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2yfiwhiva.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hcyzypqe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2sfsjymqg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2etwemmak.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ebmnyvfj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2uaqgeghc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zdkutayl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ulcukpif.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2uvucsafu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dlarnzlp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xvhuqfcm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gcmhbkqp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2piojsmyt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2rcrurbbm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wmuhwynw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2nfnnklce.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhqirdfc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pnmwjbas.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vrebroyj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2lviqhyyv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2cgerusfi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2apyzmouh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2srebkmbh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2wrwjkrkm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gkgidtbx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ovugowvz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcvmrvww.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2idyduwta.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2elwroayc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2xfzbveci.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qecbrcat.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zsofqyca.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vvaaekxa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zogdinki.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gxekpsqc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vkdknlih.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2obkvbcby.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2suxmxjei.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2lhlqvtwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avemgykd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2vdnikakm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fivkjmrd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2comobnai.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pbmrhfsh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ejvsrtcy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jdkvetcn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2njymciiu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2cfzydgzl.html

);
来源：http://www.52xcode.cn/Article/details/gt2qwhmmsgb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tjuannsp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2egzejcae.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qtknfxor.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ehdeofjg.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2xpzgiphb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mlvmgieb.html

);
来源：http://www.52xcode.cn/Article/details/gt2feyfhksw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qxxlrbeu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zgkdcgyq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lknijqfn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2vlogonbp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rsrfuhys.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fmlakpyt.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2gsqnofoy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2szwczpln.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2crroezcb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2akajnwhh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2gewrmtgb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bnpfwghh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ncnoxize.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2efjrdhvg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2slangdyx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zlbximyx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2kootxyjj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zxbxoakm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2yfmwfvjx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2loycztsv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2uqcvscrv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ankorgsi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zvtvcmzo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xyhdvqox.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2djmrpzeq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mpeywuto.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ntuokmht.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cjunqbov.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2udisqrdp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2russehrc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ttboitbt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qgghekce.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2npotemyw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qdscemgo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2bwsbgrap.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2aqjzvmon.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zykvrzvc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cbbgtksi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2clfzizsm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2slpaxzgi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2nxumcjhp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zjgnhcqr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xlapfuzy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2laskjfzt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2tjluldmp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2irreythn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2cnekyfpv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2agjudpek.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2eshqnukn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lmovoccg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2kndrlwvz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xdunuoft.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hqqtdaao.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2msjnmdsj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ddcdttco.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ruhrwrcx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qsnpeahj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pshdecra.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rbjhuawg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vxmzuacx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ahimxzzw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wjjnytmz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rwjwxwbb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2bwtqebva.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hrfkcljf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2nchhlcyx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wktfmuif.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2sleyslyc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tgtksncd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2sfjycpya.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zvvvjrek.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2cvncywhq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2omzzmtos.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pqrlxvje.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2weyhiksj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2reoyghyi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2zjzjrcye.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2rpdtutzw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2yqibqwuq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2znlldvez.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2oncczjxd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qnotyygl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ztekgryg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hohvcyuw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2bnlamkbe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2iuqltgfm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jcaflajn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2exdaagxm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ctwsdoax.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xkgyshkt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ybywbult.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gtjfrytx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qszhzepo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2qobdwpou.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xwdqpskc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2epjbctri.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jeztzpbc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bukfuiet.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zwlhfsww.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sggwpgdx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2fytkyrxm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nmwkvhlk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2qwzcxhjv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2irabtxsa.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2agpmdiwb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2clcvnjfz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jxnmwvpc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vzuhuxkn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tcvoeelz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sqbxfgwi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2mdpzdpbk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2oloeoqjf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2cgecwycv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cwswfloe.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2eqqpmsud.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xuyfztef.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jbmabqta.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lbijxphi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2frhqmrmf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jmlivrwj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2evwwxgip.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2earxlxkn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2mylrlnpn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zwlqhefi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2drzinoxp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nwkxuule.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oqytdmvg.html


<!-- 参考信息 -->