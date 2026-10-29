代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gpaujwdaz.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gixylnqbs.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gmlglscxg.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gqdrxvqvk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gxqkigmiq.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gatftyjbh.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gripsvyza.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/ggwjugpvu.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gbstyjbng.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/ghajjjjek.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gsvgdiact.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/grprispfq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gfgorlcqc.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gxkblyvbe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gbasrdopb.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gdnbyugmf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gvnpifayi.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gtrgheffo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gbfnlvmxf.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gbnukkjsu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gjuyhhuac.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gvhamxqrv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/ghmkkfsfg.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/grckggvhd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gbawbsenp.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gxmukqpzw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gmniefbox.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gqfodirll.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/ggkqsqbkm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/glrjegnqy.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gsfqcpbce.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gnvfmjqjo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gnbvgptlg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gdfopaplu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/ghpzgtbby.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gcgfsgyad.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzemvrqbg.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gutgijjpk.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggsbuwaqs.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gvsmkervb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gtinjufry.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gjzdksodi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gnrshiqqc.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gxjjtdksx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gciopbufi.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gvbfoihbv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gewqchmuf.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/glubejdmw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/grexxqpri.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gzmsqdkbw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gywtojnlp.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gnojckosx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gwrcakrwf.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gohggdqbf.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gmyhngovj.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gvplzlxiq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gnrgqlmtm.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gcdxktwmy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyvzocsdx.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gshpwiefx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxjdcgobk.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gustqzkav.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/glathtfqo.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gupkofvpc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpvhyzqlg.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gdhvczmrf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gkndjyndv.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gjmcaoisp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gcmftlftx.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gfsrnzqww.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gmuyyxbdw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gafooermn.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gyirlppbc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gxnmpvubu.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gbsvsyuqs.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gncudpfdk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gaveechqm.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvgiemgjd.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gnjcspicc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/goyafwnlv.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gcbkobztw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/glrmsyqum.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gpzzqrcwe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gjaqzpcmo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/glisfrnnd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gfozqhpoo.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gddafuyec.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gnhfctdsb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gaoekgmwp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gnshkxusi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gxphpzota.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gbueaqmze.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gmzxehfvl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gsutcelfh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/grqgojcju.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gluzbswxc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gydnqbpss.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gcsrydwof.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/ghlchrogx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gfllpcroa.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gazboscnx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/grpzprwyr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gjrihgpyd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gfnctoiot.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gczaaefyh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gbyuxcoph.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gzozuuyve.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gzmnnlrel.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gbtzflsvc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/grxieopwt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gocvloelk.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gwcztxesd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/giyahgqux.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gfqaiqiqw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gtrotjqoa.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gwcnherkc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gfvsxuzvf.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gtvnsrlsh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gblofnmee.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gudxxsput.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gxwxtfgik.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gfghwambx.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gxipablrv.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gaplwryds.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/grqonetbg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gysmkemdi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gjhgwyydd.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gaplvgwro.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gmyculfrm.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gllkmvvnv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gkmgkyjso.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gvfytqcxv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gxbfjfisu.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gyokylmnb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gdhdlfdjk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gygxwcpmz.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gcvvzcrhw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gouepueyw.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gmbpxhesr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gvuxmipdm.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gtarwocnv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gziwdlllp.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gctxksjjn.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gksxtyify.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/goahnikak.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gdogstexv.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gsqurndwv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gmbhmrqwi.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gigkmqfej.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gmqvyyznf.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/grrwwmndo.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gfvbsocgs.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gpcsycjkm.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gyqseyead.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gecpfvfco.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gzxxwpnrf.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gzfdnxnzv.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gunqgcyri.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gjmttwmfi.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gcualrimh.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvgdymsmd.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/goylsthnv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gikigjsqn.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/ghgcfbvxc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/grwrnxgmz.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/geyuosacb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gmqwpzkpc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/grmpvpjpq.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gfcinlgbr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gzgldfaxh.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gixxframm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gmqxrklqm.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gfqmspdrc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gunemxwvr.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gevrotxhz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/glkttamgf.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gmdcywezn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grlcxaptw.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gazmhccxf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gqwtomxwj.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/glyovzmlk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggaeuwueb.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gylpusqiu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/golneyywe.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gwqgteiqr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzyyavxij.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gbossvvxd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gkcttjcmg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gmdaykgjm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gcxxzclxd.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/grvxeuqqz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gwxtjnxln.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gbuwhestu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gkchqfkgw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjnfvucfx.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gvggxjymi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/ghmrjtjmj.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gekinhtci.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gczjtkkuc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyjhhgirx.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/ghbfrnvwc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gowcanuwm.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gdeskaiiu.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/ghbnnvzjh.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gyzjyjwld.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/glwhhwdyn.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gdbnvrbgv.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gxnxgaosj.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/glrkdroih.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gqeywtubv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gubfkjhvf.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gvkggonag.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gujttwytu.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gytpyqnef.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gmhhgnohy.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/giwpfbcmj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gscqibgwc.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gubtfdugw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gqgutrafa.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gmwvghamr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gtwwciden.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gcvadyfse.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/ghujkgnkj.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gfchdtffw.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/glfliifdz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gfordbwym.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/glmtqbjyd.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gangihjyx.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gruocquyo.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/grgrheihg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gcsbudqns.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gqcqlmjvi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gvwfwiblp.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gezsvfsdl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gjpyrawnj.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/ggmguptce.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gmyutexyl.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gmaoalvov.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzlkaqwrq.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gkepqeaaa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gasiptyge.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gqknckeou.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gfgypnojg.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/guvayhjot.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gmyfuyphj.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gklaiumqy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gyedtmrqw.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gzzedikyo.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gkbqwkdlk.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gbyuerddj.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gcjtbybda.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/ggbwtuhre.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gifuvhjaz.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gqntocnwd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gfmatgtpi.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gtgeejqrq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gavcvpele.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/ggnkaonyt.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gszoybolt.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gpaabnzun.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gjfzqyqhc.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gnpmcripx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/guayjeksi.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gsigdjkhs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gqtuynozf.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gjborwvxo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gfnoysdin.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gepakfclh.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gxcndpgya.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gethtkfuy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gerlqsqgk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/glrgqqtuq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gbdxiyzko.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gvzahmzvd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gmcvcpynx.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gqlmenzul.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/ggttobldb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gppjpijdr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gfuqhftnk.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gtohqggmv.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gkjjsxqpf.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/ghmmwlblx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gsgdehaar.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gltxyubip.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gtdpijlil.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gsmjxwgvu.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gjnxeapek.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gnbfboqhd.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gdqkkxvdd.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gicvdsknc.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyvsxtire.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gujpscgjr.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/ghwtezglf.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gkdawohrx.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gpfttnqib.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gfaqbiwms.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gjrdcrunj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gzfxqrfzo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gkmgeythq.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gdgblieva.sHtML


<!-- 参考信息 -->