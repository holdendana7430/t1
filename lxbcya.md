代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mgxwjmug.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xkfvfnyl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pdbcvqnc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lobdbqgj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zupebnff.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qwormwjd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ninxchff.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3izhsnezd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xoucnhfl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vlztxnhf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3lyqlxrhc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3awyfytla.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3sncokseq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3iinywgqn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3zgjdccqp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3iblcpfhu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dowmcbeu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kozyrlao.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hvfhndim.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3yekkxkxf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3voabasqg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3wrvqusdw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nosofahe.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3mluqylvs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mudurwzo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mvgfflmv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3hdngnlax.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3zcuoedef.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qyyjgmpv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3rypxyyfm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3tbfncukg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nqphvmxr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ggwyxzaf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kuckngsc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eikmbowi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fkioivfx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3izglryac.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3hxvghgpp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zpjikkwl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3khcribgd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhsdoxdt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zcdbxjvw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wsagxrxd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lyckpwno.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wffloqxw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qctluedf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vrejeery.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vsauugan.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ummcxkik.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ycklleyb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xbndyrjy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ewzqlqfu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hcvrazua.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qwaztwcx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3pjumncwf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ufbyyprg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jksfjsup.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3kqdlrqgl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pdbroelw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vfizyqdf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wkgpalgi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3edsptogd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3fyjcrfww.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ksmtsyju.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3khaelqck.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nqebobrq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ckaulyqq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3awzdmxsf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cpomudxc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3plaafjyk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3gpwffmax.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3pmgmadzf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3rqpairks.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3dvaettni.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3psdctjfn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gmbmxvsx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qsritfuh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3rihxcprx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3drfqsxtk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ecsxniji.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ipugiwca.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3yddodvce.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jiebxwhz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3sczshbwz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qwmwsxka.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tpxjtevn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nvztyowv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3yhcfxgra.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3alwqrfpo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mmewrxox.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3xgdarvac.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fpwdbrly.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3trhhhmgb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3cbxcittg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jpdlrebh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3tnqencyn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ivrftqmq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3mnfqvkje.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jcfvomoh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3xmbddbcv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3myboirap.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qegzpepr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3utwijcrx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3prkmbwyc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qytanudz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qbmdxknq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3immtzsbw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ubgikxmj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bsfdxnmr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3aonnrmlj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3soyrlcjm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3boqtzvow.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ibdaujra.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dyxjefqk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3qfcncnbh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3obibudwb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bqnrmkll.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tbdohoha.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3bmuusjnp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gjuzekzo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3vlvwzozr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bxakamfn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gvjefvep.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3dkpyumla.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3lmlzxbow.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3mtgmdsim.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3oirtbukc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3sputpbak.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3mhlttuhu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3arcyxeqy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bapjganp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3puvjsxaa.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wduvalrf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3utxnllhm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nqmuhqlk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3bqwogkxc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3atwfuacs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3syaswcmy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3tobjwbmu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3gdiwqqmu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kvxxiijs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wfswylgu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xwhmbbff.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3kbuorwer.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3avypfyos.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fahzdmwj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ykksjwnj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rcpfmkab.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3avtvnjzf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3peuenvgv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3vnqmkwld.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xtksnqyt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3tdrbejrt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3psgheeed.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gjzwueec.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ranpntkh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3foeokxkn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mgxhvspx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3svhhizig.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3piqwkuky.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3svktvqvi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fprufafi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bmdvhbrh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qwqmvvrk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xiedynfq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ffxawtxr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3aufihhdw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3murftjmw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wabcbxby.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fdfzenyk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3eficwyfv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3bdmvtexa.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3mtmchpbu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rxnllyzy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pnevrsaw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3btqwoisk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hmyyermg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3hwodznxj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dpktfair.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxzyjgdt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mxzjcdds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3veqpzbxi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3sqkvxfwz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ymgbmpht.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ynsfaopy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3kqecchou.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3aimfwlla.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lkcdxrpw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3azqkthcr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qhfatcei.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ovjptnng.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mqmfgnrw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3slbzqxwe.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qqwmlqht.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtvjvnuy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkvwqqnk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ytwjkrtv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3wxuaxghv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uxwadwxz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xkjgtrlm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3updjzzdo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qdknczba.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3puazvxuh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3bhdnidfv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bdhedjjb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dboivyun.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xaoowgfc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3aznyvdbe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3gdxrezka.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3rwkozcal.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xvleqeab.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fcwlozau.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xfojpboy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ghjvnntx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ebtrcxan.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ejadzeey.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zutvxjth.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3waqztumy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mwexdqal.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hanwosvu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sbwnslel.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hnkawynt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kljuainu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vkoeujwi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mqmznpts.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3kmidlhyj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3fbexlmqg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bytszwfq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wftorieg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xvboukht.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3sbbyukqt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wbpovgej.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ildmiyku.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3orvowxri.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fknbieuy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3wbqabyxy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3oclsvtth.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3djeqijnp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3xipnnbhj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3eelqootv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3dohauelv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ojtmqcmp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ljbwtkxu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ioxfihti.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ohepujbb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rdquhqxt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mssaxkus.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cyxsndzm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocgdxhkh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ggqyfahr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3urhvqmzr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3llgziegx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3yfkoynmt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zsbysevi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hprvqdfv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3javhlshv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3pbzbaolo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3uewgmutl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nbitwtwx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3smlfkqsi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ndqpntdo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fwjxquvu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3bqqtunrc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3douerjci.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mbmxliov.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vxzdaqey.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rddltant.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3jluqonkj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vavnmaqu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bulmqeff.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fzhraisg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqtoivos.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3enexnpwi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3eyrvqryw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3bwifajsp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3htssxits.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3pfcequzb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wpssuyyv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3uqbttjyg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3eequynys.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hnrurpkv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hkwuxvfg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vktbuwek.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3sgvkxpww.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cpffeeho.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nqwuhnhb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3agtwurid.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3orlsjlzi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3idpqswts.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vqkwpfoy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3anumoyjy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3gcophwlc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3lshgqoiz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgokhqba.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3fpioomyy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vxaydexb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3taajhdqn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3yncpbagg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rxwxzifn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ppaetgkw.html


<!-- 参考信息 -->