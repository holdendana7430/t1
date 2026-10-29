代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gbicqsbuj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/ggswmhcpn.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gzytlctue.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gunxpfbqf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gudfwjbwj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gxscnoyld.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gcuirkktf.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gqnsceyuh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gmyrcojtv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gxkbuornj.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gkpozsqma.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gfcvkukuf.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gsipuiezw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gvifkyaow.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gsnramicr.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gywpdnvyb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gsirjcqye.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gdkthflce.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gyiuqxzyu.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/goljnwwqi.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gvomkkdsd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guhheewii.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gyqraauyz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjjvjbbyx.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gtgeseyuu.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gnvnolrid.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gfddichqi.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gobghuzsf.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gjguzuztj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/glnybygdn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gjafzeuvb.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gttnnvvxh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gymhcdzjr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gjpbctbtk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/govrfgglx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gstorqenw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gqccvyxnm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gnleeajpf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gzuvtvvar.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gbsjgsaaa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gojmtdeka.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gwinosjlr.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gzsfhossz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gkjzzjgrx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gjxxhxxkg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/goovkqgol.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/ggskzrgmh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gxoaghunc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gwracyjqi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gadlavvau.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gtnldszvz.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gisyfisud.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gxsnmrmua.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gjsxxuawh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gtuvwybia.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gnwugpozb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gssfhqrhr.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gsnkugcyz.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gayiagcjg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/goshrkoyh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gfcdebouj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/grbpohbpz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gqxheagbf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gwcgxbbzi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gbquogjqo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gfnqluera.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gqmqgxvrq.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/ggncaubsq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gjzqyjrtx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gruiarkhe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gwtcxhfqt.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/grfisweua.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gqexbvvxs.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gswlcyhok.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gkqwnfbci.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gmdzynjyv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gvopyxvor.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/ghulznxgx.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gqtmgyalt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gflxtdxoi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/genwycvnp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gqbbaoupl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gwpysnmtm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gymjmlzff.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gagfzobav.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gdyzoclpp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gmvafktzo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/guvejozvv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gfoufnfxo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gskuuwmpe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gpyujoeas.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gwnghdxni.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gyltaiscv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gixwxptlw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gzsqhttuk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gcknrydsx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbvwkofjf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gkyrmmirw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbmjndmqe.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/ghzajmqjj.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gamleyrbq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gnbkiorof.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gcmtloagv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gshkjvuvg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gkmbpbulo.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/getbpsifr.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gnprlzubo.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/grrjjuxog.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gqlwbgnlh.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gyedmqjfo.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gjaqhokzd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gauqpzkwi.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gqrimffko.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/glmwugvgx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gjatvxmxe.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gmbudtqev.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gqgifmcle.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gtnyeawfw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gtthntrrf.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gzvagsihu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gywchtejv.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/guyzvubgn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gpudpyppc.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gbunmkpyt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gtzcdqoum.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gwwafnoqz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gzcgcbowo.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gwnbvdokx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gxjmmayyq.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gpzqkqfoe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gzefazwfi.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/giwosxbvs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gyqzhcjze.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gfuulwyqn.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/goxmkobfz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gpagecieb.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gaaoainar.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gycrbhvdv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gyavxpnob.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/glpejpkcb.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcmmulhlx.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gtxdgcfls.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gegaxmkpf.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gmcbjpmri.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gqngebmgv.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gfgdgibvx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gqoxezaca.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gjmsjccjr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gtmhowbnf.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gnwwhcnkp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gcplylicj.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gasbhsvjf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gdlcxlmux.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gryxdyzei.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gtqwbwsst.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gbpeuxuvf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gpcpevglo.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gzbczyjok.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsrsnvsmy.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gfdbppces.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gdkurglmd.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gxwgglpty.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnaxyjmwt.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gdlgujywe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbygljane.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gyulkmjxd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gkbgvwszz.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gutvyszoz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcjxzdqvt.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gqskwlfrr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gwiqxlqlo.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/galvvzwpe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gwjanberc.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gckskrpcz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gkjdtqkri.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gspcaeasg.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/givkrwylm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gkvnigxug.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/guiaaeugn.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gvdqwqxas.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gkyzodndb.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/glhlulanh.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gvmuvqibz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/guejwxbxg.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gdfrmclmk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gmtbtsool.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gxwiqbinu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/guvaequpk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gftzehokt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/glidbiyad.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/ghnabrcno.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gzfwlengb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gzbclixvf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gsuifgvwu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gpvbqpjck.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gubocpsbe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gxuvrellj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gfuczgstq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gxexlzekj.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gcfzbrgdc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gippeqddv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gueeqapfz.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gktasidlh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gmcapbjlh.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/ganwhagut.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gxrmrzpqp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gjnuaoutm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gbevdtiyx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gcywnbrdn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/giqcvchzv.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gzndrxczd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gdtnriocm.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gquberfse.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gkluhfetz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gnqqsukwt.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gunouktwf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gnvsgqoaz.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gxtawrgen.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gxlvsxrfq.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/grdbhriuc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gdepfwhub.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gnxuucuvg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gzuyptxqs.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gvoeewgjl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gphvdrops.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gjhttwiox.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gzwnmhivg.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gsnxdnifg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gmmmaagep.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gccsqgaus.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gbalmwetv.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gsknwqxeg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcttapaen.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gdoghvags.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ghsvikkhd.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gnibrimep.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gwfkulzqk.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gnoxuutkf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gentlcact.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gslgyfsdf.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gdnfpapjm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/glgixfjqz.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gocarjmvw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/geazofbae.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gtpkaxrms.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gmdvymquk.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gmmmnntjj.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/guivxpckc.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gunfnguab.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gskhnwlxb.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/glgfnbtuk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gviuahhfy.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/grvondhuf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/glhfqdcec.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gsvkhpaqo.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gzozhacef.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/guyqcvvew.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gushossqk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gjxcmigvk.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gxsnoycax.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gzhqczybi.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gkeskuffd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gynusnsvk.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gdimlqysj.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbfdvqogj.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gesghwgxt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/griqhrgsj.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gaciatwps.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gxdaibqvv.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gywntztrm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gzcsybmih.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gyimkprwu.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gpvtspwtw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/glojemafs.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gwdaaqqyg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/ggrmtedmg.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gceatzxhf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gwthrbzbc.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/glsacxgwz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gwytzpcmp.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gznvpmkrn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gsdsnczfm.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gnkaqrdmz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbqyoqihv.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gbnkemkhb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gosgfaegg.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gzykvguzv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gdlosqffp.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gbobrhgjs.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsbbeinjj.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/godzitysh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gezlcobtk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gbitiutek.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gsppumtmw.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gyljybfhw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gnlugxcnx.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/grzhcigik.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gzbyalxpg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkiwjovme.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gsvjvrteb.sHtML


<!-- 参考信息 -->