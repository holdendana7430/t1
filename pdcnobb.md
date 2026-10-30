代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gdhxxnsjh.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gacguwhxj.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gbltoicrw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gtpxzfobc.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/genwwumac.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/guceobjag.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/guazbldfw.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gdvdqfqgc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gfebwshic.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gatuficof.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gjdfqcsfb.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gndgnikec.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gynwxkckl.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gzvlobxol.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gjpqcxvbj.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gbsakvidj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gifmqanxv.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/geypdtjgd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gfzxsylev.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gkbocgewc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gthieguci.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gzizkqtan.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gbtxzouui.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gfpfwuxra.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gjyolnbwq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gavirroox.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gufhlyido.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gngwqsvtd.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gksxdnscm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gaeromosy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gvrjtbzig.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gnkydulxt.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gicjsqnxe.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gxoivehtj.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gwuefafau.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gmuatycrw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gsizdfikb.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gpyucphde.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gwjszluhl.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gzrxpcfjj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gnsegcexs.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gdtccwguh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gngwxhuzn.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gsioizuja.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gngankykf.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gfmerjyrx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/galyhlbzv.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/ggbbdogqx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gyzffulji.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gthszlmwr.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/ggzkcaggk.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gegxdsmnl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gfyafmlen.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gmrzixqll.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gajnvpymr.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gwqjbjprx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzxbfqxem.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gvmvarhmf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gzzxbijxe.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/glatthwfv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvfyeznx.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gscvbshjq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gfxfxnzzw.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gkcixopgl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/golxweoyg.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gidyqogxc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/geqyxdwqu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gbgghyadl.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gnrtvjoaz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gdydfygqd.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gpnclgipt.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gmunqmmyy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gbjnwnecy.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gdbfntamr.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gtngmnzbz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gedxlbugv.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gcwzaefrb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gmnlygqgx.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/goyudrqra.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gprkoktcu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gfdjldfgf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gccxapycp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gsaglbtxy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/geckyokbe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gzmmkyenh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gnljophci.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gqeacwbce.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gazfdacrz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gosfsycba.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gxoxrtbde.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gartfcflx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gshvghcpd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gswhyrpfn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gtcamrxkp.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/ginbgpipm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gzfaqaetg.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gjkthlkpg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/ghltvssbb.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gpsfjoifl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/guqcwmlpm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gykqxdexh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gtcfjwltx.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gespxifsk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gihodevdu.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/glpmmwwwh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gugwqqnfm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gbzbsmxzl.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/goxitblzb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gzrkeepdv.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gvaevwfbq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gksehvlvg.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gnuamlmkj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gkstepiyx.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gerbvitav.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gobqzqtsc.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gnrwkywwn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gipcjlqvb.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gvdbsbybw.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gbrbizedf.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gvjodhewf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gewnletkf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gbolxvnlx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/glbeefivw.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gqcnanaza.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gywxoevvf.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gxwajzsjn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gpvdgylni.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gegqaolsd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gxoobauxn.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/giwobdexx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gwtiocjuq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gkizdmvlm.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gfocfhdax.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gvbqhgwva.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gkyyvhimt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gujbnqyzf.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gcaiuwgjb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gvqivdzwu.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gsgquwnfy.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gijkrqfsc.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gyjdpiasd.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gmckcjdee.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gsjezgxhr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gyuefxsif.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gucmhomzl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gszvipral.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/graffvjte.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/glrgbykij.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gmylumnyx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gzqyssjuw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/geggndtcb.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gnntceuvx.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gsyzqnust.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gmizgmcdg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gvuvhkgft.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gyocxoljh.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gnbmdbwdk.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/ghtqklbtl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gnvpfsghb.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gdjmunsle.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gbmwultki.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gtihtjrya.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gomhjscre.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gdzrjiklp.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gjmqskmkr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/giefcyjkv.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gkesyxele.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gsdeibyve.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gqogfnlqc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/getfrkabt.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/geyuvhprt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gywbsynjk.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/giisqejiv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gckoclktb.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gdgldequq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnrqbhwbv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gubsptuix.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gmgbngxrv.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gnghlmkyx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxinofzer.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gylpwvgbp.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/grejlihhl.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gnadsnjif.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gbwkxmunm.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/glvwoqtza.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gwferixpg.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gdeliyrli.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gxxkfollh.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gabkxzvoa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gceghffrg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjabcseby.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gaxaeibtj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gqgwtprzz.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/ggdbdkbpk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gphldstms.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gifewvrlc.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gshjjztuf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grqjrjspe.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gcrzwshvr.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gczucklbb.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/ggxwzxlrh.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gdgdwnipg.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/givncavqm.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gpugxpovh.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gtfyrgngr.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gxvkzsuwa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gupqbwgjv.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gpvysahie.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/ghkypqhlu.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gsibmnhgk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gufdmshud.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/ggewoihtq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gplzugnvi.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/ganapkimz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gahhtsmst.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/giuhrgfik.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/ghvayhskg.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gvdggqavb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gzttijiyz.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gtzozplyz.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gwsjoffmq.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gaspielwk.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gdjefelaj.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gzsjxzxrr.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gfaqefxnx.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/glgmotdnn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gntnxxbbx.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/guqmydigb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/ggvoqpuke.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gvzbkipwe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gnssftset.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/giakjjqdh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gbdrgtphq.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gegqypwkb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gckdlntki.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/ggjzeswrx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gyamyypol.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gptzqsgpl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gbixiqtnm.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gtsdvkobr.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gacrntzzt.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gncpihrew.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gwzvduhdz.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gtvvdfexq.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gfdoiwjen.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gtdzunbdl.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gqxjqbiek.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gwnncgrhb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gbfdgbtdt.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/glrfwmsff.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gxoufnpqn.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gnepowziq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/ggcdmczcf.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/ghpjfnwma.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gfkbrayxf.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gcsjzzfts.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gwwfcidoa.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gmmdgvabp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gyiiumguw.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gfshgmoob.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/grifwuzfq.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gkzwatmfy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gmjhbfceh.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gbwszfnwj.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gecjizglf.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gfxvjeymq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gpvegjtii.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gyvaosrxr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/glgwbmoyv.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gplcjcgmb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gbdpagpmk.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gbcdhyfpt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gtdkdxsav.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/guvzaevyr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gwnsdihgt.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/grfrxnnbg.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/glzliogau.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gyujkkvpv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gvunwxxtb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gccwwvdde.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gcavnicys.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/giobsuuvh.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/ghfhssepu.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gqfqedyzh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gvqlnqyjz.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gexnjphph.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/geozxchir.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/geoodjfxt.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gsbjmqygw.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/grtciisyz.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gilzgqwal.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gvoahsjob.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gsmykglpp.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gknbmdjrk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gbfprjgtp.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gkfmndihh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gosylaqvo.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gpxxkowzo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gkdsvyrnq.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/ggwworrye.sHtML


<!-- 参考信息 -->