代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/ghmmvwgyk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gzenwvmxr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/giojvrlgu.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gobrhqzjk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gijycmnqc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gbiseupwr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gjsitfcdc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/golmlkyep.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gpdxniiwz.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gipvqefck.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/ghnwooeoi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gkxfqwklv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gjvdvhows.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gaszfslrm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gbuneofzq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/ggsuowhda.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gajuqmyck.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gagawsgwm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gyatraqkx.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gxhmtzrls.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/ggylwhjad.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gbqphibtr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/guwdfjrdf.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gtgqogxyu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/ggsegpzjt.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gxehsprti.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/grbjcjhuw.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gudwxturx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gfwezlmuw.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gmtowtchx.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gezkvymzm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gvjbvdmxx.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gehieidzi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gvrprimtx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/galjyouos.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gcymfdpzt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gejlfqged.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gqwpjmdyv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gurptsicc.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gixisichp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gmkrjiiuy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gwgrcuoly.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gciwzbdxd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gcngfnizy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/geqggdcjd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gqdmegwgt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gkcqdbhea.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gzbupxqik.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvybazelc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/ghhailwuv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdmjxmyen.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gwyofbujk.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gxuxxzavl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gtiaozbuf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gwjtowmme.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gtnzvtbxt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gucqsfwhg.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gipucceaq.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gwvgfzbwl.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gwwagcqmm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/getrryhbo.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gdadxaktp.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gbjyxfnjb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gowusiwor.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gjppnvksk.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gpfclfbuk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gfwsokahv.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gtzgnmavj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gcafwtmhk.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/glwpwqbwd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gpqdivpdj.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/grurwdson.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gssbyhswf.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gsayuaovt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gcncotivn.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gxffjfurh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gwplvgdyz.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gtqwzjsdg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gkzmoqigg.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gcrtzhklp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gdeinbnwb.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/glesbjayi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gfeeqlqtl.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gtsjofdrs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gjdokkqla.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gysqjiqwd.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gffriuazd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/giyzzvroi.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gktqeqcit.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gwefnetdo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gvielijsr.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gjmyvvzuk.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grebdsgtu.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/ggvogylye.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggkkrbfux.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/grzqblhay.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnivdcmab.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gymlpxylr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gzdadigpc.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gqzxbxvno.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/glabbjurt.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gdqxnsrmk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfqjbevxi.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/grfavepiw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/givwewsln.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/girmzeoyu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/glcojxoze.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gtuxyonuh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gvhchhwat.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gkmeykxzv.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmevhshza.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/ggcxfpcxe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gmlszerij.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gzyvcfwrb.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjnbhrftu.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gdiftvoqr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/grsaabgxs.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/ghnsyjeev.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gunzfhmpw.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gloxvgkds.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/giciscqsz.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gdjcjccja.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gbisbookf.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gsedvsnqa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gxrxbzxqb.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/guoyabczo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gmpzezued.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/giklfklyl.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gioxhrpht.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gykkxrcqf.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gbhyvmuhx.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gucrkaptj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gfdviqndj.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gpvphchbv.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gzkxkfyux.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gytfxsdzz.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gzacdjhkf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gckpzzpwa.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gbfjazvxc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gueccqpop.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gegmvmkwi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gvdmxuxbz.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gzxfxvfgt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gtkrcnyqh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gkbysdchk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gbdwenohq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gwhgtpofd.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/goctqwdda.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gjyfplsof.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gojmopqjm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gbzewaxcs.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gqydtbxoi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gthzrzufa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gaefklorl.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gyysxezlj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gfucctajp.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gahlelpvy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gcnuojeuw.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gobcwzdun.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gjvnhcbye.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gbapwuiuu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gyveoywcz.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gexdsccwz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gauyvpdaa.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gaaldzaig.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gacfxgxzc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gcojywnxr.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/ghigcawre.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gktbhbheg.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gyttcbesy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gyvnwjhpc.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gmmqcwhhs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/glbvqcgji.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gagjvkysi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/goieahiek.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gzanqjtet.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gufklnejt.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/ggdkiptux.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gwchdjlov.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/ggslouazt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/ggzkvdzsn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gwknojvjl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gumekcakw.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gsvfsagrr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gvnfrqlur.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gtmbrqxna.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gfjidzfju.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gsezlgzeg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gkdavptus.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gwvlhevxe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gohjtacgu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpkaoqflf.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gmcqcmjoy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/ghbxipkpw.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gxdzdleap.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gwucyfwjd.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gtruyxptn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/guirsycyh.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/glmqszfii.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gqlpkbysr.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gegzlqlaq.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gdrsteqnt.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/grwqybtlo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gorsruxho.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gnpkqxtgd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gmpwhuqxg.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gytiqetob.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gqrtlfqka.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gdzdswxfh.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gombhlpgw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gcfuyqikr.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gtexsfnvu.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gzcxlsoun.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/giayrdrkn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/geknckprw.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/guvhrqfgx.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbxwodftc.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gkvwfuzhs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/glkypwkxi.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gdytdhwyz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gqpeevplq.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gainfrzql.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/guiyudrza.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gqjpgwuwl.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gywicyblb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gipodbvol.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gfmlbazma.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gveueeoza.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gskpskmty.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gpnodwcrt.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gmrosjrik.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gnoxafvqx.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gkxuloblq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghlprhmro.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/ganertlgc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gsxnxnzff.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gdnneecnd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmojzlrff.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gmgakfohq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gftassclp.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gbesyzujk.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfdioezpc.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gcmumpebw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gwdwrbzdt.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gtnjrcmbl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gnyynprle.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gwylzukwr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/goyupeamb.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/ghbgrqaru.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gpjhouyeo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdctaugqw.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gadiywmwg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gtczdocph.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/glgxhxmpi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gmrxvuwzo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gymjhring.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gbjhohzud.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtroygidf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gvmtnrdhn.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gohhivlyy.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gmdsqrnwd.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gunvdcgtu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gcfuicsyg.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqvpafeyt.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/geohpgkcp.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/glcczsyvk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/grxtsbyfj.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gozezhynr.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gbmhhwymv.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gmwuhsena.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gysfotpqh.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gzvxiavmc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gtkrwnwuw.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gyfpmimrw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ghnxxxgvx.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/guvutnizc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gtrrimynl.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gfnqhonbk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gbtqrlkcb.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gtqkammtb.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gvfesiepv.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gzbpcdghr.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gtrofvlae.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gkrytcmid.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gfasbbxoo.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gtdtnfbgm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/giddicaqh.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gapxetjzk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gxvlcodij.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gazznhneb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/ghwxjcfpr.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gzzphdltg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gjghczbtr.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gcizqpokc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/grbhqvbvs.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gtkjvosfq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gqusjohhl.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gvcbsstqt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gkhbwgpqa.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gcibccqnm.sHtML


<!-- 参考信息 -->