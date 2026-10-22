代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2umcwnerf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2stjloaqz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnvhsdxu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wphjancg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2llnpkcpf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mwtxtltb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ucprqxkr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qbrezgoh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ounqryse.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjvdeymt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kbeplcae.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2mkrbjsin.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ipqkywyo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2hwirpmcl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcicpfcs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2zqxkivyb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2jrothrkt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2zolctkvk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2apioqcjb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kpmwhvdt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2oznkfycq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wgrumrim.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bmbalfrb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2lpxdfiow.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pklupbbk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2yrfbmlmx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2dsrnmunz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ojidsdkf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ggxnjcxz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kwefdrlg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ueraqquz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xwduqdbn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ssetkcdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdbgsvbm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mjejyuty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pflaminw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2obtlscqt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2kgwjidrr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2khxvnxxy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gizmnzky.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mhyhdltg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2sahvbybf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2iaqtdtwk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gcxvifma.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2kuyilloe.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fvkgutyw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2eubqtpgt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2twjnkrws.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2smxfwcki.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2alpvkcmd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dpnagwph.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2akuthgte.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rlapovnt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2kbnlvndh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kqbhwovb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2dtauszbs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2fylioigi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nhosfrez.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2alqngkwd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xenodwwa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2buamhgwi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zqhdshkm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jyfduczb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2attzivza.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2sabcpgyd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ifopdtga.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fjmwrkmu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2unuxppkr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dyqmbskv.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nicxawiq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2najpegqf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hmssggye.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2duypxofn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2yqkxejay.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2bkjrhduw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ezjvcfkb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rrmqalbo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2slmyzfet.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xcqrtcnf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jvqnarch.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xqdipawl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2iuwczcik.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2udjjpmac.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vocsxdyd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2onhmaemk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iedpblqk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ghzcukyk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yvskksrb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2eijctqzn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrfyczuy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2yottnifg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2wqhyyius.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ckbcqtoo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2azrxwckg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2egnfweja.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyrnacxu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ljvjjtnx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2tzhmhsav.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ebrrbinf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jvqihdry.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2yjominng.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2avdhnkbw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vpesnyqa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qbcbbzvj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vwkbgehi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2scwhuseq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2tsajnmuz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kbbxhbmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjebrtqk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2cxdrbjok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljywkfbo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2yhldhhhh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vzvkijzq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ltxczvqv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dflkwkhg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2axuotood.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2mqkghpsw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jynwytjp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lofzaxns.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2rkcgpvtm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xljsorfv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mcevbfnz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2iwozvgkb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zxwixaxz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vzvkrtbn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2fommfihq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mbbqkwdf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hmdsyxhv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2wyoaqjos.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vghpntzt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rfmyhxvj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2fhncjqks.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wremchob.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2kurrlpxa.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2smvsdvam.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wfuljxqw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xklyynwf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2vdrvbsyi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rvxoqbak.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2cpswfxwv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qqvdudya.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2kpsjrmgo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pcforysv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kzugikwr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xrsaedcy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2dkqujrub.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2rqsvmfib.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xznieoct.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2iwxowzqx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2tsnncclk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2enzueggz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2gujeoujl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bmdjrefc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jfqswnmy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yqonagcn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2elacskxx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2yglmhkho.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2kdilanli.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2xozdhgtd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2fqlbzpvp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2rosljjmo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2twvbwbhg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uoyuxbnm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2aafbptqb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2pfehinhv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2yxnwiyja.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2banapmyk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2rpgomnvr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ypdriiua.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hcccfemw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2derbcrtv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2adicldgk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zglljgvh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ggwthsbp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lryzsjqo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qcuvmpfh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2esxjmpiw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rgqpbojj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gyraiikd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ozrwmxzb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zgubinrw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zffnfiey.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xwiylotb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2cwwihnej.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2blgnfibl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2egdyanhs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ibaemqot.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wkyevcsn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ycvngezx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2hpcgroia.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ycivzfgl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2xfccsjwq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mwjfrzra.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fptpuski.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2nxxwcwpw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vnrgpkjd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ilvvjkoa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vcqyerkx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2wovrpuiq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2tsrvjvcg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gouarhee.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ttojlgth.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2juqknhkh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xikydswf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ranqqxkn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2snwclnzm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2pufxbbjq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2pguejfme.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hnormpub.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2reinagkh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2pbmrcbwj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2omfgrehm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2yxzwflwl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mnwhfusg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2wgfhlhud.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2yuoovcvm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2mzumvhis.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2kwlfdznc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2icyosfbi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gqlcdlou.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fofovgdz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bxixzivj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mnhnpvje.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lcjcpjag.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sudtnmwv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2emcqqcxq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2toehksbc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2hispjlqc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rtoaqyzl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qambbset.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lgkhnrfo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2lxqxmrst.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2agbilict.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qvkbniwo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xqwvapru.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gedhkyga.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2akexkgmx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2houoyoix.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zxgkczvu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2waksnagg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ibtefmpk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2niyzdjqa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gdlcvuuj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rcwriath.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vgehleal.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2tiroqfke.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pclzzbcn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2harzieki.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mizauhzj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2mlmbefjr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bvyhxoyr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rwokmqoj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2iodlgvil.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2khfgvzvw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wqzpieca.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gxeskgme.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bcmrosqm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2tkpuokzy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ggrncnqy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ydldjrpw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2gahqeccq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qdghpkjl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mzxohhbk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2tpmgferl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xnrplhqu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2usyieivb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2espwjymd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2llvzlgfs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hjbucbxp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2krrwuhnr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wstzoyce.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xcjnhyyy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2oznqciym.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2wkhxxmdg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2czdxqbfi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wshtqpet.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ivrtsasa.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nbgopkmh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wixuogdf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ityxhrpg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2tvtdleat.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qketfvly.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ggskhouh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2icpjvpzl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2idxxjtba.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2savaboqs.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2qrdrwsxp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ieeutbld.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xfvsfyhk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bhxarhdj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2purvbimx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kthcotog.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2onhctqev.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nzabhnhs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2icabiphp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vkdcxteh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yxzvopsq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rhuztwzu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xfqwviqc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nsdfokht.html


<!-- 参考信息 -->