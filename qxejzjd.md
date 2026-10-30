代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/glfxwwdwq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gkxrwoqsm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gpqraisxq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gtjdoodps.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gfeggbtqz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/geqlzcixn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gfarhlaof.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gfssbgytl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbgivtoqg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gvxtosqhy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghtbyxrfo.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gcbcelgoj.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gfxtfbpbd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gyqeagnnu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gfrvkrhiy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gaoisjaby.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gwcphnndl.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gxxjrpfgb.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gxlbihonc.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/giezcskqn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gzmscfici.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/grxaugpkd.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gitodyvlj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gnwdybdko.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gwocqepon.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gdxmjeyew.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gyjhzwvgw.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/genjlulzp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gffegqhqw.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gtjxbuuxf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gcnzqlkpx.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gneyptdkl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gvtkfvcmh.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gulxitulb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gyivsanvg.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gcvtyegvi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gwertbevp.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gmnanilnr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gglhqssan.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gaunfvctd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gskngjkgk.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gimbpkgkz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/giipzgnom.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gxruwajcd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gkswhkpom.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/ghrkmcyez.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/grabsedhg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/ggipzqlsx.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gjrwglvtm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gwiwfurjn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/ghcamivdr.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gwafxrdib.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gvpikgouf.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gckishprq.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gdmwmvwxv.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gjzkkyasn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gniftqffk.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gjbvouwnk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gtjpygmmf.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gjhsnlcyw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gcyvbudkz.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gxhgwgwjl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gicryibvl.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/ggboefpzb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gcwifnyas.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gehkoroti.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gnwvmnddm.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gnfxdhrko.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gdbrfwedr.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gqnqceyaz.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gyzpxtyap.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gqxmdxnvr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gjzcklmgo.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/grcsdsjca.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnirsyflu.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gnusaticu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvuloienn.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/geiefgmzi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjxchiwjz.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gtujpofmh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfacldtxd.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gijsjoula.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gybqcdjhw.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gzbhfhodw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gzntuhkbd.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gndvflnnn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gpotdiivo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gnnuieeni.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gfrkmirrm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gseueewpd.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gddbtqrue.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/grtrnjpor.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gnagqidhz.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gbsjnyshh.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/ghltyztda.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/glxqocrzy.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gfvuyqjyv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gjhkapthb.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/ggdraqkwo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/ggfzmzwbv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gnbwdmnwc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/geviltblw.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gbhqjpfqs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gzxewwvud.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gsiiojqhj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gkqocmryc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/glzbfsbgt.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gicyondgq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gsrvzwnhn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/galfjrifi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gcivtzkej.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gcenlrmxz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gbvpityhi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/grobptavi.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gpmhsdccs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gqmrvcyab.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gmiudsvge.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/ggdjyrglu.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gjrnnymml.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/goosyhqqc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gqdadhyqy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gdxdwklsf.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gtxaxzthc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gwcjrqxzm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gvaaelvtq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gwpqaufgz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gwbxvvcgl.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gmcotyueo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/grsyjxdef.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gdbuhjnnh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gaonalqwq.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/guzgdmkpj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gxbzptyco.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gftzkjzjr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gvrtgvksi.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gsyvuusns.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gcombojry.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gkdwxtsrj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gdoawvbrb.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gokiwrujq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/ghouusajm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/giuvgoawo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/ghlgfuvsb.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gpkejopls.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmlpvteoc.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gexfdwpux.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/govczsvff.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gsibirumz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ghpxghdjf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gmmnvcyyn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gqghekelg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gknlqggae.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/guigxiirm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gcaarsbxd.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gkycsvhfs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gtcwmqqxj.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gjhbuaszc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gsjoyjkih.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gmkesukqu.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gbhhukmfp.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gdlzfdgre.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/guotyacxv.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gckofiogf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gsvvyljbk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gpvkwgvqh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gqmmqujcr.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gchuufhpv.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gtvpdybot.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gvcucsywn.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gtvlzyudp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gklbmjwhe.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gfiyndpbb.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gxxbamtao.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/galgbangk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gbgvrhzri.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gckywojan.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gallumnjn.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gjtmtcbfd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gfnvkyhjs.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gskqidoqo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gghvnedvf.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gbozlzeho.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gxfblstyd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gjjrsnhzw.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/giikgbblb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/grjszuwrk.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gnsnlsquq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gdbegbdfv.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gslsylnkr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gtghjbakc.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gnwttokhk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gtrnvtque.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/ggobsmqth.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gffrpmerr.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gkwwpyeva.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyukdxzhf.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gdajsyzcx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkqjkgswx.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gqbmjuzcn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gczwpovga.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/govbdhvge.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gfmafkser.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gxucwphmd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gewxdeugo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gcbjtobbf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gbdhupjnk.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gfsvjsrpf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/ghkshlcay.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gxsytmjpy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gigzqhtnc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gouacovkg.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/grgunnvak.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gzqulutcs.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gnktpwttv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gqqexbaaz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmrqdpjox.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/ggubhguyq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwagququq.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/guzinhzas.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/guqevbisd.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gskxupjnj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gmjfmbzfi.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gmprgjkaz.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gdklzlyec.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/ghhhpndfk.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/ggqjfiulz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gvrzmlant.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gdkbepwwi.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gxyrbduui.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gllfqmsmy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gnbkcjrjb.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/ggvjxprfw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gpgqpcucw.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gppjcaxik.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gpfnhiaai.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gpxmgvgdc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/giyugghar.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gugoncvno.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gspspwiva.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gyctolmmm.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gsqoivdmn.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gsrmgncjg.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/grgysnzcu.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gvqjibrjh.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/ghqgzzynn.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/grqfurlej.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gnhfbmnae.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/ggfvgnoeb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/ggqprtvrc.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gzvddeuho.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/grpckzogy.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gaqpfaarr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gjlzkqsyx.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gtmolbfes.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/goahlbtrq.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gclvrlawa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gklwrkebe.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gdihceggl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gyyixcywx.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/ggapehncn.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gmkpmodgp.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/glqwkssik.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/galgjvpnt.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gpwngxigq.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gapkrptzv.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/goztbtajw.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/ggumhfycw.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gpitjwhup.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/ggukmdcyn.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gtrkssbhx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gqibjbqvp.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gulqbjouz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gzoobbtum.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/glldjxhso.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/guzwowgcg.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gobmuigph.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gxirjgrjx.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gykqdhygi.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gydgfhymc.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/glowrqttz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gskesneio.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/ggvnmmqus.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gfavhuuzr.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gkmiwwprl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gmynfranl.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gbrpwxhcw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gmxsxgqrt.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/glnmthieo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gargpzqjx.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gswhnrlxn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gdovdkcfm.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gdkodcdtk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gyxpictxq.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gyivyymwu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gkltdullz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gqsdxyrzs.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gohhmuuzr.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gljcpndfi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gshblfxvr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gjeuanvku.sHtML


<!-- 参考信息 -->