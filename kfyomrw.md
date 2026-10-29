代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gyutybcnt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gwjiomtcj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gzlohdodl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gfmyvagkb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gcgutbljs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/geszfgwof.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gggxueosm.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gkjuezgtz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gxqowodcc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gcnqywmgc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gmjxvlhxf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gokhfjumq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gzpkuuikr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gpunicwiu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/glqjpbmng.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gvvgjmbhg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxdovjjvb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gmqrthahu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzmgvekzu.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gioxxipyy.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gnqomfkdr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gjewwplww.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gfljqzzio.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gzibutqgd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/guwohlnrm.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gufvabzgn.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gvykphwwm.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gyrlxakwx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gabpydlcn.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/ggmdpuclf.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gbtbcnkec.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gfrrscmyl.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gwscknsym.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gynvvmdcn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gmgqztwyn.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gkldaupxi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gqfuetonf.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/govkpcjct.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gpqkuoazb.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gzbnaspvi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gmrncqent.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gbkfwvdxa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gizuapehd.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gfoheknna.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gtegyvsrj.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gxrqjlajt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gdsoolmma.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gfdvkyhli.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwznjouol.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gfomolwkm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gswxbzcdi.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gpdkovzts.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gowpyvdum.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gpgxzmfnp.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gnjdeczvt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/govddhjym.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/geovvayui.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gbpaflfcc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gjqnnxlxq.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/grgedsxls.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfejbxyol.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gxypkiwcj.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gcpzgboes.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gpnjjbuyy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gvbdgtkgs.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gemthcvns.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/ghxwzzgmy.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gdmjmeris.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gvkyegxyr.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gwnmjyyqq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gimkfloct.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gntvupqvk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gjqrlrypy.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gjddelibi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gzccczunc.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gubbtktxq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gcwqwrgzw.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gnfkelayk.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/goacxiheh.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/glbeatptj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gzatftupr.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gdpjzyjsa.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqnjkqjfn.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gvromiump.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqxuwlhht.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gxbuieuic.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gjaljxaid.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gxbmhatcr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzsnamawh.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gwivgqfqi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gezsaypjf.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gmallvidm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/ghurjhavk.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gtmkemvif.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gbooeirhw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gsbsrtwpp.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gtivvymgt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gxbfuczcx.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gejgslqck.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gxowjczpn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/giygtsakc.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gtbhefbdd.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/ghnqgevre.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gabqdbakl.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gjpebntlx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gzcxjhvuf.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/ghvraiofr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gtmiffjis.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/glzzatnmp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gwqqadlbb.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gydoztiys.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gillowzaj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gqhtlaxro.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gxlbpaqkr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/ggdlarftp.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/grxmdccfc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/ggtzipmmg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gbsxfuupz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/goalbpnas.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gbypkpwbi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gwtssrmnh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gjeprkzao.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/giepaxydc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gmtuksgvm.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gkvofwsrn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gxrjtsusx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/grokcuksb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gaxecvlzk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gjtdmhvtp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gfcqhugxw.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gchilhdvy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gtfsqgpio.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gxwikwbcw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gptzhrzom.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gbvgofbvp.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gmxicvlfd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/geupkjwjq.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gdvivpvho.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gpevlphsy.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gsktbyico.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gppoonvzh.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gwwyqloep.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/geehlhfdd.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gxauqzfft.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gukyajozx.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gdivjztte.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/geymbtrqh.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gvigojykd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gtkdcmotf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/ggdhtcwef.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gnfdzupae.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gmqqrfejr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdjyxqfsu.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gyovxlntj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gkpzmvazk.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/giwhrbbfz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ggqwomkrt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gsepepnmz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gwhonavpa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ggkpvtktm.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gcmetjdjl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gfhulhvzb.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gzlmqzshu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gcwtltxsf.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gsejtmwek.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gmdgftvbs.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gefjhikpr.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gaqivmshl.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gpxozpame.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gdfbymbnr.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gabfutzuq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gddhnnviu.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gjkjmnhmm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gobyidbaf.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/girumyvrb.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/giwtmeuxn.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gaurybysr.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gepclsifu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gxasndkoj.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gegnkdyrm.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/ggmnouugw.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gkgfuuhwm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gjdvzqrnj.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gjtexvpnm.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gudgyklug.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gdxffzkuh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gsigljzja.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gehprgklr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gcsphbpwc.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gylzawzuh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gsudmulad.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/ggmuslbou.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gvllkxriz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gjvqhckzm.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gapzvugtq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gwafpcogc.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gtczwdekd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gnwedqmxj.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/ghcfnpskd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gqbktcegn.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/ghxtqupxr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/giuiizaoj.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gnpkryjqq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gutexmodj.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/giopirynt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gadtyhzed.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gzlrogzui.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvutbcohn.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gwqrzfhsb.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzcpjezio.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gwxfsydfh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gpxhvnjef.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gqggtwdtf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gquhawdpa.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/glejungqk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gabeyddnj.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gqxsssgot.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gjplcjkpm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtjlhrizz.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/guffurslx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/ggujftnms.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gotzgzjzv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gkijpqlxj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwtaoouhf.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gdgdffdwe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjshcnktx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gdtzszcan.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gvmcseydr.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gjtckjfup.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/guwqqyfoj.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/glmnuxtgf.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gwudexhjv.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gysruujtu.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gjcyexasy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gyrgjicfk.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gwemvdbtf.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/grurmutne.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gepehrkqb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gfbfggzka.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gvhwtykdy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gobhrnsdn.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gpmzbykev.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gmqdyfmdh.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gmmtbjmyg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gnupbsluh.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/ghhznxben.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gwcxeswog.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/glenijpey.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gpxgleipt.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gfgyqcyru.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gmyvqgvvg.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gvhauvisk.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gjqhavuxg.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gnamvtdti.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gdlennxsg.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gxjycapra.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gjtywhzil.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/geqrtmjwe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gcktgjkwr.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gjtcyuzif.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gmgvioguo.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gpcshdyjv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gxquzqhzr.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/grmrsucbu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gtqlgxtdr.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gvoulhwbz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gayyjchbg.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gunmzaens.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/grkudjudx.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gzowoxqvu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gskpllwmm.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gcfrqgdpd.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/glewxnmjs.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/guyfcmfdj.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gpxsftlru.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gmoyptejx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gmmkabgwv.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gwopfbjry.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gpzmevkpg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gtfqjsarc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gczhrzhre.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/ghskdspio.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gdpslkpkb.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gemipjwnm.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gstfejjxa.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gdamtdvts.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gadkmtqzf.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gczqwyiuz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gytollnfi.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gtvfuepjy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gnpanhykg.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gwdhejzks.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gedembmyu.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/ghxqaejrm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gtfpadxvj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gsijidbvk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gajfpvhmb.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gxtimylgp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gkimbmagf.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gjnnbabnd.sHtML


<!-- 参考信息 -->