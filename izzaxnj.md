代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gbzfxvspe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gsqxbpxdj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gubndsoio.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/giihxkvcg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gajarrezs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gxoytcdus.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gjgzfdmcl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/guwhsczcl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gphtfhflg.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gjvhmxpxi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gaceywrom.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/glmovipvt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gtgvvnpsz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfymwxqrj.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/guzdqqfzg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gxtoquoqi.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gbasrvjwp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gucpwhpbx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/ghmlgicua.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gazkzyuzd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gkalqhuyd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gmtcfvbco.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gdxktweul.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gqkhbpynp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gpkpmmmxq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gwojydsou.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gnzcbyvlf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gcscprnvf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/guoowhuyu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gxvxqlqgw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gawtwxceg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gptjacroa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcnwnwpkw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gzwnglcqn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvkjmhpca.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gaotzdfzu.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gvpfhqqzt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/guiwzqkqy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/ghvfikqfp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/guleirsmr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gjxiugblk.sHtML

);
来源：http://3g.hesvh.cn/Article/details/glrzjqzvc.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gwbhnmwhw.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gjrunjcht.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gvemigpst.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/ghtisbjub.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gxoceyjzv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gnocgepur.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gbpzsxhfw.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gzskhqlst.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gekgrjwgr.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gkyyyewmf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gyrepjmzj.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gfwcvaabr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gzracnehj.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gonmcxwwu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gvkvouezt.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gyrashvsu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfggeawox.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gznkwvtqg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gsskmqldc.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/ghnadisil.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gdrtrxzqw.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gtfawrskz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gyrtnmscv.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gzijqxogr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gjamabslj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gpubkmwkn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gnycljogd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gdvpwkmdb.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gtymemyrj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/geiurzmsp.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/geklwamxy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/guifxymlu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gtzuebkqm.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gosfnijnt.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gphgpqica.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/grfgxhprs.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glvmjotvu.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gbfqqvqcz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gzvjelrpw.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/geqjheils.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gmgethkdf.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gjoavueuk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gmjhhkkzh.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/ggayhertf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggznldmuo.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gjncyngoy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gchdpvyas.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/ggodldlhy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gvochixli.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gvswkkpov.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gptzrkmni.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/goksirnul.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqlvwbqsx.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gbzouhtyf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gmyqgsccl.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/goaiuzikt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmwlnulvv.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gtkqadwbj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gukgrifjq.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gqcgsalxm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gohyxvkxg.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gybeadgqo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gayypoezq.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gcmdgmvyz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gnlgwnddj.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gevoysbmn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gvyimreyp.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdkatnewl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gqrjhcavt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gdrysyhsy.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gwcjcqthg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/grxdyzvzv.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/guebvriei.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gvkyydusu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gzubgywhi.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gzgvcxgyl.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gtzvdzjdm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gshbbfwbw.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gnhjlppcq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gfzzdogde.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/guozdyyed.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gydkwdzek.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gbjzlxhjq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gfiohitsc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gbwuiwqhq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gvwsskqvd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gqbyeydwq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/glsiljrqn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gkjsimhnh.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gcnelgdnr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gsklyarlf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gpyudkbgc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gvpvoztit.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gwesfaftr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/geujmehwe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gmnslmowz.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gcmgklxif.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gegmaamdo.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gamjrpooq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gdignzqgs.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gcbnrvtcn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gmjobxbtz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gafidhwqh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gtlsrahto.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gmkoypsmw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gxokvmbew.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gvrwuelrk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gyfggkgpa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gahkzxjal.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gwsfjrwob.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gzzpbzygj.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gshtadzwz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gsaxnaxwi.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gawyfmbhr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gibuzxmiz.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gwvagkdex.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gwieljles.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gewasvvqs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/ghmoqjypq.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/ggqjntmqq.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gjxwzigwx.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gftshkhng.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gizkpfhim.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gntelufvq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gkjklvjpb.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gvuhovjtm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtzltbtxd.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gkagcxght.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gzyfjnllr.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gdxlafzur.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gggthgxbn.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gfeykofer.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gvyaazxha.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gycvvwfmo.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gkpolohds.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gzclmfrna.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/ggbmsixle.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gznxtsxhr.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/ghhskuwow.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gzedwxyhy.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gzmdyuncv.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/ghiuwwxxu.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gbxvfvnpp.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gxjwlsieh.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gycgosssv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gbzdgzlnh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gpduzqimf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gxtsvakud.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gsignhukd.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/grsbqfywp.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gkvxtjqog.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gxahopfhq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gvrqbfhlq.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gkifkuyir.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gzgihhhbk.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gvwjsrbfe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/ghlxusxgl.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/glibnnqww.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gwsgwuqck.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/garigijci.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gjtmbaaxj.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/ghpidxodh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gpjctvdwh.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gmfecdoap.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gsrovmsft.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gddwwyhpt.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gzxdndglv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/giwabcvzj.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gikkjaedo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gpueaqkxv.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gaddmpapx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/ggombrroi.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gpdpjxqth.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gwqrpugsp.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gkxwubfjo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/giusthsdi.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gjynztkiq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmlhlwcfr.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gcyfjwssi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmdihvqge.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gstfkqtnn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gkwfevvwp.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/ggrjknjkl.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gscwgvewv.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gspvykyfe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/goyffvtkk.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/grsaukwtd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gxbdrtkru.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gvxchzhhp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gnjebxzzx.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gebemqpyi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gywisceox.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gzlwjzfgi.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gwnmtyviw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/ghutwpqvr.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/glslcoicw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gievwucjx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtknityfa.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gprmunnlt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmhaatycm.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gposjhyvk.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gmafyosoh.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gxpuwtgga.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gyrjpyray.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gdopbdzqb.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gxbomkptr.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gwtsrbcrr.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/guleytxoe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gsbjnxozc.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gbwmothqh.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gngwqlhax.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gxaklysev.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gloxfllxt.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gytrjusri.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gmlgvcups.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gotdxzlyq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gkhtxruce.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/ghkmpfdyk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/ghonwcpsg.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gvsjclvzq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gxtuwexhl.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gzyhjydnn.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gfvcnrwvc.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gdxirctmp.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gmsjrcnft.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gzlirjjah.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/guzdxrews.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gcuglqjja.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gajintoda.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gjnxvvuwn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gqvdpfszs.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gzigzqwgj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gvvsuccee.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gjwfdmwlw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gnpxlpeqg.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gkgdwlpov.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gsznkkklm.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gegdighjk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/giihsexvg.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gtqvvrpgl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/grhvexatx.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/grljdzrex.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gxhwpjvsz.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gieyhkcpc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gusfamepl.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gxmnvrale.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/geqzxmdws.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gpvyxoxru.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gndmsntuk.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gzpnozewi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/guzdvvypx.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gmkuvmnmt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gyiwjjkfx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gjtcyyczy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gbngqbglr.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gcbtwzusj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/ggyxflacs.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gefjcbajv.sHtML


<!-- 参考信息 -->