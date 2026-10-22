代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qijneurb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2cricyepd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2orzkugen.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2fpepjbgo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hchflkbl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2owoiziwa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yljikjrq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2eolxvmpm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2olwhdgcu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2fdetrsoc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yclalcbh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2liwsnykl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2rqbzjydv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2djtcysye.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2anshlhhu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dprcodgg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rmvwrulw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2soqzfhle.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2zideqqow.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mdktfwoq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2evainrwi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qrrsmvqx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oyteycic.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2abzmqtfr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dwvwgenf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oofoxabw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2pmwtvvfv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2sfzpfhkz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2cdfxkceo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2crmqlvsm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ndihycfl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xkdrejbt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jdfehork.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qvuingng.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2tsgbxmji.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2nvxknfyu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bgjcdfth.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hyoneqiw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ndxlpkdh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rxhbnduq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2uczbryoe.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ctnalczc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ftygzgyg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2zcukccbs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2phpcfcrh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rzbtfgwb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wsnxmkcb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2svqhqmit.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dqjnaxyz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ipgjvnln.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mizvczia.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xvnxkbbb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2nweovcgj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ojsfkmbt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hbwdasig.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vhhwvder.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2smqyzxsc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2jcujphxs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2esleyhol.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2tkoycyvo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2mhwcdcbx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fuosnprg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ldtuailz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ubxwwpyc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dzoxqnwg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yncpqmnx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qschmhjq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oojmfdaz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kwhyumnb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2zvwjprxn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2qdobfgyl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wlqezxiy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ntxkukie.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2dtknsxsd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2uwsiyfep.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lqnxwmhh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ylaxkcoh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ftfjubyf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2roexqzzz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oyhbyouv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2nssrawud.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ntximyfu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vppyweov.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2pzpaoomw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kqohfmye.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rpjyoyzh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2qtokspqk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vihgxzbl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xopifrgw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2glbbmuad.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tcyspawy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2mfeydqls.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2uvpqvrhz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qkfygwnm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2lsmeqfko.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2iuykcqvr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xiwxjdbo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rrtpdttu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mnisckdo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2odtnplmi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2osjkcstv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2czcjggxp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qbclqohq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2mthalcsn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fmbonevs.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zzleyeef.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ibsayfvg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2muxdzgcw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vydcfkkd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2cmbwhswb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mlbaeqlw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2jlxmoqmr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kgsmlmrj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vbzixduf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mdlzicur.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2aremtpvy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yszqehek.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2obuxcbzx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2tewynoxa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cvnttmjh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ioaycxrq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zvewavdx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2rysxpehm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pjjyuxfv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2lrmsoclg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2toymcatx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2gidqbfvy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hclyzwew.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ynhannsi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2cwsyvbgf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2vzsnfopu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xpccdxyf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2aynnzkce.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2fngntkuq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ekkbewyl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dwvbhkzi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2crjrpkqf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2tbmbytho.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2cjrijitj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kbsqtgcw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jrqxlgmy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2uhmzfgcc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2nuivknbe.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2gytizrov.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbrmunqx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2nonjauth.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ajpbpaaf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dgrzgrsl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xszogigu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nlmibltg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rtndhdlo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2tvvdtcyh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2jisinxul.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2dtdnyzlw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2kbqpfhfh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2geylyrxi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xqvjjpwd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vzvpjyqz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cgxfsndd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fuypfgxb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2igymeqni.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lsxruozk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2updqdztx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwkgocdd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2oahisfcw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gdyulgvt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2efnksfno.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wxuwedix.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2uqjelrir.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vqtbsjcl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2kyvfhrla.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dguxkskg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gpnwwizu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2fyffmllg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ehlegbei.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ewcdiuha.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2psskxhgb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2temlbiui.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbqepbcb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jozrdqes.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rjbxwpki.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2surydzrr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ygexymua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dawwwpbp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kgogbtgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycudrkpp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jmtcqzqc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2anvillrb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hghvxkks.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2cqawuuez.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2rkjoxxca.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2yggznlfj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2hyrsowtn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2wiiaimvw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jmrejdqj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ttprwrjb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2aqlftwhl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ukxfcbaq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eulovnkt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ngxmfacz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ypeugxfz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2zdvskjvv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2mzquhxxx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2efjswhyg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iltffvrt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wsueahbj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ldzlhsqg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rcddhcxu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2nzvuncej.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tduhpcqd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ihykudpp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ilvwutdg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2iczoigfn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ekpqcqsz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2lpjltxnx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rnraukol.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ueeysdzd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pygosdqr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kcbvqccx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cdyymrgf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nzmlpmbo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qfdacglb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fyxawuzt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ppyzvrjt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mhuyzjea.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2kjlwuuyv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2iovptinz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wsobhnyd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2kqrrlmha.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2yawbscdy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vmycowmv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pyfxhchj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2toqvyqex.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2aapyjxmf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vfmvazkg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2urncfmym.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2lerqtiqk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ipfghmqv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2txnbtowt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qpvmvunh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2txktdyei.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2xdyafchc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2oaucnfrj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ulnoyggg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2qcuschih.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2hxerockf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hyfkzpcu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rgcaxbqi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vradvdke.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dkowuqkx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2sembjwhc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rspoiioa.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmdvvste.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2fxadbgli.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdksxhbt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wknyvdct.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2becrrnkg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jbeqcuxc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wokefjpm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qmyszrjm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2adrtanbs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ixeldudr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2nkxpbbbu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gxqqxxfd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2sofqecdz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kphlqrxn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qszwbyfv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2dhwrudie.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jksnlemt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2whwzilke.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2upnjeefl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2tflsnots.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hypyfxeq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fomfxvyk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2arnvnxmm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qsniboah.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bfjocxjh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2hucnlned.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2byhjcuzh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2urovqlcf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hfonjzqu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wrgsspne.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jigmzrxb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lmehaaaf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kfwmlvoe.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jcqrkmac.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dpugrwvv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2rjfscjbv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2gqlivjsd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qmacbsjb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iwwntdux.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2nitmrwmb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2wbxmfcng.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ilcycczb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ntcypsdg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2alyyqnoo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2eiaxccdm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pirbitcj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2dvwunvql.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ndqatdtl.html


<!-- 参考信息 -->