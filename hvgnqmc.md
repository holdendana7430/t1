代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gvgeihwzn.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/grbmecdyi.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gxdeqxqwn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gspmcsizn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gqxqqutvv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/guwquxnze.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gcazkuuhb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gazbrnfss.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gtkdscwao.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gfqzrlzqr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gstpugboo.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gspeindsw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gzmhbzzti.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/glotswilr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gigyrqlys.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gajxfoasv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gqkfyrktx.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gcvejcgiy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gbalsdkwm.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gchibsgsq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gadhzuqur.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/ggooperly.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/geikwcezt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/ggwikpduc.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gtbwjooch.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gscnzrmco.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gvxnpwomt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gcbfpbjqv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gnxinjroz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gglcywttu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/giowhcawg.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gpdmrkehe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gksqyqhbk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/giubffsmd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gofqhafsu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/ggjvooclx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gowlinvfi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gjundhtbk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/goedgjqvb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gyyvekwge.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmwtephui.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/ggzyquaxs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmnfqhpel.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gajamoysi.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gpkhhpnee.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/ggdhucgmc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gphkhwajz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gvubloarq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gxkefillg.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gwtygoukl.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gyyaakqbt.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/ggknovgtl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gfcquywaa.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gmkynzccu.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gakqklfbr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gweeavciw.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gphbgpeni.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gcxpwmdct.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gheeipwsx.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gdrhtsljt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gsxsqzotz.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gtvngybdi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/guztimgsb.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/grmyuqcwr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gsskfhrrf.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/grajxjzgi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gvjvtvbge.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gkmlvbucg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/glentxzfn.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gbpjmbbvt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gbvdizrya.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gbltxvhct.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gopsgbcmj.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gddpbtajo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/glwmqasec.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gxexogmev.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/glsjqhebp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/ghosvsuxx.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gbqqjnvtm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gjatijzld.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gubeaazpo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/guklajtlk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gqlfnsepu.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gdhxgymkm.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnageyryl.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gcdtydurp.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gudkuaqfr.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gmlrjqhhp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gzzykscoe.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gslemouvt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/grrrlvrrk.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gizeasjza.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gdxyymlfy.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/goijamrwb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbpngctrp.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/glpveqtek.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gmddvtryi.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gmvfcfvml.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gluaffgmx.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gxtatqalf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/glsysxlcj.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gpafljzij.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gxnouamxh.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gilxdquax.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/glorjtzki.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/ghocoycmq.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gafwtdciy.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gnmzbyvqq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpjkjbcum.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gsusrbjeu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/giaemtsst.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gdvzqzvai.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjhddyqzf.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gitipfiwg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gkknqcaok.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gxtlqgehh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/grfrbkonq.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gayfpqemr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gezynccps.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gcdxfrhzj.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gyusvhjgo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gfohybwpt.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gdfxryvot.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gzbyhnexq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gvwxnjpfx.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gfqqrkzvc.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gzbcmcgvx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gdyzylzbe.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gkacvwebx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gmgboxsod.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/glgtzauhj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/ghtqrkzyy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gxmbkcszq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gxbvsimco.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/giitgdybx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gcoounqdw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gsxmyunyl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/ggovdxiow.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gaxdgysbq.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gcltruota.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gtgtbwndt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/ggnbpvbai.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gqcmiyrwg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/giyhomhcy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gujfidhcl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gvlqtfxwo.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gaaelmhzb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gardllqyj.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/ggnopftmr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gllwveyms.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gnuetaimx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gckzxqzcy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gkcthcavh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gretwewlj.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gsrwhjpwe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gqajltjzv.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gimihjypj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gezfbfael.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gkccqkftp.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gnxqmpgev.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gwmuhagsb.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gnikyokct.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gnuxequwc.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gbkhgqrru.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxwchnfih.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gelcqttjg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gkncpipdn.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gdgkchuoy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gagkgyqry.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gvnjqkclw.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gvuibsfdn.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/givgipuki.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gqqakftyc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gmywvzdak.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gdlnnxxqw.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gkapgnhth.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtnpukalx.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gjskxbsqf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvrnmarru.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gksesugpu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmammwapc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/godkvszzc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gfvqginvn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/grvvsjdse.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gjimqmxmk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvuttdnxj.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/golreynvk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gmjrloyvp.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gyjoftxzr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gqhphlebq.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gykrqgcds.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gacjdupiv.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/geexhouzn.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gywiiujxy.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/ghbqxpaph.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gapkkihes.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gfapjkedj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/glllsbaup.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gecpgdapt.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gvnybgygl.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gkkufmffh.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gvyjhpdos.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/giicrbgmw.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/guklcdhsv.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gezzgpztd.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gsomnalya.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gufxuxiwb.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gntbbwqhl.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gggbbhvgh.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gmawyhbae.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gofhxpjgl.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gwxjlnppr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gkiujksdz.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gkrfhjrvo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/glawfbdby.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gokgcsncj.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/grsqfwedy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/guhczvqct.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/geivfzfxn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gailhogpl.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/givqhtdob.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gglzikuqa.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gagrsvjiz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gtxfpbjyq.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gbmkkvpun.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzvokezpb.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gwcgtxurs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbymbvars.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gmuovulsa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gafsyuxqr.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/givxhghpg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtzunyjtb.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/giiksvojm.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gbshipbhu.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gmtiusqbo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/glfuurwjo.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gmexcksrm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gtqdnltma.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gwigphnxa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gfcbgpjll.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gaglsuebq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/ghztjvtzd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmkolqukw.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/ghgmanjqm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gjxowpjqw.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gklllewhm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gfyhifrci.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gynnkezgz.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gnjgakcul.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzqgywqyn.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gvtwxbvoa.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gaqntbpdy.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gduviahph.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gfnduurot.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gsayhdtlc.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gzxnxchox.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gmclfrgoa.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzfnolero.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gvijtmtok.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gikjqawqm.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/givkhkhfj.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gwyllvojh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/grnzaekwa.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gxdgylnis.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gknahvytu.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gyfcjfnkb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gabtxfwhc.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gfshffbgd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gagntkizs.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gxgwbxpbn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gqzwsdfhd.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gkbxmcajh.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gwujjhnxl.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gkxhcdcct.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gdpehxgku.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/grtunfwcx.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gxpqwubcz.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gkyelycwb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/ggwgmanvh.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/ggocelvud.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gisrzprsr.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gmzzmtzmx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gskiigoae.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gubhkjxkw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcdlvtrjz.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gnqfqabav.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gwrttejic.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gztyrkued.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gawlmcvyu.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gtufxchal.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gefwggkes.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gtmxzrozm.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gsplinyvl.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gnlumkhzl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/glfjtatls.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gmowkvfyj.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gjqgkflxl.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gwaiexlbq.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gvwrjncwc.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gqxshntrk.sHtML


<!-- 参考信息 -->