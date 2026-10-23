代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bcxxtgmo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mkfdcojn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pwpjkyrs.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3avitusbu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pottqgho.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3uwwqgdkn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3viabwiaj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jgsytwau.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qgarbmnv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3nkkstpdg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rnbadeye.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3jjwomliu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3txhxrtbb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ltbvakzo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3yubusell.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tvhovsim.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3tkgccofi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3izgzklyi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xjtbyviq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3sdndtctc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zfcgzvib.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xhrdewct.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mehmpvpy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3afzvxccz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hnprigja.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3viqfhvwb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ihuqnala.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3divudyde.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3nsdpgsnn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lioudslq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3cfcdhttm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3jptikvto.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3szoiipdw.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3bygvngms.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vuvoosjx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3nxjkaaap.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zqwdvebr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mleywdlc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tdafdonk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3iidlndfx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mqrvbpac.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3uijlcvhm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xzsmnmdw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3dvkgxeax.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bnigjxpq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ptfecmxs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3blahrhml.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3npnrrmhm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cvwwkldt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3afhgkzvh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fykgzalv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jtmipaka.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lkzdyrla.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bzwwylid.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lnokybpk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qhpaifln.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3xxbgnlqu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3cuykvgih.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3juontxtg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zytaeiie.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tfdvahnr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3egmihbbe.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ihfwaumu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bpvqqnyb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mxhmneao.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3catpvqbz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vvjesufp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cpdhwrig.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qaclcnuu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3iepydztq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3uiibhkcs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3yxpelxrb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fnwuljvf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3xlehjbrn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hmufjpqv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3nvxnokcm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3yrqoefes.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3nlbwgjoc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3bautvotc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qxfoleui.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3acitiuzi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3atetmhtq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3toxjixcm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3baqbkzsl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vzbvxggh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3texesqyr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ubomqncq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nrbrpplw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ytenhczv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fphgrbqx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3wevryivr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3bdkdeekk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fzsilveh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xnlgsjlg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ufwpkrgm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3obkhcrjx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oomvjolm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mlryzkyj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hcqgrppt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ykqbgjlq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3egnhtrqm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3srwziqea.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3edruvwvr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3pgmxasrn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sdyjdabb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3crlpgwed.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nsskizum.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zvzvfsjq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mmrzxybc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3nebqblrj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xihfepkr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pumyndac.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jyuhicwa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wzikmtxx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lcubjomu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vglplisy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kehuahnn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qlbzymox.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3icvyczgl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qhkgczjt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ttszsigz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gilhogkl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3zzquudye.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pgzpnsuc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hizllnng.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3askbnkja.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3coilbwir.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ajyefvot.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3rxnzcoyd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3mxttxdeh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3blvxavrm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3iahyrnqk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3nqcyuegk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hkxgovpq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3znarurfh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ibpmmhmt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gxoxrhdp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fcngfisf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3azswjewv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3wlbkgndm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ouuhxtmp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ajgfbmpv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3bunecmjl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xpwjcsdx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lkhfdeuf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3mgaausmf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mjosmezz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3emzghstr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3xhlqhyvn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gjtrbxqq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vluhhewk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3unrcsyes.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3kunjvqdt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rpxjktmg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3otaosxsi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ciubkhys.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mfjajqcp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ymeozfwh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3udohgvol.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3irlqdexb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mmekkwqk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hcsbeaeg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ryvnsqhn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nlpnqhtd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xsoibzvp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gltorfcs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dnebhlxo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gwiaxqba.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qlpabqrf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bydxaalb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3matsjihw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3pnetmlvq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jitsvpzx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3puijifpj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3cvciljsj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3akvzoieq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qnlarcrb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3znapdhme.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cgdvfckw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cwzouiab.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ucshttit.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hhptdfrp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3wfxbhuja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdwdlocl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3otbqauze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3osgfijqc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jtxsdvws.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3omvnydad.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3mwffciet.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kzcfbgsy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hqkzpqbf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3soqfqyhb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3miqvatkq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3smfxhvhb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3fwmvuuqr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yexyqzvr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hrecgtmx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xlyvbjeg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3arttgflp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydarwxht.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kbqpeyvh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3npdptcne.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eimubpxv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3adpepwdo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lldbjxfi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nrbqwtyz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3lzdigkfv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cnwemoji.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vhbhtucr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3cpljlmfv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3oxcgtpyc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ysqqstod.html

esac
来源：http://www.52xcode.cn/Article/details/gt3wriilcyq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvauwxuo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wkfrfmtr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mamftxet.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cbbnatve.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ebjkrksq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xltfgblg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qpcxhwsl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3alwrjahs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3pluvjtiw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ngvjgppy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3opxqceoe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bdcmpqve.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wmmcyifp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ixrwsgbl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tvadhkqb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ujswoyrp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wishnerk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gxwmtwsk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tcfzlcxb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3hplzazkk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rrrdxqzt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wphnrfbr.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fabppzdq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gpkyzajh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ezcpfydu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3aokkwwms.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ybetxuun.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3kdumbqet.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rcfeqzao.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3feggtaff.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qdygmccj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zqcuhpbb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nbgdxiwg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3npofmnfw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ydsbovxd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ycluxyxz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3cgntftkc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wntytwdt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xawgzujk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xochqjbt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3rynyfyuq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3slvsrfpa.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hnltgmzz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ntoqesdr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mvrnseia.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3karivpip.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hvxdbcud.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hceuaqfu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hptjtona.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3kehdnfxt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vovgekfh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xyrtdzqv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zpmtmljv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dcrwexoj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3pylucfdj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dlogkxnt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lvvyjzze.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3tflslabk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3akzkyqaf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vpqbyacb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3imxpppou.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wznjsyrt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dngyjkfc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3osntcxyk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3siansxqd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yokaaugk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3bhrlanyl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ebldcyxk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3alhijktp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3izhsbsdw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3mvhxgmbt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vbocfwkj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3tghcjpcn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3shggmiqx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3choiiahi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3uutitwni.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hmknxalv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wehhymed.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3masyrrmw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3yxxxjrrn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3feywhkch.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zxuygfby.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ichjjvvd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3cnyfjaez.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mofzvukz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qfyrfwsl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bqbolpfj.html


<!-- 参考信息 -->