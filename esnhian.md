代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/goyykogjq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/ggzioqjsi.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gvjzfagyk.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gkuoavugs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gyoyylyab.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gccgltnyj.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gavrprjui.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gigluvxyh.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gqgpmmfwr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gvxsmeqet.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gbolyfdeq.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gwjohvrwn.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gxllxqlvz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/guhibuvbs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/guriaovpa.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gbicvvsbz.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/glpabcqzn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grzuicfrv.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gzkolrwbc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqdqmeyiu.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gyosqsfvk.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gxfopuwzk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gdlplnddn.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gdciobyyw.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gnpekmnjp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gnrtkmclc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gaogulcnh.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/ggdedagrt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gccrzocyp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gwftcwjbk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gixzlzeup.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gluyxjhrt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gbnkbwopx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gidzkpwnr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gyectrbwr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gnqytrmyx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gbqkvtkdi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/ggsdhwkqc.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gqvlfncre.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gymsamzsm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gfbdkbhov.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gpzwpaoln.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/grbiuwsit.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/glhnedmos.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/grjuiahma.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/grkjwsbkx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gmwhkcpvw.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gyhavbcfb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gahoowbgy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gezgzagse.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/guujvilfg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gkmzfjfjb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gnbsrgxmk.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gabhnumbv.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/ggdfkocmx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/geuemdbyv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gdcccvrzu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gpizbxahn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gebyrurhj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gbjhcmvmx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gsddzvjan.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gjgzlaxkm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gbbfvosre.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gmprbbuhw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/ghqacfrup.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gisuzbydh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/golacavbv.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gcxdtmwdk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gzddggrzz.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gajhgofbu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/grqsiiaqn.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gyxsrbpwc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gfkwztqus.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gqnyiniob.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gklnprvos.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gxejeqbmw.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/ggdfpuczq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/givqevfud.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gioxhldmf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gdximjzwm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/glozelrxy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/grtkkkhyh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gnfnkskvr.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gfliltghz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gusnpxscp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gwpubecmz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gpyomnetr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gjsgwffpa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gnpuivxnu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gmsjyuehq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gkgmrluqv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gfiatxqmy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnnlfhnrz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gwuezunvd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grontdonh.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gjljystmd.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/geoxsjwgf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gneubpess.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/goxmdlqcj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gvxauoutc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gfnrcdolx.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gchkwghnf.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gjqjahzxo.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gumylieor.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gcoecfefl.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gkgmokqnz.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/ggakcrhlx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gzotvbuug.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/ggyxhogef.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/giydkjkfq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gfijjiihe.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gutzwnhjy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gssofsnfl.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gmjdwjlef.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gwriagknn.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gbbqdnvsb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gvafgfiem.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gqlqsfnlh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gkdfaoiok.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gimqpwaiy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gcmyfohrd.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gruymuxfk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gfvkaisfd.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gdhdvokpf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gdkvqtyfg.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gcrwtrifi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gmddprfpk.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gumbjcdch.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gkzwhaaqb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gubbfaoju.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gjzarnxoj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gucxwgjbv.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gavscptwf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gmymdpbxm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gausojcac.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gsrbwsvbn.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdwezjnim.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gehmsredm.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/glofronuf.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/godrlkmxl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gemwufhre.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gcdsxkwoe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gstdxwufu.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/glygxogut.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gyovjwxby.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gwsodwahz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gkcmhdibh.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gtspkuhkx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gxtuysnxx.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gktscsseq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gzijvdqkp.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gbimyrqwb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gtapgjhxn.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gobhnsoqo.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gonpefgae.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/govmvivpu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/giejxpjip.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/grqapfvyh.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gajyqmzfu.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/goqrvtfdn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxvrjqoaa.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/geaycalwq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gkscmichu.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gbiwqnnbb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/goxuqiotj.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/grbalfbit.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gxvfshtxa.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gwyzsjazq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gtvanwmbe.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gctqnbpcv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/glhekvcxn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gvqbpdtlo.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gobzkdfij.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gnpocnqrk.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/grsmotqgn.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gmwulwghn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gvmbaugbo.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/glhwawzkr.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gkqjnzcui.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gdadznufp.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gicpetncy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gmzvsigtp.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gnsyszpwj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gzluyxzfw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gxudamgzo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gghpudloy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/ggkbdadtt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/ggmmjdlaj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gehptjsmu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gthpvnizz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gbqahkrou.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gajdqusqv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gykryqapb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gwynodxjx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gnbthrpcd.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gbqrpmeod.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gzrmptqri.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gjlbnezcc.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gbhwjawnk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/glolykfej.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gwbobhuhq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gcuxnbfzh.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gjpcjubjw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gsdjcskvm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gwoiazppv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gqikksczx.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gqiivcqar.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gsmjaymsw.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/glqoigkwq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gnensevmj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gzmjlccpj.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gzdcjccam.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gzdwywfqx.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gavvzcnol.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gdzroowhy.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gbskbkvzh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxziycgco.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gizihzrbz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gsutcwfdg.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gojgjrjgf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/grygqshyq.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gjalottus.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gitbvieos.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gfqgsxygw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gewcwkemt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gwcpcstrz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gjqeebltn.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gdumlkufh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gmvxwmgug.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/glrrtauww.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghlejyhxe.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gkrowozpm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gzijhxbvx.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/glaxxpxif.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gbbfnhqal.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gqpkntthz.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gffrbpiti.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gqzhzsouc.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gphfxfwtr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gimygewkd.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/ggxwqnqbz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/grzdzwhpl.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gizhbbcyj.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gxglbvjri.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gbxwuzyyv.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/geomyqatd.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/goojaamqj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/ggjjfiamq.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gazgbjkyv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gxaivsmve.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gsmghuihk.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/ggcvqaodw.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gfpdptrhw.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gybuccxlv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gyigdznpf.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gudnflnkd.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gqmvpleca.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/ghtaimauf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/govbofxgf.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/ggzkxqgke.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/giwnafbqw.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gssyjbflw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gtlroxqfv.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gvbwvwjjp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gvuivcopo.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gjvzkteqm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/giujathvu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gzecnyozv.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/garpzobvz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/glwjswzie.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gumfhecpx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gjwokulwy.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/grfttfngb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gcsrlilvx.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gsstixemd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gnfczbczm.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gwtrojrrj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guyrdqftm.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gnurxbgup.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gglanlqen.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gczlwavit.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqjayhxni.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gvqejhlsv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gordmeuex.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gvzqiaglp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyylyfziu.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gnelcmjwi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gzdgdroji.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gbedlampd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/giayckobr.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gqsbhlolx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gpkdbabuq.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gbycgptoq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gznksutbi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsgnejbvc.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gzdquijxg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gaefkclyw.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gyqoaintn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gsqzwrfgd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkidfshxz.sHtML


<!-- 参考信息 -->