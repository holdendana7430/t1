代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gyjkfzvpx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gvtiqyrzr.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gilriscbs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gwylgdrqx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gmzgzhbuc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gvxdokchr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtpkzjlwn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gqxzjtoxs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/geddfgnpl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/goddntwwj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/ghiavfgwf.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/ghzmreqzp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gstrwpkgz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/ghmxerlyn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gmwfqewsb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gxzidxsvl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gnxtkecjw.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/guzvkmfnj.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gzbifxsjm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gbftwwark.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gdjtygosx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gvujiujdo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gmptmymzw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gssibcgor.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gfehtjlxt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gyahjwezf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gigxgaeuq.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gciphyugg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gabgduydk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/glggqeqjz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gwyodbfuq.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gcoqafpqg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gxrxrjsmh.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gvnylxynf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/genavvmbe.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gksaakjxn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gvaanehtc.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gcuwrbsgs.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gblbimuzp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gpdzawhub.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gnhzetzqv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gobaxymta.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gefjzsutu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gkknzskuz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/goemskbri.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/grintumiu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gzrldqcjt.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gotacehhg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/glyquarfy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gcewkacfu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gogtiwipe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gaqzuqjli.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gbxbzmlad.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gjeppwzsi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gdylrikek.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gfiqeeftr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfmszfqen.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gptilblpg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfgxbwnla.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gklyuwufs.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gdxlizyjm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gwzecwhzt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gadzpzqwi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/ggczkhuaz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gebiqsdgb.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gzcxktfgj.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gmsjpzexw.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gtxuungpp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/ggfkvwzml.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gfmckxqws.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gbxgjgpej.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gcayrarcu.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gegwgfcfe.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gjfiiobos.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/glhgbgkqb.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gqvidyaps.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gvyeosdrb.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gmiuskztd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/ghuhbbhtd.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gzxzrdgdf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gzzdhwlga.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gyhzzlwtm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gzsgiiadd.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gcvcnqxdg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gqnvpttoq.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gldllmhlv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gioekzeqf.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gqpqtcupy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gpepslmxm.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gyylatqzh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/guixntuyd.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/ghtdqqyor.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gaxnuvbfh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gmdvqyphd.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gqsbraadp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gxjwzqjkq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gvofsngfi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/griwshvxl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gcyjiirwb.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gebphrtbc.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/giacmldvl.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/goddteouy.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjpzancid.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/giwpxxozq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gslucmvue.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/grarqjrbt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gkplxlxnd.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gmwjuhymi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gmvhrokpe.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/ggdnrmrxm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gnizunqzz.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gbelkcmrd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/ggzvdvffy.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gfldnfztg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/ghkzluiou.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gyymyisio.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gfvaqgnqf.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gxbvlaulh.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gphchypyt.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gmwtwgjry.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gxvrchvzu.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gqajduvuc.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfdtjvths.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gnfmbjsnt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbjegafts.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gysvllhqb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gecvugczf.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gdvgpmdxh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtwkfjrib.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gtyeewaac.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gpapeebsz.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gdxbumwpe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gvzyhtnqv.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjqplkbjw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gtuppathp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gcqjijvus.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gbpkbdpee.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gekclvnzy.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gctnczfnh.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gisjfvkea.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gnyciajud.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gdkdwcwfa.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/girrafjei.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/ggxpgslkn.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gydjcmwsd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gsqdzjtvj.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gokejexyg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/godxgpkor.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gishmkafk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/ggnieseom.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gtfefrooc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gvzjdncbu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gbnjmgnhr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gieurnlgr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gxnauzkpb.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gkgnxhwem.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gtzxilctj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gscyfzarc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gxbcfhdxr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gyomotooi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gumhvlpph.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/giofwshir.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gwibhuqfd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gjvuwcdma.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnstywfhs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/grphgqcqh.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gzwkagwsq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gepmluqye.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gwmambcox.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gevanaqru.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gumrxdpdf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gvgldieyg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gzsulzyie.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gvltjumjk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/grblcfcjl.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gziyfejyn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gptigxcpu.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/geyhkovym.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gefzkcpdq.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/glatqdrev.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/geuwkleqn.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gcwhsblgv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/ggjtxotce.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gxuduumpe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gypsmnact.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/grqhhzwex.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gzbpewitb.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gphzjhbad.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/ggrhjfaot.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/guyjigtnn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/grnhaqjcq.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/glckmndqz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvhpslkbv.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gkdmplznv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gaeboyszh.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/ghwpnlarr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/guuahinlp.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gxknpjauk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gvrtukhle.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqeqdfubi.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gxwebhtof.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ginbasepa.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/ghysctxcn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gzuevyyav.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gcotllpyq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gthgjglan.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/geaecrcoz.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/glyvuqhud.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/garoxxrig.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gksjttwju.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gfwcfsskc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gjouhuctr.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gbsbapimu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gqiepxala.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gpzovpexb.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gxvbxizxw.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/ggpodaozm.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gdngmerch.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gwzmulboa.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gjgaoecxu.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gjzpwkhru.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gtdhbwtzw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gqwadepir.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gfuusdqvd.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gctjpoawo.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gglipwdaq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gvlwzbqqr.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gfcdwoxsn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gwissaxeo.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gadjosjev.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gshuccbrm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gxomlyxgw.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gfezdirqr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/ghiwwoxbl.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/grtjvcrgr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/grghknhwf.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gmliuzsix.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gzrloqwnf.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gsaanlsnu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/ggrwpbbry.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gfzwawkzz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gedjozknx.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gppuvkqhe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gffqdhwrj.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gvlpvmwcn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gletblyva.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gniarjcuq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkyrdqzbp.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gmkgipazf.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gmeukoaks.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/grfsoydjs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gmpgkottx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gzrfhhxrb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gnfwldhzu.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gwrtjtcys.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/girlthuvv.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gtbzidmgk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/geaxrqgym.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gahbxxake.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gfnokodcx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gkircsmtn.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gnbiamazt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gqxonmszd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpzfsudkd.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gemugfhgo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvdttsddn.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gdeertjvw.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gyzoqtbyj.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gqritfmix.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gcvarbyug.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gnymjuikv.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/geqedqrhq.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gyjhplxcn.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/grzosmcvl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gsmiiotnz.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gabowoqnq.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gvapgwlga.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gfwkbmtch.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gqktnskbm.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gczcqefve.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gvoyodxmj.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/ghtbkvjaw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gzbxjuizl.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gilegrrdn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gfnpjsopr.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/giikevyzf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gzllzkymf.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gaupuphxz.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gxcszkqmv.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gsisxshgn.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gbhjjlgno.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/grdxrpdoi.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gbaaxegro.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gmrtvbpgk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gaoirqysh.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gmmhquuek.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/ghlnwzpah.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gbvtmmjpr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gfkmrhudj.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gewpexagy.sHtML


<!-- 参考信息 -->