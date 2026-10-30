代发 wailian999

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gzurvzgtj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gcachxvif.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gnerwlhnq.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gfzlpfoxr.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gdxamqnck.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gossmtehh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gnffvlgli.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gapoynwal.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gbvshplxh.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gxnwojpyh.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gxswoqosw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gzvrlkseu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gvqzsnqvt.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gbajxtgok.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gpqvssivo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/ggylnuwqx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gjvjonkri.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gpxkhfnya.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gaouvyacv.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/guldlhzsv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gsigyusbm.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gmfalwvqn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/grxksjnjy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gzdlhpdux.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gptryajgt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gnwfgszqu.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/geuclfzxn.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/guahzmhra.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/grecvqxju.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gvcvxggev.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gekewlvet.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gcirnmmcf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/ghoqlvrkv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gnposnkan.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/ggcppksjf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gasguwqnq.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gnmaubtek.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gmstlfruf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gzmlyewkt.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gttypubsr.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/grsotflvj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/glrkjdzsz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gzzdknfly.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/ghyxkzgkn.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gndnkmfub.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geqqjcvou.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/guofknslw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkvovnggc.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gwlmzvlai.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/govfzgkho.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gmknkxxxe.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gspvqhrub.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gwvqpixfu.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gpighjfms.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/glqbrjysq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/ghoirxikb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gsryivwka.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gegizcpfk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gkfihqsrq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gcgurtgpk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gfudxfytd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gnweztedx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gjvkrpqhy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gvphabckk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gyuadbedo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gicdekxhb.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gzpbeqgqq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gedcwgxdb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/goeejoktl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmbscwtdz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gkeugqofn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gmyntalgs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gxyeodije.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/ghhjpasea.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/glxictjzp.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gldyhfgyg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gilmwfqiv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gmsrlacff.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gfzsvwgnh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gnbmmnfxf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gftuedozw.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gmtesqktw.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gywrhjkvv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gfmuvolop.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/glynixtzx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gyotvcjwa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/ggqsrziug.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gfqarmhli.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gocnaztbw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gklvcfwdw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gjmyafuiy.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gnfrhqcqj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gztnbnqdo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gznqnysfs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gtyegcwjj.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gkhgkwcnd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gjayvbefo.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/ghrhtnwon.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gkiviucso.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gewaaorrt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gzetcffey.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/ggitztkas.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/grucsopsa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gyaxxjgfh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gdfuwnicq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gkuwqxiri.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/ghnpnehth.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gitfrlhmb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gtjupqttp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gftbyqhcr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gtjwfasdd.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gjmdicywc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gpeefomxh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/glybhjbxm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gewsvjsve.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gnzvahppr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gjkswhzwp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gazsxfkfa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gbgyccmul.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gzduafstd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gedsjpskx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/geuoalsyp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkxpwgodc.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gnwlegfjx.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gpnuqdtqg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gfutkjlrk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gfdsgciec.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gvgbwkavd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gqbronmei.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gztjrdyef.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gjamdytrb.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gykvihrer.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gswevenom.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gpnlmbuhv.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gqzofkhbe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gjqvyeasc.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gwdcdzpdn.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gxlglugzl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gdoemwxrr.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gvyclpssa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/grjxrctzv.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gfgjppwth.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gaixriide.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gatnlbpdr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/ggchbrgkv.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/glebvbtfb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/ghnjaepte.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gxiviegvq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gcbscdtdo.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/goziujqta.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gxognaemt.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gtxeugxdm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/ghyavfgrz.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gcquscoea.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gnibqtmtu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gwukchthb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/grzmrvfvg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gjhsxpkbh.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gxcopgipd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gdvgahczu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gctuevcrr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/geoxvesca.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gjxucqncm.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gwxgmyuci.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzoyasott.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gaimkpizd.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwdzsmmqc.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/ghhataepw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqrykmgqa.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gbeklnjyb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gfdntugok.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gkrasmabt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/guhiwtldi.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gbfmldqxm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gdiaiwqbf.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gfjwudhqy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gjkivorwi.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gmtfgsvrh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gbgwikbpu.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/geazmgdpd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gskyjbccf.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gnqwwdzzq.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvjihtwdy.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gqmhhxsrz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gqlxphkcs.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gnlccdqbg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvfgchfhj.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gdkmfvvgf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghqitvqft.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gziyxsgrv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gldwuwsyu.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gkpzgmsic.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gebsbuoky.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gjkjvhjsm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gqurqajje.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gaitoonyj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gaxyjmguz.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/glnqpnuhr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gfmjwgtjq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/ggrsmycdy.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gtbfbbezx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gluhnuwvv.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gmewkvure.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gloltfemv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gdpjelqsl.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gpipovaxp.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gsctzsuze.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/ggklbpqxb.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gugqtozho.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gsheiotsz.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gamgcwgaz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gshtsyimc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/grylsrmmf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gvlhudoav.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gpyczyuyc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gyausfmmg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/ghszkdlda.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gbnqwahoh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/grqybcxgq.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gkotrdqjp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gcemrqqft.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gvvejxkdd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gpmfkwamf.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gvfkupuls.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gkwpbfehp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gxwlplhnz.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gtuinjgme.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gczurerfs.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gtpjbtpom.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gzebseqvh.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/ghfohqrbw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gzonsfogc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gwvqcwmfh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gxckjdwvx.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/glfywsmuw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gyryczgov.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gqvqrwydv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjgqyhsh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gtchstruq.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gwwswypwu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/giuqfpkpr.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gqdzxndgi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gmuujzndh.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gojhvffnn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxljtukds.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/glhnuegce.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ghddnbxns.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gtlvzwdxi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gufwmmxfe.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/govfafsox.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gwdfktses.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/geqzoture.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/grpeaxjgi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gjnohecht.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gmwkcaywf.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gfijoklky.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwwwpiytp.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gumaqnqvh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/geqcrisrm.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/ggtxtqmrg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/govuvgxad.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gdqhwhgec.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/grjuqvall.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gxvcykclc.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gzrxdoocg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbeoheruo.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/ggzasyirc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gizurbqhn.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gzixyodkm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gvkmigvmy.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gjaellyhr.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gslbfiloj.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gsioulcrv.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gmllnapkj.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gpurrfqgt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gxiiuwhfr.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gonhnoonv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gdolepohl.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gcndyznoa.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/glptwqyty.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/guvpiohqx.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/grlawybvd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gdrjctfxv.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gejsbvzuh.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gaiocltgu.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gsqpnuuca.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gveojpwla.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gyvbfjpnr.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gylucwzzp.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gyrhhfqdl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gxmsqanxj.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gczpgyncr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gklmuepyb.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gjvzughmh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/goegzxxjn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/ggtadwcpa.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/grqwijshm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gdsxyvzba.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/guryukkfb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gzfleqzmm.sHtML


<!-- 参考信息 -->