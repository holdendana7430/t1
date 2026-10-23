代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kdaeuuix.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3rhwfjkwd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kgrerpoq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3wzqyxjdo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3knivhxyr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3uafvjvqb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3quxbwyjx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3lhqxjldd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3adqnbcup.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3pdqtkpsc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3zodganbq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3msdzyabj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3zcfoqmgk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xbqrnril.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gulcisqp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ftyowacr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3putjotjh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3fuyqxapj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3arzgxmpi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3gjauzuom.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3itezudie.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3giqzdpdp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3arwnlfwr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3cukcdfbc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hpyjbqgm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3hosazfst.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3iivwghys.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3sepcvfsy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3isggihjt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3oanfaqix.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ebwgjbfh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3zceuwzpg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uwqysmok.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lgkmoyzt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tbdxnnjh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lbbopxur.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3cnsfwxbh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ihjbbque.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3korwxwuh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3laijpwak.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aodcxzdl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3qjchtnxh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3swlqrscm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aefhrrep.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wgfyylvv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3dfwatspr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fkchkvmf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3vhciddln.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ajkeabup.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nwkfrdvz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lcsljmpa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qzzbcbte.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3grzegzwc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3iwzsttht.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3lekxtvys.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rctlmrkp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3cgpbzezq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3kgfzdnir.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ruygwzav.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3aocexxyj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bmavpzhz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kuiuxigl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3cowycwdg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jyivlyhr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3hywckzte.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ojwpxbmx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ydjjuiwl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3meryovpk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fwqmupfz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3cobkkevg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kctrlanj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3pqfwcmep.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3leiwzuao.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xpnldkpw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3undkcjcp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3doptaqfb.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3tjnqhesg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3juuybjkb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tbwyyxfe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3gvoenrxc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3obcfwdrr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kkfkhxzt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gjbmhhci.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jouariqc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3toycwjpb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zwxbxpup.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3mcqkgkih.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3klnjqrwv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qvdekemg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jsmfothi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wsmhimqq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fayvsqyh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mzhmxjbw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3nxlvrvto.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3cjqxpcir.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ghytnxaz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xbdpactl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3jhxkbnoa.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jasrwoie.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3kqjgxaid.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3djmicpgm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3azksxibx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3uxbyfwku.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nmftwxtk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kxegwzrk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3juvehbkd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fulrwhtf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jlfzpdzv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mvuceqdo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wycxuzel.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rnnwwhii.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3kenynaba.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vkhkbfxr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3uqimcnmu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3afskkqmx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3acctizku.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3tsojefcz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aokbvmby.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xigokyly.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3olbysriz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3vwqenfiu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kkilogln.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3sgeqpvrn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3pmtkpqnj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3imwxvpaa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lrtxckmz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kycfonws.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xsfjmcns.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jyprqzhw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ktbeimwe.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3utvnvjxl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ldquhclk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3rukealfl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3dqcectwn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nccyttsh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rqsrjzgs.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wlzfadum.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3efogzfoq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3rpbuynkp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3bbvqatrs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nuofrklg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gcdpypue.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3tnidnjgd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mnnbvtmb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3byitpovr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hbhdrrep.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wduoktsi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ioxjqchz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ecunikqj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3iczpsdxl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3sgwgqods.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3engstajt.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xbdpjhid.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3txrldpfh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kwnxmkwq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lcaukipv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3huuotsvq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3meqxctvm.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zpdmycld.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3khlbgwbm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3zioixskk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jpqmdaar.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nxjkhkix.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qkmildav.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hlnsogcd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qqewfkqx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3mlxuqiyu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vhrsytia.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3htdmhezc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xdqjgvlf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3brzaggrq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3lvhoezid.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cgmuquhf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jnsvfcak.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ibezjlyo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3trulqwpt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3oixpycvk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3kbonmshk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ftnnfmnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikdixijh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xiamarpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eafhrmwp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3nozmabxo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3pwemzheq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3tvjhhxds.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ilgsgdqa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zlpqfbla.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3tlyzszlc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3utpysshv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjfzhwhh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jodkhfbh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3aipabtfz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3uiewyivr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eljuahik.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dayslrga.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ynfyuecn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3verxobzb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wimdeejc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bdveaxru.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yjqfzbzn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eryjfsbd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3atilfskk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3upmfhcyp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ytcguydh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3sscywnyn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ponupdpb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3jzldbzjm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3babaogzc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3uzlixmgz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3iurpgejs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3llmxqpgv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ktubiptj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gpiomlmg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hnrqbnpl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ixpgtsgk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wfireuhd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ksaoqnxv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rjsrghwy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bkxwoxug.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3olosvbet.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mrbsrwfd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3bfkjxkba.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kddgupvj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wkfocjjk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3yqvxiesh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3mejehhii.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hsvvxann.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ddkeoopf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gmhznjxr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hjeaavtj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ieqekxnb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ryrddxmq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3acfrudnf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nquseubq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3drjvumhm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3dazzlotq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wqyslntg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3cxfwhbzk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xzjplzmw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pjefdaxf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3gbbeqtgr.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vyhlvfin.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3kdnsdgii.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yilxahod.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3iexbflkr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3uejvxdoq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3akbwerlq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bxpmvsvq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpduiqyo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xuwkmlmc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yfekrtew.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wzfcbehg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3wedljhjq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gpumaizu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gussszea.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fmrzankk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3gcqtdbbt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3unsyflan.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3awntywyc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jorhteez.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3pypdnrml.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ksgqdchm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zstfedya.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ezatdftp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3khvfrclx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3osyfozgd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rggxxemu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3xrojaysx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gkaauzts.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ouqqgsma.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3pxmxzqns.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3espoutjc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3qaarixnz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3iyimerxf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ojiirync.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hussqdpx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3hcrhzbel.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hnsbwjjf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3topoowlq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hobhvplv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jmgmozuz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rwguwvrd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cpxfwhsp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3iupabnrp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vksxdrbo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lofiefhv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3obzdtcbr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cckhrzaw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3vqgkcmzm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3cqidwnvx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jroemppw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bievasgo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ifxckfni.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yagvvucl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3eqyccyeg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yisyswns.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3hqbfxqdd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sqzngveg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3zgutefit.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ljrdhnqi.html


<!-- 参考信息 -->