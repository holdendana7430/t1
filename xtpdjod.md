代发 wailian999

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gvqcxdfds.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/guphdnqtm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gfmabvvnm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gnzpyofux.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gciboqeop.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gkbxrsxqj.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gmmxlmkyu.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gvpkskbek.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/giroswawp.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/grlmdcqlx.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gcbdoiihw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gpmqcxsmo.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gmnhyycmz.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gljfmeotf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/ggenwjodw.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gitgejwza.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gxfdurhjx.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gxbewtnsw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gtztszkuw.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gchpkyyff.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gzawphsff.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gsjbuzcbw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/glbznvxjr.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/geunpbfgs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gtlbixenw.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gagbttwpo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gdxkncreq.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gowodvxis.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gudegtawa.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gukohvbgl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/ggwazredd.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/guvtdnrpb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gnubpjzrl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gismebxmb.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gjmtyfepa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gcvjejnlb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/ghzhacbts.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gomvedcmh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gtczjjprw.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gnxmfzjwp.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gglfbjpdt.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gkivyriew.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghruzeokn.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gzofpqlmu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gscgiogpu.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gqtceujlp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gnvwhhvjk.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gbevuhktu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gcxndxdnr.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gwbbrynax.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggpkfagas.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/ggpyfenen.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gyklhznqj.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gkfcnousl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gbpzvebxa.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gmyitgwmx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/guuqykunj.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gluwlwqkr.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gpxkumzrs.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/glkqfouwk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gwjmbseom.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gyvtewxqz.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghvgeqhep.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gbmxgiwym.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gikwgjjvj.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gfhnrzefk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gaijipqns.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gexpgnifb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnceohjvj.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gbutghdzw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gpuzwopcj.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gqqfcvbpd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/grdhjvztm.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxghhmoto.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gpaksiiqu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gmsbxmpdb.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gxrmknyof.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gjlszcszp.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gnojdclen.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gmlvhejxy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gabrbiohs.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gdyqwxbbp.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gyvnwakcj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gjhtsjjjx.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gfvyynttr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gopcvqwwp.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gtqfkjfth.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/giuwdfkzo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/ggpmytlfg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gyctjqwkh.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/guubpifnr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gjbdjphge.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gzqcggmig.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/grouxwgwr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gshzmgaus.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gtxueuokt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gqfzcojhd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gmhdfhauo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gwjnbpirc.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gypanexui.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gbzilaozn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gtjbhscay.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gfvtsxqru.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/getdzkkvv.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/guzfeknwm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gxueniyqo.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gqwjdiaci.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gdchcwfpb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gdhbfmdtr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gjsqdkbrk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gjdtzccdf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gztryxles.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/geqwsbxsm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/ghybimwyj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gcbmloacu.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/glqbnjqoi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/grrzmusyh.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gxquiupjp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/ghnwnrdhf.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gzhflnzkk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvghiiwna.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gtzzjjffh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gkgugxwtz.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gnjlvqtjm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/goromawwk.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gfocyopdi.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gxgobwnmc.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/grtsltthe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gccjhshan.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gcawatjna.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gbnewkccn.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gmftorntz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsqglgodh.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gkytfpkvg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gzqbwahyt.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gylbxtbzf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gwnayvtsl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gorirkhzd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gbezyntlk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gqlfwyimz.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gpkepgerw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gdcpgstqc.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gytnblsim.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gthsmtqpw.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/glsmhlhau.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gqvavwyms.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gutzteokk.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gumcptvzu.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gnaehzezv.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gyivltxat.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwwftovrv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gcrypnmik.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gxxhhzyns.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gwyetrypn.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gtjuydrzc.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gbfskrdvn.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gzzgoqmyz.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gnfoljpns.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gnbqofvjr.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gdeiqguwh.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpmzoyrre.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gqtrpampq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gmkdapidk.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gelgrqdgr.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gwpzzsdnk.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gmqxxfcul.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gjqfovwpl.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gqrkruwao.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/goizzuzbo.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gejxuzndq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grbjjifox.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gkoybqvzu.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gtsfefiza.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gwspmsbpd.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gqxuhjraw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gytlqkhfb.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gbtnhloha.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gtjcrdcag.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gdhbfewcr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gxgdpecuy.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gszjobhit.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxppejtym.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gfdsybbjf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gmzguikij.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gifaupalo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqjxplrbk.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gkzxnknxz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gcjbhypvq.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gjwbkrpvl.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/garoecghl.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gzqomdifc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gklssetrn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/grbrbkrzj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/goexrzsyi.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gnehxaqtc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gnlddtpvb.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gxmfpvdjh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gdlofthnx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gemfcfoay.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gibdmnciv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gzbvmtide.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gxtucrmwm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gydjlucye.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goycwbqob.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gfjkcfiit.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gewlilwdl.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gbplzbtjh.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gzswamtyy.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gxfnjastv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gthwjdpoi.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gaqubmbue.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gszcwofzk.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gdwbqvmhw.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gshzdxhiu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gruywqclv.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gbjtbnbjd.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gnkpjyzsf.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gkwpfmwkk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gctglnzmx.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gkyiledyz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gopeoilxs.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/geihjbuza.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gazglvzup.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gihncjctz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gqaolwxsg.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gxmgkgjvs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gfcfxhgkj.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gemejvkws.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gureflquk.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gjrxxdapm.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gjuzxvlsm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gpdyjbkxs.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gbspxrpyy.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gqulvsoxy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gvshmmfcc.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gqrtfxapp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gwvhqgnjs.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gvahsdywc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gdqbzjeho.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gwsrdezfn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/grwfuqkvs.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gbjttchxq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gtcbmxdmw.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gpwaeaxqt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gyihjjjsp.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gzfqybrri.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvnwcmlzz.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gebmxxusw.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gaoifctod.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gdfjpxwbk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gjgxjvppp.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gblkcixyr.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/ghfynoqfb.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gcyccugdx.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gbjaigvyr.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gaxbzknix.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gatcxxvuo.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gwvljbzgh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gzkjsfdrb.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gpgcewmzp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gurkavuyj.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gkfnjwwfu.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gggexzlre.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gouxqjyql.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gckvhykit.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gjdvwfxdh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gleccfuru.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gnhcwmwsi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gfxvfxajo.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gkrfhbqlq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gkoxzqdgi.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gqeqeugkw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gzknlhwdp.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/ggpvftfco.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/glxaqiuhj.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/ggfofysgd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gwrjhimlo.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gtrcgwbpo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/goxlxtodb.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gmzgapysd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gwrchsnrv.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gctvwshrh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gtoofvyym.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gldfokujn.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gsgjlkcpu.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gdzymogor.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gsfiwldfa.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gfpklifwh.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gwsxkmcdl.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gehrtgfsu.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gyvakrcyb.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gwkiptsyu.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gwwqnlcxz.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gsegkhkuc.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gryipqmhl.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gupxmnhqa.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gkwjssghy.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gpfskjlfz.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gxvyvuqab.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gwbdbembp.sHtML


<!-- 参考信息 -->