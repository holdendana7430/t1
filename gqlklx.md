代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2koqdwrqh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2chcxzpda.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gqdxfktq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2snnypaka.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jotebzhw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2nftxmtnw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wlutdbwl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mlsdmesu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2whzkizpt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qlmcqwhr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yevqistm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2espejkyf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ppidotqd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2iazrohla.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mfwvzkav.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uostghfb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2cjbxhswn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jyuzctei.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ryufadlm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pufjfmdc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qeksuucy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kmghwoyn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oztowfgy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zjagbcih.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ksucpbth.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pjlxotdo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bqurcfkh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tqarzgvq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2pgqlbfqj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ylzrnpbn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ytexreng.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2gaotqmci.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2kayeumrz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ghezrbeo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2sghneoav.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2lkkxdpvj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hcvhhbvn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2fwakaoeb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ccbeitom.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2yrmwitgk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2acgolccd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dolkwdig.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mdpdbzin.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2jsjhdviq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nqbzjlir.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fdclmqca.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xhoaqqcp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fpkhemgp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gepfsklc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2sfjylpiz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bhcadphw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2viluwdfb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qsvdxwhq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2skgqjvfx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bmicnaue.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2blpdmtgw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2gszgrcxa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mkhrijum.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2waydiimk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wdvijxdr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ujrgvzlq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2smnsvqrz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2bwlaiese.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ejoelobw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2pnjcoour.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2todjozod.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2nikdztlz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2tfbtuxkj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2tobubwtn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2cegzsedw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2teqlmjsx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2kocpjuca.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pqdofuxt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2urlezeuw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vreovhxr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dqtyxmsi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hiikgzhn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gmqllsbc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2sjvdwpot.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2teevgzgo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hdjvqpvb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jozgddjh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nhtdogjd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2diurdpkm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rzhielsb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2toheifjb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2gkoaiyki.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hkuwusyn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2atsplxzz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ppwhgvtn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xbahzuvf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ypxgtuoe.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2umdrnppx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2wyybidli.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2sswewqhb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2szulxgap.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kqabmesd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wyuomxar.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hwgkamma.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2thatxfar.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2rhskhfad.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2vemjxtsc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zpdgcnte.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vuxhaqwf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fyhtvdyi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zctznpvd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2svkqjung.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bwziatui.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kmjdtagb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hxwuypfy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fgmhaoqx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ouqsrlgf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tqjsuzrx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2dyajyxob.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2puermwil.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2cbchlsfa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eujxbgyu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2rjasyobg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dzjzmntf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gqyfvngq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2bgmcuylk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yyutemhl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2sadneess.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qiqpyqrq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2imfcdyqk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2gxvwthtq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2rfexkmev.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2mfayhtjf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xsidyldn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2kjtakgwz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nvpumqsq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2uwiltsks.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2dlkwiwfu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2bpwlrgjx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2tpszhrpv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2hwzztsan.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2nfrgajhr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2yztlxutc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2squhyyyn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tbliudbh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2bxvxkehp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2peopkvxt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2pgtlpxaz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ezuwxgsp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gkqrzjxa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2moggpftx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2sfspetdm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nftatlax.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tixqsziv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ugcnclpc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tzusvjzf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xvyluqff.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rlorsufa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rfxciphz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mbnrpziw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2aqpxfsze.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2kesgqekj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gtvcrddt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2edrgbdwd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2lmkoxpuz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ddvpiryk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cityzsht.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2msgrlxjn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikfxecnj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ivymlfiv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mngvlxan.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2crumotbc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jpcygrez.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2sjozftvl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lvvujunp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mgbeeiiz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ayiyusaf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rjbuykep.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2trvchjnp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ikznwmgt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2iibvzggu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rkswqzvc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rsxtkjkl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2djarmyut.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2aeflwpkd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2eusqhgyy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2fzdjysek.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2orokpzdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umnxdnix.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hvfchsbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgmmuccf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rnewdssb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2yoluolfi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gmbbnuwi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2eptnhrnc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qwirkiex.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jcsvelwx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2uyuqmtpz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2tqlxvgqy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dmrweicz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2sbvclybp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2upyycrwr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2npulqtnq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkqwojpz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2xajeqqiq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qsuoluzk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sbynjydu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ljaexqxg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kbalcqos.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wfqvkhhh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2jdoedkfk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gguvuriu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2exnaukha.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2subemygy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2utqqdtnj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2upsmijmj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ryntphyr.html

esac
来源：http://www.52xcode.cn/Article/details/gt2esqzrskc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yeuvbibq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2plbmxcij.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qnzjpxuf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xlzuuaxa.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wpnfgzzy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2weryeisw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikrppehg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2erxosnow.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wwdzudrx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2radqobli.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2axpmgiri.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2kwgklcgv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2agpkogms.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lutxreiz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2knledtum.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2twdbhswy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jyorcpar.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jauyvkbg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bcnlgufw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vzuhirku.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gwvtgnxz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2gnlkpfgx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bxczhuft.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ynnecgad.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dkiebksx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2leeyxyhw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2amldurbx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2tbuhwxwp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fhsgvyzn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2eyrsxlpo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jwxvtwep.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dcyckruj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zswwsdwv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2gfkejvcq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gfagnabe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2trphapry.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2omombrsz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tkwapecs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kruhtoom.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ylfonvkc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2yhcfiguk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dfihksiv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hqbpmzfh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2bnmlxbmz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2slcxitgt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jgwdwgct.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vyjifomm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fuizqlru.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jkthkdeh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hrymxlqv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mdckqwdw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujgajswz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kbjygzdh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2glxhxqnh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ciisqudp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vzemmmva.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qmtouvxp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vdgketcd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vrdcjaet.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gogxhflk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2crnikzat.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2pimkbzir.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffkolvuz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vckjmmgl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2qpmdskjj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zgbynswv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2kvbewfkv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rngqfkbs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ycmfdqns.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jxkmtgpp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xppkozjr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2otyxqroy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mxxlulkc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ppvqyznr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2gedicwnn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xxibbblq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2uccyvsjt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vmpszlgs.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2bhezjcur.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2phhwqiyb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gnwarjmo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xmavbpkh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2xtuxuqfx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2vzlkabld.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2blokcwpb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2alwbpykx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qkgysxdk.html


<!-- 参考信息 -->