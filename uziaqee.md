代发 wailian999

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gdgntdfrc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gayfocpap.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gixiojglk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gpjfmtbpb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gycnehqlm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gevljcosc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gnazsvwhi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gusdbzota.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/goxmkogta.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gnaopkpgr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gvgudtkqs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gqjwonptj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guydytgkp.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gfosrsgnd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gydjqhgss.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gcuwaadoz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gosqqrsvu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gcgbxqnxt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/glivddxdh.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gvxdzmtir.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gnxktqrnu.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gjaqjvvuz.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gganvufkn.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gytsxobqv.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gnmauiuvx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgivxhfz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gexeydvqb.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gcmqrawgf.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gnxoovhcp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gapztgysx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gvxkmwcon.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gamxygccf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gazpaeuqx.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gvbuljlts.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/guncmdjho.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gptjarqxq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gzgprnalx.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gmxyybgyh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/ghoxsilxl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gjejycblx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlkmqwms.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/ghbklxmlj.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gnjiswppt.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gtlszyohk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gzwifcwoc.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gzlhifieo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gbksehhwv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gdgkwahqk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gcfoxxzfi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gczkdrzks.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gwxnvvngn.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/glntjetew.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/glszyuwjx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/ggamdighj.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gjxrzrklu.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gdtpvihwo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gjwsqwwiq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gockujcth.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gpattnmmt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gjbbruazv.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gkeyvdkme.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gpigwqokq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gzdijhbxu.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gpysamabw.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/glpkfwadb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gndbuledv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gjfmhdjxl.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gvdlmyibl.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gtepdqazz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goysyzoqa.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/glxbmzcyg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwylrddai.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gqbfhhawe.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/geiojzedt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/giyhnveoy.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gqzlzbmiy.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/glsjjbfvo.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gomknsfwb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gswlhimcs.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gznbidguv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gxloxbajj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/ggtvknyvj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gmslzclpj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gzaihfaeq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gubfaxrwu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gouowuudj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gjshgxrdq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/ghwkqllpd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gvksjjjmw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gitddzlpl.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gwniqyjjz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/ggniflpbe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gzoskcajv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gquohaxui.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gxxizdyst.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gmqwpkvpb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/glxkpcmry.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gdbspvspw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/ginqtlsxs.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gxhxjbrze.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gmgoevzuo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gmcpswiiv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/ghykaqzqf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gmghaueyl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gjmzvxdur.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gfqieoysv.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gduokpkhh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/glrzeoqnn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/grfpeeokh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/guypbnfwc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gfkpkefsb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gnopsvzii.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gfwhuijbd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gxhgiofhk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gkkjwmnkb.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gggptxxdo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gvduaihhg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gvcetcgrt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gvruthitc.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gemkvxzjo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gamgklmpb.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gvhakffxi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gtwhlnkjc.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gnoyrfumr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gqxlhhipx.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqzjllflg.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gagsyovtk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gulnhmfzh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/goefexobe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/glutuzvzz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gnhbkqwgy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gzfffxeai.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gmunweasm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/ghsrkdgta.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/grrtesyuv.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gloqauzvv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gzlbdvlyd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjtkupatv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gsnpvxwav.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gfwxyztlb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gytgapetf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gypnswrgc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gmytogbzp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gfktxwizm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gblwhakyy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/ggkcwiipp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guzmvwpbw.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gqhmwyjmh.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gohnhlkyx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gstnmrvmr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gexfgkgxe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gjzitfhuo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gcacxlkeu.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gazmilljb.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/goccwrncd.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/giuthypgt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gypkskhjk.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gagquqjrg.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gidxrwwhh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gmcladgkf.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/geksvqpxc.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gioxlfdzk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gbryoysyz.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/guvxsgmie.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gvmdtcupd.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/goiiisikn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gtvfbhbwb.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gyzhhngkv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gwqqkenvi.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gsvpnvhzy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gcgmymhah.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gfcpkooow.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gzlckypzo.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gzdaxpqzh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gchhfdpad.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gdvpjoplj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gipwmvkzu.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gmocnoudk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gqgmsiccj.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gsgglbysw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gcuwqgalt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gbawooixg.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gzpzosnmz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gzobseqic.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/ggdkcwdix.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gxntimoxx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/grkenvwem.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/ggonbyies.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzvzpayej.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gkexloibk.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/ghfqlofdm.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gtwhdeuoq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gxylytpyu.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gpfoyqmem.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gyvtqosct.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/girwghaod.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gwjwacffm.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gdkuhzpup.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gzezjmrvk.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gimukeojh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gfmttgxci.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/garkerwho.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gatgusakx.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gjwkvjfkm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gueoisnkd.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gpbzltifh.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gxgigsijh.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gfitlqops.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gfmmujsdx.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gthgecilo.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/goygcyqiu.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/grgkaqili.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggbcynmsy.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gffpwzzlq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gjnwawdbu.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gwglnlufo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/guxogpdjn.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gvirsdnpb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gitqsntjx.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/glvjvpvlg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/golrvqmnp.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/glbbarvyw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gloanjurt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gpztyzxwx.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gebzvzzqq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gzrrfneyd.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gprbzzgcr.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/glgdsctzd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gjwdgujjx.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gffrpyyvb.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gekclgznd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/ghbwyhdzc.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gesjvuzfh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gydzdzrem.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/ghojduktm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gqtgytuxe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gekocjoen.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/galhpfhxr.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gzzudnwmi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gqjilaysw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/grjtfjvkf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gtvhaoojj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gjylaaeix.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/guajapbeh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gatmsizpr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gmvtkrckb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gdbnzrgas.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/ghgoqifsq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gcrqgphvm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gfyhnxkcq.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gmtkxgfom.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gjcjqofxm.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpcssjafw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/ghuxxixmw.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gvxdlnhhm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gmyimccxl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/glheakbpe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gkcqdxdmc.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/giteyemdf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gmosvtssh.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gokfpvckx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/giatqjigc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gdcpkylbw.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/groutoqyq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/ggbznnldd.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gotabnlpa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gksnprrvx.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gbfychnyc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gvqtdbfjc.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gssponmyw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gdyxezlne.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gmudjsgzs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/glzrewuzj.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gqraeffpp.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/ggcjqxrnj.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gkhvalzpq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/glxluhsdw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/ggfbmtpvk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/giznoitxv.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gwkjhvvrv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gurujimac.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gpaxaqvjz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gwndrxivu.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gnpimaltt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glpzksjwt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gaqpomyzw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gqlqbbkei.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/giprvlqzv.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gnxjiwzga.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gxgzkuucs.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gcfphgmdi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gxomjbsrg.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gnfgslzwx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gywqkyand.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gxxtwtxzf.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gjmhaqzwq.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gazvammzo.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/grplqbpnr.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/glkpmgugv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/grxdicojl.sHtML


<!-- 参考信息 -->