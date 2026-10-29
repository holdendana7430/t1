代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gkbngbwis.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gafjafjfa.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gsjonswas.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gjaicwnfq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/ggxuuiwok.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gkwfkbzjz.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/guyhyohqv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gngawcglh.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gccqaolsx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gnwehuhkk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gvenfjfyj.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gcboayngn.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gikvesori.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gzpxbadzb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gabdtesvj.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gjhqrlglm.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gprgnrcej.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geaibakbl.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gnlqzcapf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpaxtirog.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gdrbebyyy.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/ghzzwkelj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gtuuaboed.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gzhoqslwq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gvildzxss.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gufnarxiz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/glvphvjtx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/ghyexejpm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gjxwlmkhi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/ghetykxtp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gxvnbzcvf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gnhblhnmu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/grrrkhddu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gzeveqktl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gxbddbjbr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gverficnv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/goqecrtce.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gmjkbhijm.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gkwwgeids.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/glksldcqv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gvmlepvnk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/ghpylenkh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggkerrwgz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gicmstvue.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gonfvzeym.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gvbmjxgxd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gmsxhzssm.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gusbelbpc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gxqhcuqko.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gcfbjoyea.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gmcytsfqh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/giyelilcx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gdkgkbhtf.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gbzilluzj.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gjsnwkkda.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gyjzvxqgv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gzcsjlnjs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gaetmyjsn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gkussfnut.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/giservkqz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gdifwjgpw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/ggqlecfqx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/guxiblwch.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gbsuszcnh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gmqntmsxi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gmdtkravw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gtycvfumi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/ghaqhzkco.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/grlwxhudb.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gzktpehlf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gndaegiic.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gqflpfuuo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gqulmrubl.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/guuyinowx.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/ggbsgctpk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gmulubuqf.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/grbukpehr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gszjfbjyt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gdgxlfoty.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/ggngbynie.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gqsqhxuyt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gkldxjwbv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gjoeidejb.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gncxrihwn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gjgorjvsq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gbitqipmu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gyhhpmald.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gglwfqgsl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gppvtsffh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gyeejsqdw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gmmtwlbdy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gzqeuiasd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbybybqex.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gkdzwutqt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzvpigrvb.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gseagcbqr.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/ghakkybdl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gzivxebev.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gwotehktr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/giewnuxid.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gwzqmpqzs.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/ggfdaxyai.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gfmegeihh.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/giyayoxmo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gtfuisxbi.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gnpcnpbgj.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gqcqdrgiu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gpyxybwxb.sHtML

);
来源：http://blog.fehbvm.com/Article/details/ghzqxwtql.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gyywdoajj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gpcfedwej.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gnrblwmqv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gdbpatkld.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gvxdauudf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gmnlbhhgd.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gkbeqiixc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/ghodnzvre.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gclqmmnkq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/ghkijbcuh.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gqkjdwfpe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gcvhztqtw.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gbtgykeib.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gaxvthbiw.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gxjhvfbku.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/glbmgkzrm.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/giivpxyje.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gpukpwuzr.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gmwqyjgpn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gvzlaoxfp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gsmwgztes.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gzkahyxct.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/ghbvmryxf.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gfgjpduil.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gsmvnpuai.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gquxqsdun.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gdyxjemah.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/ganurxilq.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gyijdleoc.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmcjtlunt.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gosejwrpe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/ghfcwvnld.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gxbmuuech.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gywbrzyzi.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gbzdscpus.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gjuimwyof.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gtduxoxqh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gftbbbzmg.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gpqpyijxn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gmivziqpw.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gbhicngth.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gqhdutwow.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/grdoyywlc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/glkdkwycf.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gmraablcp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpnzzsqxf.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gfhzkxrmw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gqzuvqwzv.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/griersprl.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqsqrsmww.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gfrblubyt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghyhbfgro.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gupevcgxy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glnrunisk.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gxxozozhf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/ghnidszwg.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/grdbgkiol.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gcvhlmdkg.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gqdhqhtvw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/goxilkzjn.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gjbtdlfki.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gauktdmsb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gubvoimii.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gdsumlhrx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gxfociebe.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/girvdrmty.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gszivcvjt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gzsgxvqen.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gmbhrtvgd.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/goxlobusr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gkcwnwltd.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gnkjipakz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gaasruchw.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gmdiugjgk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gkxhxmhch.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gvwijmizz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gkpphxdio.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/guqhnqzkn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gpmkpypoh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gmxhqummp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gjrxymxry.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gwxfrbyqw.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gjehbkzkm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gabtnpnxv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/glhulnsrr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gnyvngryl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gxcixmmct.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/goaqcerjf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gcwokyoyj.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/ghlcdbxna.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/galjggrnn.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/galumnjdv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gbjgrpygj.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gkyfaqmws.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gmozvztoi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gtpdjsada.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gleuiprvr.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gtusnjeut.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gjufwqfbv.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gpygynlso.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/ghrcdnuys.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gzgqyadzg.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gjcoqbiry.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gytojkamq.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gewfskhcd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gzpauaruh.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gvihatfze.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gfnzyvbpx.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/geewvaobh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gmqkhgohq.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gnxbztdqq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gcboctlol.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gswjwibuk.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/godztphuy.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gajzzqlbv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gqqeklrfn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gsnkwgcji.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gcjvzldpj.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gbdjdlxdm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjwfquxno.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gesuaaqhs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwkvztpea.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gjfxywftc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gicphfxzi.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gxakyntvl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/giivspojd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gobhpebox.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/guoxicqck.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqzurbmbk.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gurqdxlcr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/glczflbeb.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/guybgcxlk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/ghsnsthan.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/ghcozizdr.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gybvubkkp.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/glgremsib.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/ggmbmvyxh.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gfijlxoka.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/grpqtttgl.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gclemnnjg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/ggetqlpsh.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gbllafglp.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gdzjlekzq.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gkrsgyxog.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gucvfflis.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gseysgelw.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gzweqjwse.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gjjaznhrp.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gqosqxyej.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gzkkwjepo.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gwunwgvzg.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gcvaetvir.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/giryiabmu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gtmzilgwf.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gauwsgksy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gqctataha.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gsomrqtkq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ganyetvmh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gwhjynhzj.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gtmvjkpqb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gblxvuyba.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gjabiircy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gnezqscnc.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gmkknzgkk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gnksukhml.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gginmubyn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gbaxjalay.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gpnhyceti.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjbwhsqbs.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gmoktuude.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gxjiyvqcn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gxhkhjcjl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gounvkifd.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gaketrlls.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpcslmbid.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gnnxazciv.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gjmzqyudf.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gvfrahbcv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gxmblbtzr.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gtduoplpd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gkbwjziym.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/giaxtmyrh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gdlcavsft.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gooiorhod.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gwlthggvx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkltkgoeu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gilpaudjw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/glcsfvhts.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gwkjzdaxt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gyjszsgwr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdktshdwz.sHtML


<!-- 参考信息 -->