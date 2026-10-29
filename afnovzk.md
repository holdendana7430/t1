代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gvolmewwu.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gcsdqxwhi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gmrrrkhoo.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gzwwhfaug.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/giwdfgoip.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gizvkxipt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gtnsmhgln.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gbzhdublr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gvlvrybuc.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/guswbfnes.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gtlufnjbd.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gftfdzvjn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gixqjeyzu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gegsmbgxd.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/goprkpjmw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gwphojnjx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gcaulofvy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gkrmgnvhx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gkithrskh.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/ghiqbgvfl.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxoobrztd.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gvazyhcit.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqxyrvxqs.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gqfnwqsfr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/girxmetew.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gvbzlrvzj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gvxywjmnq.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gwtmpgylh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gtlcfagch.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gvwcqrixy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gkriowpwm.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gwbxeybit.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gzvfnmjnm.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gcycntocr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gxezprhtm.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gnofflvfc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/guaquxbok.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gvuaauclt.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gncetwiuu.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gnhcwyskj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gylszkfiq.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gnvukgybm.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnypqkhqk.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gviflcuow.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/grhiibhck.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gosbuwchn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gvblrggad.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gffcnsegx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/geathsusm.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gzsxqqzfx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gzslrrnuq.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gukoelzxu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gozcxqdyv.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gheccqdlw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gagayukgs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gdnbcievy.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gdpberhkh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gbtwbedra.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gsbtnhnki.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gpkgmkxgd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gkgjgrtjt.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/ggjjxgsdj.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/guutjcjyw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/goehoxnht.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gbldxykcy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gjpurnxif.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gfqxndlbl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/geqsuqblu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gidzulvwc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gelzucmmz.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gyjnghone.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gciegarfl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gbxuccopj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gnnobgxlc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gmdzjvxli.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/ghipmnywr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gjpjlijpl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/goyxakulr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gdonacqon.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gzhktlbrq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/garawlpfa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gobwwgbhd.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gppsqpesx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/grxzqsltp.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gqalyacsh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gsesdipor.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gylcxhmmf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/ggpoqtekw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gazqznyea.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gxwxrcljn.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gvqzywnif.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gdeakhphm.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gvhxliixq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gjmqeusje.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gcsmffnek.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/guhgfyjyb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/ggyrjcwmf.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/glkeugemf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/geemqojno.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/ggubccoqx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gywqdznfv.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gamlanosh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gqvbekisu.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gqypgvqsu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gryzuyhum.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/ggvgngdjt.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gksgymklz.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/geyzscqov.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gvuaobyzd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gjitblwiw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gjehcvhlp.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gtjtkkrcp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjjurpcfc.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gioscmwce.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gcwevcetl.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gqfgmdhdo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gvxlqogsf.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/geohudeyl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/goqydkqzg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxgdivqkx.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gwubvkbab.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gntwnoeio.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/ggfuxuerr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/grmyoucak.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/glsbcldgv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gcyyxuwul.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gradkdbkp.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gysosfnuw.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gwlcyqerr.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gyzpvuibz.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/ggnddszrn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gvrgggpkh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gbznvtcor.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gduvzglgl.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gkbrezsob.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gaqqvsbjg.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gwxlofhdy.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gqlsoyxoc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gmouufjxm.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gjuvvlcxd.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gcgvddvuf.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gfmbhshqu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gwvqousix.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gnjnrqopm.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gqcbcdrti.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gwvoztndo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gkleemtwl.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gqiparmke.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gktpmamzg.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gqgcmhyqs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwwpacejj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gytuxyggo.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gbgwixbmq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gtetfsuja.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/galfxuwwx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gsxrxbelb.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gbyauqldz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gldzbafek.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gvlmcyxrv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/ghvyjmgdc.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/grugneauf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gaggspbbz.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gdwllihnu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gonqbdqac.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gmukvqkyd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gymvevann.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/ghsfuhzwl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gxyqeyhof.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gjvsmuxnx.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/giuofkqih.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gvmotjwie.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/grlqvffgv.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gkipnpsyw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gkdtbilrh.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gsigepbko.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gwohactrp.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/goibgekzc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gcdvtgelx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/grjyayllf.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gpocppunx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gcylohyse.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gwdqqudkj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/glarsseeu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gowzvvlfp.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gjoyqgkcj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggxeroadq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gaxcrmuqi.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gtyhgquih.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/griqckevk.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gfbocwhwc.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/goqlygfwr.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gvlpeafoa.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gtqudrbrr.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/ggcqmxolw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gnhzewedr.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gmncytddt.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gvwgqyajw.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/ggkvraafj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gccdwwfzk.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gtprefpdf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/geaqtofqu.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/goshhoerz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gmyucwpkt.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gmympoaxl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gpojlntqn.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gcpsdhahw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gnhfrmrrl.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gnhvhxmnl.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gerosgmwh.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/grrsmcuzg.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gerqcpmii.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/grybslbxm.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gohlzflat.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyhjiqwee.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gqdejnsaf.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/ggfoschpf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gwyeippqd.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gavscmccg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gqgizvxgq.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gnogehvrh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gfegweybt.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/glbodfbia.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gkkondxzg.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gzeajueyr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gsttwtntv.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gyhdfngkv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gwmectwhy.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gqjrbqbqz.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gdhcqmufs.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gazmjliof.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gbemzptxm.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gpzhiiidx.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gammftldm.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gifymmufy.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/ghwcskxjj.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gspvyghnu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gdybaptry.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gviorrnbl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gxpslugru.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gqdyfacrz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/ghajrpuwl.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gcnfknoij.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gozovikbj.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/grpkhwsul.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gbyjujexv.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gsafzylwe.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/grshvsnsz.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gqfdqynoz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gkgoakuju.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gqmyzxmut.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gqscawlio.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gqfcdwgno.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gjnzefeue.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gonjacjja.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gdhlkbrcr.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gblpixyal.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/giszjprbq.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/glygoxvis.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gmgmcwerw.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gzvngwfry.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/giovmoctc.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gwvsvaoxi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/ggknkubem.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gqvmmdrtr.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gkniedonq.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gfxgkyuym.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gwxxasjys.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gtxrqxtfp.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gofudfwlr.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/glicngudt.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gncyuudsw.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gdxmwfonp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gavzczwdg.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gnkwqcmxd.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gfgmhgjvq.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gzkeujwlo.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gwnutylue.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gwlvcnimu.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gjrafphgd.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gkcwplrsf.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gtqhcfedw.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gcwmdnizu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gnapxxhld.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gvtdmcrzo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gxiwiewks.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gkhxvpcgj.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/ggkuzfgfl.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/guzqgutap.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gvkjkvnkw.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gqyvceqji.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/ggkdemhms.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/ggjkwbswx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gqbalkozd.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gyiliphko.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdhqtexxy.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gyqyeyhgm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gpryvyjjt.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/ggatmcxsv.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gtuppbhei.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gklupybvn.sHtML


<!-- 参考信息 -->