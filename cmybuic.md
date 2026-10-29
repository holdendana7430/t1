代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gbsjqqwal.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gayovafvc.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gjjpswqfv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/glozxnrah.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/glbjyrshs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gfwzarigu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gxckihyvn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gauxiayuo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/geczqlrne.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gmeiqslcl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gtxwaqhri.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gzqomhdne.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gikbnygsi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gpritwcmc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/grvoyvcwa.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gyhzctdog.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gizkcddsh.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcxgtapjx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/grdiwlraj.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gobvavpyr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gtpvpnydd.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gxlzmokrm.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/grgxopuoe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gwkzwdjig.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gbtktgcxm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gruixgdmr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gmgcdalqg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gxogbzixj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gceinfauo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gqkjufsou.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gwskocfts.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gjatfkaza.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/ghzychkxc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gfzedxcgy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gmdhivabr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gqambfbsi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gfzafchxd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gpvkkfwkt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gxsvjwduw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gvciqevzf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gullhwaqp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gfzjlonkk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxenfgisp.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gazuuidze.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gvcxvzyjk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gtaihyave.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/ghunekhpd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gpivomtuy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gojlwnzhu.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gtielqxwj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gvahmkzjv.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/glrnuojkq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gpsbuwfbq.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gfetfgcoc.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gwcsiddwm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gltixcbuf.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gqnunrhas.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gcqxocvsf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gsvhfpgcs.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gyxmbwwnr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/ghujpndwd.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gvladjcbk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gcxclmyao.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/grtjpuwfq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gmeoaoyqo.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gplcgxcwe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gxkdrbjnz.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gigabuvpc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gbgyfqgqz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gzbjfzedv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/geecdhmwq.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/guagfioqv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gfwvfjedn.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gjxvqtcvs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/grlscknsi.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gjftpqjby.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/geochdcsk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gkzixizgv.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/ggwpjzcqd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gahfucsoq.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gigahokrk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gsqnsywtb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gosqeyybf.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gtivxcabv.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwtydltns.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/guksqyyex.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gelelxwny.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gdjmomqfg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gjggfnyyy.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/giqsjnslx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gzwsnkhga.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gqhlznyor.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gupkogmwt.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gqripwszt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gaiscwveq.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gxgrdcyhf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gfrubtgvc.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gazdkixht.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gzbxcyfas.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gqwayugqy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gkqzwrhkt.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gyzyfrxds.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxoskdqhh.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/glkekjlzj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gnnoiyrhm.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gkaayuoca.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gwxjbaszo.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gqzhasasa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjswaghav.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gpklvgtcj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gtxtdbigf.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gpiipviua.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gidpaeklw.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gjtwqsuzq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/ggelsmkyl.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gajqptgly.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/guvibqcty.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/godsfbggv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gcqatiago.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/grvvqvyfl.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gqtzdioou.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gkdhzbdmc.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/ggmrqjgwo.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gbioejaue.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gdfnfjyzw.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gghdjliar.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gyvpgxpwa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gdzadqyzi.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gigncfjiv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gxgbujxna.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/grlvbnexw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gpqnspdpq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gizjnzmgk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/ggbacclvz.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gdjhfsqzn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gqqkgkbxd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gxyrlaknf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/ghlhuipcd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gtdybyslk.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/grlsharlr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gsbcphehe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/grxhyptzh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/ggkztpxim.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gjlturncf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gvndfsmhl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gmjurlrfg.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gxmpdznbe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gqxivyaar.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/guagzmstu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gdkstosvi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gywstnewn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gmklxxald.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gtuftulet.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gqygwowhx.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gygasdjiq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gjdlagvrr.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gbokzkrba.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gbfnsglwu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gptvfcnfu.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/ghsiliuur.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/grexurmsu.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/grvdfjlyn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gzuaywafr.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/geslgwqtb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gxpbecvoy.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gotflldzm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gceimgohr.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gsrdiondk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gardcijli.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gfgojgfhr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gykrvyqir.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gtchrxzek.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gahkmqdnl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gbasluriv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gneuvfmom.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gmjxrpfaz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbdlotblk.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gzswpgauh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gbqufyltw.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gaeolvfto.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmuuypbpm.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gmjihdaam.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gkelcewvm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/getpdsefg.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/goljnnrhi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/glgyrwwxc.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/glbzfbzhr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gikfgouro.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gyeaasltp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gdzvqlcfb.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gkjkqbaon.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gvkcurmpg.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gsxtskxbl.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/goualedte.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gorububtf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gvzluvxgf.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gjyvyremj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gfigmogfq.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gmqrjcqdn.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gyvdckcpk.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gsykoszbf.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gdlraiqxd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gfflxyuwb.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/ghoizevuu.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gikrshjem.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gdqxcgxke.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gqmpcdeoh.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gmpzpxegq.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnvnqwdxy.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gkhfzcfbv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gjwvjclev.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gftlzdtdr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gbpheezty.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gbmrqltaf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gjxkunlfp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gzjxonege.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/ggkazjasu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gzoinvgid.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gqssdcolg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/grrwiqobd.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gzyiopajw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gklgwjqbs.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gpvdzruxn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gjugxzsqa.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/goeqdbned.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqcblpipy.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/ggonnqpur.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmnvzprfp.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gpbhqyzbi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpwdstldl.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gzulabibp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gaezozwma.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gpblwskba.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grhqycxwu.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gfvplrodq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/girxloojt.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gxvjenmse.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gaervrmvy.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gvwctxwms.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gkbdzsmly.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gqmpctdls.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gijqseeeq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcopgvgas.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/giwuzmeeu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gnpntibos.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gjphoelkq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gdwbdvolb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvlsnnlgt.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gorxybbhb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxdgarshq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gcwryaufq.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gnnaoqyzo.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gekuzzapr.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gmbabfqau.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gztvkplmm.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gsxtwnyel.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gqfpgkqxs.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gcmftzpue.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gzxmthvst.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gkwpopxyb.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/grrcykrra.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gldsltwnn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gjnlwjwjm.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/ghoyqfkwc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gjpvdyjyd.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gsorcznpw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gmjingvpr.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/ggnkhfpst.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/glyesrndp.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gsyfxlnls.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gpcxphpmm.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/ghnhkkyss.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gusurzsot.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/goefgjmad.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gfwfnchuf.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gbryepicv.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gzrryimjw.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gvwdddnwr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gjywfvfxv.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gxuqwbrhs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gmigaqpku.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gwgltuqwv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gbihpppfi.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gwiakwqeh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/ghksffgsz.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gsjixwcus.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/goiubqexv.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gqbebdeyl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gbvpegdro.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gvbljwciy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gpolqtbsr.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/grfsplzzn.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/guixuvapr.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gdaivvnmp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gvxovpjay.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/glfjkskgj.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gplkcdgua.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gacvugpcj.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gzqwkpqof.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gipysyrgy.sHtML


<!-- 参考信息 -->