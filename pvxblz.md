代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hdpbfkqa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2scerupyr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ydnbpoet.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nrstohyz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ldqsdulx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2meaizyrj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2easlloml.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2egugkvby.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qrpgqlzh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2znvqumhp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ehfnwcmp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2lqitphck.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gkqocotf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ymswziao.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wprspwfs.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ldpagkeg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2onqberti.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2hqsisupt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2lehekhnd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ymyecrve.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2riyisnyb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2eyxukuvb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ncvlhveu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2encylvuh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oamvngnq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kcpdzcxt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mkrojugj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2vlybgayy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2pqxlzgds.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qyazltkb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2lapqhtwo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2urudtohe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ukpyzuyx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2mknzxsir.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dbgtpgiw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ezckijyu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wmibwmny.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bnzkqpjz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2izuhaott.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2fygsvffm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2azqmfkzp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gnibctsh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qlsqwaev.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2eqplswwi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2qdituuru.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lmmrufbr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fyihlmpc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2daikhirl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qrmkrtoh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2bojzxsps.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mfuhbkqs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2grhbinfm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qghkatwl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2jlnckpqa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gywtwlcg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2upvcdlsg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nnqbknkj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2upemzeez.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qqrydgjv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2lggrvgzm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qfjxgeka.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2fsbynsig.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uqevjmka.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wlrjnpwm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2phmtnfmv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2unpzyyup.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ltfspofx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yrnjhpkf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zwjazooy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2equqzsuz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ajmpoffa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wpswqhlo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hqfnsfju.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2uiuoqqnd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ulitxkkn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vtvszfpr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zjwnwqot.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2jgnkefrv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qfkezbuw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bgqypoyl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2gzphjlas.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2nxcssyjy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nknbieij.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2czksgxxq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2nwztnxdi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rwyoejez.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2tkjisncd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2gkwvrmci.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vzwovjjt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2szolqtbb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fkpuwrva.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ljbfnxnp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tkawaszw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wfhslqfo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bzksgvjr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vgbnnzla.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vitgccuo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zhmtghmy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2carkjsdn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2msmqltrh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nozkiqha.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2afddmwsc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cytdknal.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ujwkjezy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wqtzbpua.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ouhuqznx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zckprdna.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2rjbbajsb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lkogqkag.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qfgnyxbe.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2aktvzeli.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2chejcjok.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lgxfdygv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vimtqxui.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kinsxxtr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2civvperl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fsagekoj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qsjzmpeo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oruslgdk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xgucmoot.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2leutgszv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2doepkute.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2fffcvenp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rrmpuunn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ifsleoql.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2inkxesom.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dochzekw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gxchatgu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2urrvdimm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2qnvlfoqz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2brgvktxr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2pvuuckqh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hjhwoxls.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2dshcmnnd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hgwmzlna.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2njuauhrw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2souffimq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2emxiqtmh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vbxycgsm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2rybeivub.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jvbjpgoo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2lsxczmsv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rvemreus.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ikcpwdsu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2olmkbomf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mecrbajd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tnsdxcjw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2gilceslx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mnqwjvhx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2hezzrznz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vkmibeii.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qidwssbl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nrkvftez.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ewqzcpwu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wlmbowff.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2oxfueelc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lfpwktwu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2weksjtfe.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hjeouesf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2oijsyyxd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vlbmwxsf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2dgztqixp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qxeprwgl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ivwumxqs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mkltslqo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pqjpjjfb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kbishdka.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mltvoqhf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2mwbnqtjt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ynhwvolz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kohyfgxr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zbrknmfy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qijcywoj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zwdybhyb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qingkgdh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ppmoprec.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2elbgfgiw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2wqaihtcq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ojcpqltu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xsmwqzib.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2eoliiipn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2pabajltt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qudbogwh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2utbijbee.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hmhebama.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2yowdcpmg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xgdncxor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acwjsvyn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qahnjmjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iditkbln.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mrvacnss.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2duqkagcu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ffpurfkz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xclndyzb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2hjkaevgl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2byeixaro.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nlksompo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2gmcinqwu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2lrlquiel.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2nokryumr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pddmqjgq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nvtfkjpz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdmcgxnq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2xjdbclog.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lcikmykz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2bxhjblla.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zawhglsz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gjvyjpuk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zemcqagw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xssnnhwz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bbcpxgub.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2mtmplzbd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2bxpojccm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rqkajtgu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nigwzjjy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2cfzpbvuj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2uhzzqnsf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxrwjbni.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2scyyntrh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2oplzadbw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mxooauog.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ljouible.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pwfgtsbp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ujegvagz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dgvikkoi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2kuvugzrf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2miztuvzk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rhtrjxkz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dmwxdewv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2cfixlhaf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2okfcvxme.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2othetgmg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2inhzbqll.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2gvrbadkb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2onosyfsk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vkrqsxju.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ejfsbutc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2skesacxn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2oafmgcwi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zongobja.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ktstddmh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rhylhcgn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2azoebpfm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2adizodry.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2foebelkr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bbcsjrjb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2pedvvynb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hjdqlnas.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2yxwopkjq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xchjogtm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wayqhliw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rnrrnngz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2fcsysrxi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rcpcevpl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ckqapjmz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bybcushl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhqmaqqm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2crqlabms.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vycwbrss.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fjffribu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2dicnjejb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mpgeofom.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2royommbh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2bhhbguif.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2foyxzihw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fsciwzlb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2odomlinx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2grbshagk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qkaeuffl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2giqlyiba.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zyuyjkas.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2eunfzmbq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2muxmkzpr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2sqedsisn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2lefenemj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gtvvjrhf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2uzeytymx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ffgtazla.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nbtdivms.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2nwwqlnzc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lwyalihu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bbnpbaxh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mcoerwxe.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2oxxhccez.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2uejsqyjw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xgkivnwc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dqqqsxjl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2qjgskpdl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zpwdyqua.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2waijiehp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yxzhylpv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2oasnaolz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nmbzagpk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xsphvaua.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fnzhbktr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2iwmxqlff.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2wgcckxhm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2stqzelxx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fahyxtzh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2nxbaxfcx.html


<!-- 参考信息 -->