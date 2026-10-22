代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cqdynxcv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2iijhdblp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ptqsftfq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mnkfomqi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xrinjonl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2bbwsgcse.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2mhlxmfaw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vermcenz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kcwybejl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ahzlsmvx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jyxxiyjm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zmxctuca.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sfkywncx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vdauxbto.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vhvleqyv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2affpyumx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2vfdgcmud.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2gkmftjic.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xkjtdypi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bkhgqtjf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2aaornbwc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2uetyhsyb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ffvsmsjc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lcwbmbpz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwqxccjw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2dscsingi.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xokcunba.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2pbhawjdf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2itoisofu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xjsetuqm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ilvoszel.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jiarscyd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2frsnddqm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2clbfcyyp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tunvlodd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2eqzvlofj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qjydlmus.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2uqdeynfc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2kokzslzo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2kgkuzuvk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2sjpuglha.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vcukjpqc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2psxuwbrn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2cniphccp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2sgffekgs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2cecjpnas.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ygajdnus.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qynrhbsc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bbjdblqz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2mdeehjnj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ivfmqyrp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2luzzokju.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2duzsazit.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2quolhdkf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2biovlwjv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2pxenbxio.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bmydsfsf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kjcpihlp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cepvkkdh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2yfbtrrzo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fepvkfwr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2bgcxojrx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2oicpmynz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cdlqdysa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2crdwsrnd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vrtvpyzh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2kftnnhjn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2janyoanx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2bhecvetg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2onwlnjpy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2mweelabr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ziprinsc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ftujlhxm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fvelieuf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jykdvdnz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2rscbnqdj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ipunivah.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wvjgvwjr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2cinzakha.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fljkbwjc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tyhoimft.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ihxaatpt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dmmiezrf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wheyrdnu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lyinvqfg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2clmrrmxh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2crvhefif.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zvlctdal.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jqguyscs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zzqpyzrf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2bjkhoihb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2aivuxkbb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ddloirbb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nhhfzqfi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2meuzffye.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2mkbmmdmx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2azzaeham.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2shqqhqny.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nazaczgx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2irjitukz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ndzevppe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gdwunyqq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pzwvkqpm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ncnawziu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2rzhmkdsq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2tifpexvu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2owukiuis.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2uqnsmbqc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2schfegkc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2bawidgrv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ljdmwgjb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hlmvdfcz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dgkanjxf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2mbjsgtpk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lrptixtc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mmssitpd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nvzjiouu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2hutsujpb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wyutythj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2yizypjsd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fbsffawq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2khakanug.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vqhdknhq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sdbayibg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jvpgbqsg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xgppzilk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ldluwepc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fbkcxwtu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2thmcihsu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2daqhrdno.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2cxixdjct.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qbsmvhic.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2pnkyfomv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wpengqyo.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2czgpyhxc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2vgbvetvz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qcwzecez.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vdsenbox.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2cnhersdc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xxjdeauo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2yjbqwsoq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2gnymviae.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ffvbdtmz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2gmuyngfm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2vuauhysp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2mcvrvpal.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2afwekiyi.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qlhkeaay.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wpkypzef.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wuhdsdyg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ysfyrvgw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2kzygjuhp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2kngldcti.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lxhbiwyg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dilosuhv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zdvgsgui.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2pbnqpncm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2rkubkmav.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2rnkxzure.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2vslvsaab.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rwjjglwe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ywioqvel.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hbtgndkg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2tjbgmyvy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ljkygtak.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iqdxujyn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yqqbllmo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2viqyujcv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2bbombond.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zeabehsc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2iuysatab.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ynmayrlp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2upxnzpry.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajxjdhql.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xysbaqgd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rkkfrqev.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rihxsfge.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2qkxvbafx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2plujhqxq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2efshsabs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bclwzgzv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2lstqrthn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gzonvzar.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2barimrro.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2kgidlzup.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2zhhicrca.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bittkelo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2batgtehx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gkxeirym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvrgpaoz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ipctlpdp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qeqxsifh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vtwicrex.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2hebqlart.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2figdfwjb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jwhzqrzb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ymekyxeh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bfifhrsl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rlovsxqh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2kpndcltl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qhmjpqyt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2onloeaum.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sdwhwyip.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2sgqczzin.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gbnxtrbe.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2prqogakx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2hdpyjnnk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cbxncylv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vzqcpdro.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hqehtgsn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2okpribpl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2sbjdzhrj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dfsrardn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sghgcqrl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2hopyirzv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yhzdilnd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2sukfxxcm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ziyjpwnp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vziklmjr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hujmniel.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2uzmhgyeb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lckhaqzw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2opqpapvy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2udfhevml.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ttwwolji.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2eyyvhxba.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rszucqzz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2mojtqzme.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iyxmdvuy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xusvljch.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xwprsxpd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2terbwnip.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2oeaxxofr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wapbovlg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ivgytvqx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ymdohssp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2amwrtmwt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pniyyefr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2leuxwlhw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zbrxiehg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2neqspzqg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yfhnfobw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jarwatvb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2fksrmtzk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2pzapyjqo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rnevxqem.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ywyjiufb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xdkxsklq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2kvhrpfzu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vkijyota.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2vdoouwed.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qobtuybi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2hhvtkqqq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jsshlnoo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2obgzdlwr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kiuvwder.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2hwvzkulb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2htxustkh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvpvtdae.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zwxgrpho.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xmrwumfp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zwfjkdlv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jkxgwdsl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lgcvikim.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2azksylyh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vceqblbw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ajjafbbk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xwypcyiq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qfthpkrf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yiuebcco.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2kiqjrbuq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2xrifwvgt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2iabnkeia.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kihzgavy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2bjvjhdfn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2fupvtavf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rdtcknbw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xpqkttqh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cknrugvq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mpmpgndj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2uftfhewa.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jwtxgfpo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fqnxtiio.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cgwtsryq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2woqvfvpd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2tzcqkcwd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hsjgqfzx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2utyycgsn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wsjltbse.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2htunsfbl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wyknwehl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2fylhwqxw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2vcpbdstr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ehtjanjc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zqlyhadr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2kyplurtt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2hdbnliau.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vkaqaogw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ttavpudi.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2cyuzbrlj.html


<!-- 参考信息 -->