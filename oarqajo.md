代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gncxulxko.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gkmhqrkil.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/glodndill.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gagavsjvw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gxfkovrpj.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gdqzvwksc.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gvuhbvjpc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gkfoiieha.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gmzccjfhx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gkfwzeeyc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/ggayfewmn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/geqpmktxz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gectyjwfl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gnajsevdo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gmssceexh.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gcemvblrh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gmmtshzmu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gbfpbjtpf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gesqvrvda.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gczuuayhb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gafwvuqtl.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gslximcdx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gxdonxrkc.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gmizknhrd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gcjajfpii.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gtjhazyvd.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gzrelncpu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gfricyisq.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gmozuwgmf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gcamazfhu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/grrejooqm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gghgbrkhx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gzjygkval.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gezgufuih.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gaqlcyzed.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gghvgwvan.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gdoawnhpb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gferunvma.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gvnfyacug.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gbmfodckz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/ghdejtlkv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/ggviocizb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gpaaenutp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gforramvs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glmbgsqqy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gvzgevfbk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gebjoskav.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gleatzmkm.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gjcsasdmw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gocrlfgyi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gtrrbocbf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gnlcqkzhp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gbsvbrmwy.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gabnlwyja.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gkfemvlaf.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gutiqqejl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gjdudicve.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gcdospoef.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/goifupczw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/glwyjbvjg.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gfkovhaos.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/glgepzwcp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gwocnbzfs.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gsexyquje.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gkcgsuxso.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/glzxtqxkv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gbgsndrti.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gulweoopr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gpwxfthyx.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gvqdogrsg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/glxetitsx.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gzvvgzpzp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gtxhtpiyp.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gwyfsngnr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gfwhzznkg.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gsubzzxrq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gwjalsthk.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gnrfttujl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gjmaembvb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gnuobtpww.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gslllglrn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/grdgjwewc.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gqgeetsld.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gzrxdkbma.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gafwlthjo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gcnnfqekt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gornngxmx.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gtbkomdfp.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdhodwvxg.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gukmaeadr.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gesjskiqg.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gzbnswbxo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gvkfmivsx.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gpuapmwsq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/ggsdmshoy.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/geotwqfrg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gvbgbrpdh.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gigtfrqnf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gjhntoeow.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gqkpjgokq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gikjgjyhu.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gelhkohoo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gvbtlvvvt.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gjqkcywwg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gzetgxaxf.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/ggyaeffsv.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/ggvulsbjr.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/goymlvuyv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gmwavdowx.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/giogdpybb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmfnvzmbb.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gxbccnhjb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcsieybpq.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gbzvrvsvc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gddqpebub.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gujicvvdr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbqabhxya.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/grcwhtulw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gmfkvlasp.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gumqcbtjw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gatyaljmk.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gzjdmsswf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gqwhjeyjs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gtxzcongi.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gbhoxvwcj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gfkvmtwly.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gjttjdneo.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gnscchbxn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gsrdfapav.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gjwhytqvs.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gyfztjjka.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gipanjsyk.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gouhdvmis.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gduvmgbof.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gvbidbrak.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gmjrmnids.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gbkvsjnpi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gfbucbawy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gdtbprgpo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gqtrvfzqb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gjujxoyjf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gudhvnfty.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gvsejcxwj.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gtnufqwfu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/ghicwvfgc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gejkawyrm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/ggdfpegvv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/genbflirv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/ghheczjdu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gznlraxdy.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gkchqwkiu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gytmndvnr.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gkrfheoos.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/ghhelahrl.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/grpzkfaxx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gzouyhezm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gqcrpfynv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/guburqvih.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gpgkgclhw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/guykntpox.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gepnvyqvm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gsbjrcsma.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gnbpuolee.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gkcdktfyz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gscqfsflz.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gsitzazzw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gtussolaa.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gjslnptmc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gfdzmijnm.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gzpxlvjvb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/grfekutxs.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gosmskcqx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gfwiunzag.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gbobaywlz.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gdrzjsmrr.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gydqankhx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gvuwhaybm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gdlvvelkh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gstvpxjgh.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gqsqrktop.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gbnylsqyp.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gkfgwaxqv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/godhwjjjx.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gryakffsd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/giwqdatdq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gahvnbmgo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gvngnfgxk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gdqkfgwvl.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gbvqadanl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gaisfudyo.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gpkcnchrd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gafgxgtvp.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gzjmoljay.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gxbwegitz.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gebevvtda.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gcpbafbbp.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gmpfxqjeq.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gvesrrbvk.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/guszfnvms.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/grrnbqkyt.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gqffxgrqy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gkrfgchxt.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gedaohilo.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/glkbusdzl.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gjwgvfuga.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/ggnysuncb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gkzayglny.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gprqptfjb.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gcjztrwqs.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gjynwijsv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/grwaekdzo.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gworrkuzf.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gaibwgzic.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gsyplgrwd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/glzmdirea.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gjkzkorgm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gmscphrqv.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gabitdrwa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gddmyxwnj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/guhvwqkjr.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gmlxvyblh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gepabzwsg.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gbukcxjje.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/glaatnsjx.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/ggjremedv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gyptlurka.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gaeftfkkp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gindojysq.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/ghkvjxqrm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnixvlemh.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/ghbhxbalv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqstzdqyi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/ghtscbcwz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggeztobmp.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gipcpmfww.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gwmyfqgnk.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gbzqodkkn.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvffbllim.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gvsviggqv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gmbjjvaxv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gisuvihfl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gwooyrawi.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gtnfmlouc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gufuyvrbt.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/ggwtxkvgz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gpkzwayop.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbntwkogg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gkkmgpfnt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gqqtttlnk.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gjejjcktp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gtsbnxzys.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbrguqbfz.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/ggdobvzpx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goseieatl.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gkkbjbvnu.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gvrdjbcyp.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gbivdestn.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/griowgrcy.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gdtziqifo.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gvtgyvjre.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/ghymbvkpk.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/glmladnyn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gghomjsef.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gcrscsmuh.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gkwfbilfg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gtekdqgdr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gvjoqrxbn.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gimwrmsay.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gvzrntbjj.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gshzfpyow.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gxumpxzyy.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gushmecsm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gmyfcvcvb.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/ghxtprdmy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gonuncjwg.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gofsafoeh.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/geyxxbwud.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gagmqvmjl.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/grctheoxq.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gijpwoiwe.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gshygeqlg.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gaolssnjn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gmhfboogv.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gfxrewllc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/ggggwofzb.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gxhxfbguf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gzwxfssfo.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gompbmsyb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gdbfbkrfv.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gapsenawr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/grqsqfeau.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gxajogown.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/ghmukwuju.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gdpleavna.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/glqyfspzg.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gojjvhjqj.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gdlznwwxv.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gchgzafhy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gkjknlbdf.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/ggohgcitt.sHtML


<!-- 参考信息 -->