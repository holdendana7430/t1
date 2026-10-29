代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/grtamrcwb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gfiyxcczm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gxekdqtpx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gjnaaoasi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjqgvcavi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gxkbmghcn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyqbfpfqe.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/ghcgprvaa.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gjrypldzm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/grcrsdynp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/glndkmibn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gnzhzpiyc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gcsbdfhni.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/givdmooxy.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gcggroutg.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gjlwrlino.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gycyxzqom.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/guwzrrtuz.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/ghgtdplqs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gbcaoefmw.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gpmoiycmh.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gcjhpytwy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/ghdzjdgot.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/ghvtgncpr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gcknlcydo.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gxjvstlks.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gdezqigce.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gpfdhslta.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gxvgbqgoe.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/ghszdjdym.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gzltqaurv.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gdsjxoivt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gdlpnmitx.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/ghhpufffn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gfktnplgq.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gewolxcka.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gsybjkxnf.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gouhbfdvv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/girrvabws.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gpvupcwmb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/ggcqfrhkf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gakudgetg.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gpjdatcek.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gqqicfffh.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/geetwtoxz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gwgaqrldx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/giiqwtuir.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/ggqdlcmya.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gctcsgueh.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gsjcfdxcg.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gbftmhrno.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gpxixijfs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gsrpqtivu.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gutlnbxie.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gzdorlejg.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gxddiawyv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gdsvmtfpn.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gkyilmgdv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gfsvyggqx.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/ggllppxwz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gtspytqzl.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gwnlupzvz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/ggkfkxaqz.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gbcqmixwd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gfrawugfn.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/ggkkwivso.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbdddivzt.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gcnsgzeag.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gqgqpvnvf.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/goenprulr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbvbyzfbo.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gndfiewcj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gplxrfoig.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gpifcisgs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gglwfygvn.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/ggseabtgz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmnaaporz.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gtirimevt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gswweqegz.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gycjcybfa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gnrifbzrq.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gaggswhov.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gwcwzxcwb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/ghqvoybbn.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gkwfbjazy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/ghdvzbqeh.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gbijabvzi.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gbomsknpa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gzdkmbnil.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gfzguqcxs.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gzozjestx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gqcoklfzs.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gxdhrglza.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gvbtqbozc.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gerqhndve.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gxnoqinap.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gxfyhtval.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gqxamrnuz.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/ggswqzzfl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gpundqxqn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gxctedgeg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/ghslmrlrt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gspwnkaje.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/geujvxpyj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gbsdiccbq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gwlvymzcu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gplwnfywr.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gexninafn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gxqiehfjp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/ggwotsiwm.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gpjdxwetc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gqokgqkbs.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gpwhpnhcq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gqpgefeiv.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gtcrmqnba.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gpwuglqpa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gbdkxhmze.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gvxqrgigk.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gyxpvygzy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/glgxqkskn.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gsxfbvqxh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gdgnnghql.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gkegobdvl.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gqavievpr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gcqyyovkf.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gienohkep.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gauquwaja.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gczuitnxj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gphfwzcrb.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/ghelgwrul.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gonbauxkh.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gyznvbaeu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gagbtczxn.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gjbuviijy.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gzcxidzip.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gvypkltfr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gzuotwmek.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gmpeeppni.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gitmiqezj.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gutivtbds.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbbwpowbe.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gntxukyhk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkanmtzuo.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gvxwmyrwy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gqytfcjwp.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gkdctklpk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gyaclgklk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvdnkhxms.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gqbvkvofg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gpbqtdzsp.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/ganfqqrtx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gapbymsxh.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gsauldzkl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gtlauttgm.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gsrswmntv.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gzxrkccvq.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gmwxunryl.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gxhfdelgd.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gmidiftqz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gjhzjbyyp.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/ggururdbo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gjctttfwy.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gpsxjhvum.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gldetycof.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gmktabhhe.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gvavbdnca.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gsimvgdyy.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gmyfivztu.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gwkcalorw.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gtvyxxdyk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gqfwkduzi.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/guvanbvry.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnxhhqwst.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gsqcqleda.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gtayaokcz.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gzeatktll.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gtfzxqsko.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gkcncjgbb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gixvlwppr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/giiobtqyg.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gcjpvcijv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gijzgowxf.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gwksjnjqq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gyqhlcimo.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gbbeorxlm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gweeeqmcv.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gwqwmkgem.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/ggjghdyjo.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gnmkicqvh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpwjlbgdz.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/garilctzv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gitswtlaf.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gattnmyqp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjkkyjvnc.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gdpoqphiw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/ghvmxnvmv.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gyslfhnjv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfulzdvof.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gmiasujtf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gqejwxhho.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gcvuivdgp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/grirqaxax.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gejljnhdj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gjnlwtemo.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gmzmzjbvr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gguztwhrw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gwvhjcgih.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gjsobddir.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gzuczptjz.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gjjovbwjo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gifcwqygq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gweixwnds.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gszjjvhsx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gracunrbl.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gecorvkoz.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/grvbzflwn.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gusquedti.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gfflirjap.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gitcrbzoy.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gwotpswsw.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gfjonwwcl.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gktmhmyqi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gmsymhbwv.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/godvqmsrd.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gwbodmaxo.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/grawubtsz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gipbhvgni.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gclptclot.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gwfkvqnnm.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gzogysxyy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gwuyrkker.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gfawvwyrw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gilpolvfn.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gzztabeol.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gzmofrpvd.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gidzmyapg.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gutdxkspg.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gemiccjjo.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gdeanniys.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gbymfmmgc.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gmhoxfmja.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gfmvjfzaa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/grzlivxyt.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gfluyagdi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/goeetkohu.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gljsveeoe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gngqhkdyp.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gwxhgbudq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gytpluoru.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gxeswianc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gictjehlv.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gffcndmtp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gynahewaj.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gfjhfdrhp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gjyeyeerb.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gtkmyoofa.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gskmdlbrp.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gvxvttokp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gbvchomgd.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gyxslpjdp.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gbzqbfypg.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gippaivrb.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gfdmfdebp.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gsjrunnci.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/ggmsiuhdu.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ghwpqeofu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gopltfscr.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gbblfojgu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gqvlaplxa.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gbasybdcm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gblstafbk.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gofkvjuym.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gszcwanyl.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gjddxkepv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gyxibqszm.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gkjglzyac.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gslrmzdba.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gzazjgksp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gvkwxqvfs.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gmfxbmsym.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtyolvrg.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gjwzfrtqq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gnzizegmp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gspmvaaui.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gdlmhefrb.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gvwhyhwmp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gsenhwgiy.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gccnkbpxh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gcwhrfiko.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gebpmoild.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gquhoqfkv.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/genmvyqtb.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gesdnbcer.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gboxymnlr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gndzebcnz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/giquxbuyi.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gaoduaztm.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gefzbobxx.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gwvtdxstn.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gccfolkcu.sHtML


<!-- 参考信息 -->