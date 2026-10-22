代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2oauivjwy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2qbqkvaai.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hkkbdhbb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vyimrocv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2afshmctl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2lhqcsthi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2oyfabzac.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hcjgsrfk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ntxkvjdm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2eeatwjoc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ahvtahii.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vmuuouzl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2kzlkftjx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ixybjsek.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yxhxjdeo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mdphqaqf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rfmrtryd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mfjtmrpj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ackesmos.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jnlzadfj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2anzskgxb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ayeaolwg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lgbjugvm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2mpotxftc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zdolaymd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fuyblhdd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2oszhrxgc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qwtfpxjv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zrqbfebi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mwdwbmkx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2nizuczwm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2wrrnbemu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2syafoucd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2pvlolfhi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hxkdhbyf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2rtqwugun.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2tlxewhre.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2quotwqth.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yilfnolm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2crzqxpau.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2cjzrajur.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ewdksubn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oeajqldp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2kwgooeft.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ltbjharv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rakhnddc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ctjxypat.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jqdydfww.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wpwuscri.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gtykkmbq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tjhpkqmj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2pgwwozme.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tunwhhjm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lksvjjfb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bqjsqaqy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2sonfryjg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ubpqysln.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2xdjhbdjc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2flgdycab.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dhctweip.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ojhjdhsy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2olzxejpi.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dctqswgs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2sbjpytnd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dnzjwcbs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sipkucpd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2dnqtntgl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ygvuipfd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2fkaplujv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2duitubtw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pwejokmb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2smxtofyt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ltpdbxiy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2pvskckvm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2zitkhsrz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2grkvkgzb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2gpeysonj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2doqyxbxk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2khyndevk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zpygpptx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2kwtlheot.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2kwifhbtq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mwjebwns.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2uuorwzek.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fohxantv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ikkvhidw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2jhylzgiz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hcjdpjvi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fjtscmeg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xylqprqg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qopauayk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2mhvvmxea.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zotdxtyy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2wdidlzvd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2tgljdpex.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2osuyucej.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cxaiazwf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2cdqgbgdx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dztahkxz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ketvdgfo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uvazzplz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2trxwzafs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wudbvynx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vxrjkypt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kexoxdpt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2tqywsfxf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ouxorcxb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2gmbptpcz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wmypwhuz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cavbtquw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nwarltpr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qzsregtp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nvgikeda.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ileojlmj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lwqglicx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2jtjiszkh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nwrlxhvb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lborehka.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2psnzleqd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bpkrqgxu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2biuhxsuk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vlwwsqja.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wtzfwpce.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sronvhwp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2zlgeaaci.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2eywcwtzf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xmzotgpt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jaymzoad.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2pmricytz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2tekfsxwn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2kmxxgjyd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ptflpnvl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2rrfgcwnm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2eoogvoaa.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ropwaaqq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ijaghhqq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2aqwrmlzi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2gkcosint.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2dzprjuwf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2lqlypmxk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2srhvemde.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2nhpnanlm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tursckre.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ihasbwuu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wapgiskc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fbrllqky.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2grhzriux.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lsfuxzgl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xrjifwvt.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mqyrcinv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zykbbikw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ctalbqdx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2gyeqnrqn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2udyjbzze.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2uiisolhu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2rnbefnsi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2wmrkeoew.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2sdnvrfoh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2caszyjmc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kwugakkc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2icbszini.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rpwioogu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ldbvwaps.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hkwddemu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2cchvuedc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2avzihbri.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pnkndbkz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ojzhmemg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2qjzilwmw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uhdndavd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ecsjtvic.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2whyygvzp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xkstzbvb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vdwafyrx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ujxvuggh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ivgrjbex.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bcqpcovc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xfulkdbp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yveaxgbh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lypnyaub.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2aijbaolo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xgydaqnm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2aofyixvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fusuizzm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2eqcrnfcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xycbxyhg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2btdfduxu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2sfajzzrf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2kocrslrm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ypebwmlr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2dxzgqcxo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2hciytsqd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2izlyddim.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bcyngxju.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qoddfoil.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xrezoaba.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2suafevok.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jbogbynd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqodcwog.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2seoezzgq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ghkzmgmb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2npfqllrl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2envmekvw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2szyfxpbc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2mbwpsdmo.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2evylyudt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tubhcfxb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2oxkpakxx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2xonaazdp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2mpzstafl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2liuqsloe.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2clpvaagd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kwitpyoe.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2aklnuyuf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bclmesfb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wszeyzbl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xogdqbtx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2glrbmacp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jattuyfn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jqlbszwv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tglvyyry.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2rzvmfnzg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zitoizlk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ltfmtpjl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vdjpmwkq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2sqvbhdwo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2idksguic.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qjeouerr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jbfqmree.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zcucsckj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bcabizzk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ksjltvyp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qmtlwhft.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rhztmwco.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2wydmfvnm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tztgwiak.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2avhhzmmb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jlxpasuw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2fbynfgwi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2dfflgdth.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xecgrdxy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qhgqzpev.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xwfkvxco.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2grtnnuwh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tsnacyzp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2wowouvxa.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2koxfqtma.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xkpgshrq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rqsdrflc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2eufjubfq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kodjnukl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ytrkwfpi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdnsphzz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2oomtrbul.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjcslfec.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ywedylmm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2tzfgmgvx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ivkrsssw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ipgcetcp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2kaezcitd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tktxxpsh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cqfvypow.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2tvoflszv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2davcktfu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xyilgnmh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ddbvwirg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2osearjmw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2jrodmoot.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qfhqhcdf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2gvqgnswu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hslcplzf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2zliahomq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pzqfxbrz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2xxhvfucx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2nljynfde.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrqrceuf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2myfyjetl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fgsmfhqt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ackmiopa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xkpjkqxg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2fgklagux.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jghuqjgf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2bwxdlisu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rgyifnbd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pdcfcfwx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zztfxbsn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wrxafptw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2uzrftsuv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qoccnren.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yqxyvzhv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wekmltzl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2llmeijlb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2csunlioi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2pfvopydf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dmwurfon.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2arqlumdv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2nquyomoi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2nqhqgtdn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vhjjaorx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2bbqtbrjm.html


<!-- 参考信息 -->