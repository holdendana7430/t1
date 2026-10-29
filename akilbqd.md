代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/goctlklwv.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gkxjczmxo.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gptrwxjjz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/geqkvbowh.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/grcieevke.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gomvlybvq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gscpsxxbc.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gyphwpwfl.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/goxbyikkh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gcblyvbub.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/ghkbrsddc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gojaadgfu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gjkrfmqjf.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/grfjjlusg.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gnmihymkh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/glvsygiri.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gliwwibdm.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gwrspgulh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/grwmhbyrb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gwcjsgpoc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/goaqoioij.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/glbgmnhml.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gsnwlcfno.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gnixnqjfd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gzwfbfitc.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gixcunevl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gjfdhtunj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gykjsofdu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/ghojegnsq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gugqfegjz.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gixsrlstr.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gcgxqhmff.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gamnyypgw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/glkjjhqtz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gjtcipghc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gvwnsghyc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/ggcxjcvej.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gynhdnfwb.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/garchknfo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gsigbwwbg.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gcgkavbsm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/geikzmplg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gsoatumwr.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gnjnuneds.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/govwlxmzq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/guhoohwhp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gnersnmii.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/glrprijbq.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gjyclpdeg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guctojqlp.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/grmcjldsm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grhscsjkh.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gbjxgbhan.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gnghmieej.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gyrjfgiwn.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gcjndsynj.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gwdjganxa.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gpmeorcxi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gvohbrphw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gziushbmg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gsxaybcwi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/grbvaehbp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gcabpghxy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gjjfoszpy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gprjpsjll.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/guuzebjmv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gkcxpygbt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gvecawxow.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gtadtqias.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gfxcnsfny.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gexvypmeq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gaxqchops.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gvwrlxcel.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gtjvpbdvd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gosqbowgn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gmnjxdohc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/glojpqqrs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gqzvkrtcd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/ghknnrpjz.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gfkoqcptm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gbdncnjjp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ghmonqday.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gkxgwnlhd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/glsvnthjg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gvbzeprhf.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/giejidpnk.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gfhopjula.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/guyaqqpno.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gyqljsoww.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gekztoyfq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/guljblgmp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gcfaqqejq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/glgqqgytr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gkzkkopem.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gsjmyzyki.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/goanusdqw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/geqydymsv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gkkwfchtu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/glawakoqp.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/geuwrhhlk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gfuopshdr.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/geuchyjvg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gmdmxocwu.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gwnmlqliz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gwbfqihzh.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gehodrbgl.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gqwjhfuvn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gnjlyvqnu.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/ghjefyytp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gbiczlmni.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gjredisdy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/ghderijow.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gqaiuqcyu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gwrueytty.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gxbkjqjfd.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gocgrpajr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gevirzein.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/ggowmkvoo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gcxsrfoxr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gjcwfjxks.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gsjjhstqz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/ghkzgfadn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gznmkbqfx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gcwnaipud.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gthqnhakx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gfocwxxjt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glbsjxiss.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/guzdqgxwx.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gqwjzmdgh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/grtugkrge.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gkwnwtaot.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gjimhilre.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gwheqywgd.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gpphutyzb.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gegpsufir.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gbxhltaef.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gvweugjfs.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gvqmjsyxw.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/geeevpeai.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gnityfwho.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/ggzutautf.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/goqctpzwh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gbvfzyscw.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gxisruwli.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/ggcgxizdt.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/ghadnrlmn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/ghfibkqui.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gksdoudiy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/glptkpztz.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gnsnpwfal.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/guwxmjxcb.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gkquduquf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gtsvznduc.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gebpnxpnw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gvbstsugo.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gqoogglnp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gyvjoxdmh.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/ginijpexa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gsceqahmy.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gyayeuoen.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/grngazkho.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gqrricnpb.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gpjensdpb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gsjlrqjlw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gzzlegbnx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gugjbqpaz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/ggdtppyot.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gamhpajlf.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvezzymaj.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gbbybzobm.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/glvgvnwqf.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gytjaerxh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/goidfmnvz.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gosftkkds.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gsguxsvqm.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gvfeumjnw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/guvkfljnx.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gwsstpuem.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gejfpassd.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gfwfpcmqx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/ggrkfpijc.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gmxoranjy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gjyamjpqe.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gvrbhhgub.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gprepbpkj.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gfhedbqmo.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gctnekzqa.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gcfmygnes.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gdoggtczi.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/guvkfoqyr.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gypxdpbid.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gqpluceyw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghbbdksjv.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gwyjjkwgv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gwphhurwi.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/ghzpbjmyy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtzxkcswd.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gnbckoyxv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gaiweqdel.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gzuysscap.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/ghgfachlz.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/goorurmfm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gtbsnvaeu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gdlophyam.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gwvgrzxcm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gglpirdaf.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gufaspukd.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gzoqgjdrl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/goeruujay.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gvafmrdpk.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gcwcawzvm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gluygobqg.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gmfapeeuz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gabcziwll.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gamuoibsv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gdwkleray.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gevpjvxcm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gokatjyir.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gtitkoyxh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/glklkvsdj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gfyigtbfj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gmwortbef.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gvbxspgjg.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/goesyxoxa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gcjaqqcnu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gsxzlwfoo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gzjwunasv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gtkdufwkn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gbafbhfwx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gxvrylqzo.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gopqhlwsq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gfryejdbw.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gyjgrptxc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gupqbghna.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/grqymvayv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gksnajtwd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gkzdfkkpt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/giernxwgs.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gmszqomqt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gbzzglexp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gbdojmdsm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gxnwtsvzy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gshfaupxy.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gjrgkzsrk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gbnixduao.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/ggfjoexxo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/grwyxxfes.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gwtsfkvow.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gtkkipxst.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gedokxsme.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gfnmvgygs.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gzftowgiy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gqrkafxov.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gaqiikwna.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gzqalixdo.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gqdrgtjdx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gcdnwpjsv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gpwbvsrec.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gxnreeits.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gxxdnsiom.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gubinpkve.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/ghmfocntf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gzvcmfnpr.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gbibqcqmp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpuvreskq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/grgtvxrjy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gmayuzowa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gxdkmfdfv.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gkqikglbr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gcrdnohmj.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gwwwvizwi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gqlwhwdzi.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/goiljqdqw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gxpgpqwln.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gvxhukmpn.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gfozwhgkq.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gmjobebmo.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gyfsbzvks.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/grmdakbfp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gediwjrhz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gfhsdpxdh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gpzoshqma.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gdimyunyu.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gjlrxmyiz.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gpsdkxxhy.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/goarsqlhu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gvyaedfcl.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gtuwuteep.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gbjhqiqyo.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gekjhfmei.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/guhibkijt.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/ghykccomf.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gqzmhtzpf.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gwwqzqlzu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gkmrenbgr.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/girowywuy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gcfaxteya.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gjzjvoziy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gvdygehvg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gwvwqagwo.sHtML


<!-- 参考信息 -->