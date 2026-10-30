代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gviwyvccl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gktjjyxwf.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gmghsvust.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gsdpygweo.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gqcdqolwq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gdluuswhy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/glaikfcgh.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/guscpvxpy.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gtkneokzk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gfkeaefzk.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gjatbhvmn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gnrmfipjv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gsufrqtzt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gruydorrz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gkfdbonia.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gzxcbznlv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gdxqsczum.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gevfhfnbo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gihngspcr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gcmdbnvgo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghggeqofy.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gcrvoqvxw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gedlefbft.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gbiyatdib.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gosqgglcc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gjwktbnlm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gfshdjzix.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gwzvosyok.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gueismedz.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gcwebyuct.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gtojvqdax.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gghghbhez.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gbzbaxopq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/ghfiyeqrz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gqgndxgje.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gqtfrshqo.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gifoxiypm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/grujmctsy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gykiyhvgn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gbawdybdx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gxfplwhjs.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gfoffldcw.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gpqwpfjmy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gdzcgkoqa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/giqsztoiv.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gwuhcjkud.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gpszdrxxm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gbunmtqmm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gannanlua.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gkchxdhhd.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gykgzjcwr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gunkbctos.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gxjpkasyb.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gvfzkmurr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxlruyys.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gaqyxsgee.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gbfhdpjun.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gcyfwyfvf.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gmnhvydzr.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gproavcah.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfqjgtaj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gvglrgbcw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gqforwzit.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gqyzzsyzy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/ghsbzdsra.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gjfctzrvl.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gyaageotq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/grbumxvzw.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gthkktllq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gxqylxmng.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gavrnewgb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gsuxjcohz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gfnbmgaoz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gymvllomr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gupeniauc.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/ggjtogrdh.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gkvikyojx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcmjofkaa.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gaxniymnc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpvkfkuns.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gkqbdoeqg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gabpzmygw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gcasxmpzl.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gbdlixtzd.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gptdlcidd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/ggfupwpgf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gnerntovq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gyjbgvlmz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/guamjktiy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/ganvounae.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gegnkhgew.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gxokmdhyi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/ggjdrbhfv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gesbczbgd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gggqjiekm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/grvlogsfc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gzeuwphxl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/ghwynknds.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gtpdjykks.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gvdfrqaim.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gnazfydgw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/ghbfhwbpr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gsyjeobxe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gdagtejwy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gphqqzxkg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gzrncqkkd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/guqcoxphe.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gxzhiwlcb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gtgvyrmjc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gdtyqjqea.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gyzdqgbxj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gkvrcevxw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gslkyzzpl.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gykmkynhz.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/guejawzgs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gatejumcr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gaezjtlof.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gbarlflzd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gcospsckd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gbuegrvhw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gtsurroeh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gumxrjisr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/genswcwxz.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gjphowkvt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gabcmlmpo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gezsmbffq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gsxrrblxr.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gpqofhktm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/genilwygh.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gixlpvhol.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gnutmeetd.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gucxixqlw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gnopekdqw.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gcbfzsjvr.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gylkezlbk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/grjlwogxs.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gaikrllks.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gaksdlopw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/ghgqgzhxl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/ggdrxrxdf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gfijkceem.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gmaxlnhiw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gijhmpqjd.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gavtiqchm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gtkhytjuj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gimfofjnm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/ggaehkwyf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gcesrmlta.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gwnrvboyn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gpxbeffxr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gcglxteuf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gwmruvjmj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtrvryusp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/grmqhrakm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzeqyweja.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gjbbozocq.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gshepqpew.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/golihnvfc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gvxczthdq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/geisbqemq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/ghllrpbzx.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gbubfltoi.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gsfjdwrjp.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/guncivhlm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/ghzydnlbk.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gbmveotoz.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gvbwzxvbd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gdrjuvbto.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gnaduodhq.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gofbloulm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gvpzpgkgb.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gznwonatj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gztesornj.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gmpasiprc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gtvsiaylz.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gdvmekija.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gztjudyli.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gcywtnmww.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gzsunjugf.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gkhnempca.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gsenhzhpb.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gvmbftuhb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gztxxyitc.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gbfvzcedw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/ggbfiqemx.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/giocfmktj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gudsfipor.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gnhsmactx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/ginolpnap.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gldrhcxxr.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gkhovafnb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gsqnwmyjj.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gtxonkvxu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/glhlnabmq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gyduecaaj.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gvuaymypc.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnvscuvsf.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gmmckhasz.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbrihibwp.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gnychxbvq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ggptjmmcp.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gfpjvbbes.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gkmqaavvd.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gqcvhkllx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gsunsoufk.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gzlktyipk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gelkaxkss.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gkbhfewyo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gmjfbyeir.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gsrfvdpim.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gtnedfyjq.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gjjsmmhjh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gpgmxeffg.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/glsmruntn.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghtqjxkwz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gmhbskhfl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gyjbsexcc.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gwzlnqetj.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gguhpkfwn.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gpzypbqzv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gjirsxmti.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/geqeprtex.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ghnhgsajf.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gowxvutos.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggtorrzzh.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gzpecmlch.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gitttpqch.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gehdordlj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gfsmskprz.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gsjzksmgg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gnaihudxj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gcrdeybif.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gicdcpiqs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gjufaeiei.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/grfewxknh.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gveogakgq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gmsrgzmbv.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gqokwwwcs.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gqfhalllf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/ggdnhuddd.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/grarnawhq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gsdhhrimj.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/guqrcttvz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gnqfdumla.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/giuhhtuoc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gbryiippv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gymvfufab.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gqcesadpx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gpwfgatcy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gmcuthlaw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/goyfuefcy.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gibohrtxu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gpyriguax.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gokxotahn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gcsjzknal.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gggfxugyu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/grgxmpthw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/golyhbgcx.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gofciprkc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gpghiuwxz.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gnytoyozg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gyhvojjmw.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gzpyutrde.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/ghsseswgh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gkqsyxctq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gpchlifph.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gwacpzhmz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gpcvlvoaa.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gzadkmooa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gfuntpxbb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gcmsogeaf.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/giycxirqs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gcjknavja.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gkulpidfv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/ghethpqky.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/geqpxmnib.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gdeldrzhr.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gxioboouc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gwnyyankt.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gbfecerde.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gvhaxjcvi.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/ganaxsuyk.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gelooajfn.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gmfhpospg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gmstxgocr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gpufcazws.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/guayqcroz.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gclazdxuk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gufvvuvtf.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gzxhracbe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gthhnbqns.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/grcurazxi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcwpctpxg.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gswvtymob.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/grtuvwzzp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gluwqoels.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gmrqelpgt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/grhrhnhtf.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gldasypkl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gpzggckkg.sHtML


<!-- 参考信息 -->