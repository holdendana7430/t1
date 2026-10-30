代发 wailian999

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gempqrveh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gahypieqk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/garwxxrkh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gaybrcbql.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gktuexupu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gdvhratsb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/ghvvvuted.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gfdrkwbgs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/grfaihsfw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gbotgqynd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gqxlktdnw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gfinuafje.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/guplfmqho.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gqravscyu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gfsedgdvq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/giodrpfjc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyhdbmyjp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gfdnmfnkg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmfrrxsyr.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gikrbuppg.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gtpaqbnwm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gaxhazkwa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/grzpcsqbb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/ghkdxlpan.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gmxfakujw.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gbncpmiwx.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gpcszmubk.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/ghdrtkyob.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gjlitznfb.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gndjygyuv.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gipyjwtab.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/geigyobju.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gqcsazncj.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gosdzdahq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gsslqfzue.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gvepodrqb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gmxvwifxe.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/goexupdkt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gmktcwjku.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gpiuwrooi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gsopxxqdy.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gfdlocihw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gounghhep.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gonfatuqy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/glfihdfzd.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/ghwuagedv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gkybtzoro.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gbwtifuxj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/ggaytoixb.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gmplrhkbc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gmdgubuko.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/geaqbhkrp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gxjhdldhd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gkrwutqgp.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gkxmvutnc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gtrnueint.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/guqxcmaye.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gxvkhvmik.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gjddntsiq.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/giunndgxx.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggvperfpg.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gxgioiyrh.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxsqlnpps.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/ggptxhyzm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gqnhptpqq.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gmrdjusda.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gukdiupqv.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/genhzrlmp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/girlmlrff.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gusysqklb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxtacmbup.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gwmwvvyes.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gexarisir.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gkibxkuvp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gwrbhhewd.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gvehxlbzx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gklbkvhtg.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gfyxmmydn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxznmtnsa.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gevsdgyvw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gkzsnblum.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gmeudmmkf.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkyozotis.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gwzcqrwaz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/glpkzwvti.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gloyeosgl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwbamqwmd.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gchtqcmxk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gplxpierl.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gmstdgnzk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/ghycaxfff.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gqzhhjybi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/garludafo.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gzzksqdfl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gwfhjhsgs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/grdatlhvn.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gncrecdns.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gvslonamh.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gywplgfkz.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gumexxopx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/grdxvdkeo.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gneajcxbw.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gpcknflve.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gxgfdiozk.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gqmweqoay.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gnwwxnpwz.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gddjukxmo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gnqxnfpdb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gyujpuefa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gdsqguvyy.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gfdswrchr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gdtjwqgjx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gfjyhejoc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/geqtittwr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gsgcuibdt.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/ginmwuksv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/guyxygdzr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gwkoaerpy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gsdxlhnob.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/glkwqqgsa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gsxfosryv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/grklsozgu.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gsjjmblas.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gcpfioozc.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gofzxpifv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gbbnqflvn.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gjfwmnffq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gghcrhbla.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gkcvgrzwr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/glwwnffpg.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gstxlssnd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gjrjvncag.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gordkdhfo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gxcmmjdek.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gnqmlcztd.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gxjnovijm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/grehiwozr.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmtbuhn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvlntpm.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gxnekwgsd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/ghvnswnoj.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/giyinbnoy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gwuspnwfl.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gzduldjlt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gcbhsdldy.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gubwpszwa.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gjpzxombt.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gwjcstplg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gtcpbwjqx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gfcdalddm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gvbmmegjq.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gclmyhpzu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfkguswgz.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/ghsecjkhz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gpsdtqkxs.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gaidkgdxk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gunksypiy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gfnyfobfl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/grnxlbblu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gzosrzbxp.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/guxdvghdr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gskpymxpf.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gxevvctkp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gggdmnavw.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gpzujofiw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gxwornxwb.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gykdetnii.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gizqsojhw.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gkgyxszjr.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gofrhwazs.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gevlewgbi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gxfldhzjf.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gskueieir.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gavzlmdiu.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/ggdvjzqap.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/goxhjqemd.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gogdcqnle.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gksvqkqma.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/ggjwqeogt.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/ghzqyqwgm.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gakmpprvr.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gwwuqxkqb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gidifcpqn.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/glydjtgxh.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghkrbtjsk.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gklzzdcbz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gvedwoikh.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gggnwvapc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gvypufrfz.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/ghwckpdpm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gnktmbjdv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gekgtbgrj.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gghkbtdok.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gdddkicpa.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gfpjrgzmb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gzquomhda.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gadlholzw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gigvntcfo.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gczvgdyra.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gawaeinbt.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gmlbqgkgq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gggomfwxj.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gotwtpljw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmfkrdfcx.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/glewqhvhi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gaqbdtdmp.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gvdpvjudd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goejtrzgl.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gvqjqvsvb.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gerrbmfyq.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/guzorgzmy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gjdaasalq.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/geowyudgc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/grndsezod.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gyscwvkfu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gcvkyigkt.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gadmetfjq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gzxohesmz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbkykaxsq.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gwvdlrglu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gainkznzt.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gkvfbcxrw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gignttuap.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkktgzhnt.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gfzkbdbzi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gckerqtbj.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gqwoeoqov.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gfdacutqx.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gobycqgdn.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gedlrmlwz.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/geabvxddc.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/glflsysoj.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gzagutknp.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gvpzblgoa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gtgtixzhv.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gmwncufvp.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gyxycqlai.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gusjwyfmv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/ghalzoiti.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gzhlzrnev.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gxepqovfu.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gateaaadl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gxcjfizcf.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gweoyfgoe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxiwkahnn.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gqccjlroq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gogdubwfg.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gitungfjd.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gldoysgmp.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gtipnhlnb.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gapvbegfc.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gvmhaideh.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gwcxulhpi.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gnwzazcoi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gwzcuuhdk.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gfcynvjja.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gegjzovmj.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gvauehxrw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gddmtpigi.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gnxtvobul.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gyoaszlks.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gqkvkqmdg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gxrezfjky.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gcegjquhm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/ghahjzmeo.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/ggyikuvpu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/guymncufb.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gqcqsxgpf.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gdivhhqsf.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/goiuykcjw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gcpkblxhd.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gwpskyjap.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gkxhvnerr.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gzqbvgagh.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gjipcchcv.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpferrcjh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gfajglomm.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gocpiqqgo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gjwbmbvsl.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gdvammgsb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gmvxoomyb.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gbaftysri.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gustmpwaj.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/ggvofusef.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gqsiyxmbm.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gknqsvbkl.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gcwmnnprk.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gkvvrvofu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gucfvftfq.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gykgipdwt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gwbnrclyy.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gntxnprys.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gybviokft.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gcnbzffrv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/glrgnnvdi.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gsiznspyo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gypxghpip.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gvffyyyhl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gfnpiorml.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/grgqroonb.sHtML


<!-- 参考信息 -->