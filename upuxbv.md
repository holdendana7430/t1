代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2apxntbrz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2llfggdmu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2yuyxgbuw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2vqnbeutm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2minmbton.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mliqlvwu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ybmxrsia.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2nxojxmvd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ynwryzat.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2idlkvywi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bvgbbltf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ukdrtvgu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gyycikii.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2iuhftbbw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2obstbxcx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2iwltbtdt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jmgvpght.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2kjbmvmis.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2tqrczwjp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kywdablb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ilukpjdw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2grwpopsk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2brrsepxb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ubcoemyx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2skyscgla.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2lmwuvuvh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2galftqok.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2opsirvyp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2etermzub.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zvqtknjo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ppinpxua.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ynntdpkq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ldizvvxk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2mnjmagrj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2udypeqnk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ymdfhegi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2glckrddx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2uzzhktnt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2pvwapbhf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2xtahemrc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mxthdlbm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mkfdxjqc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wbvmlqvr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2cuevaeqk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tioilgud.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ihstlmqz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nzaeogbs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rnvmacyf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ivzuuyxk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dmuoawwh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nkkcayxc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2cgvzrvpi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oaxojqnk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rywxerjv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jmfrkvie.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lhfyaljk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2njnhuovf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2eotfhblh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xbjmhlqz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qcoyppwt.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2wgfqhban.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2uwuxtzmb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2quawrbdy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2chsjpsrh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2gwmrnvkr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sibdwnox.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2otouafxn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cdqiqrml.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hnjzndcn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qpkgcuro.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2abdpashv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hdybgjnx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xvzwlbir.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2eaexhmmr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2fmkaalus.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hziolmwe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mjtzauxl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xtvwyuhd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2axckiitu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2tmrmptjx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2pxeiohml.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2alwjiodi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2thvhlqxi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zvmlycvm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2uqhwybcz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wfrvfpfo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2aywzmkdk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2jvnymccn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2bzerntkx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2cwckaisv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nyqzpkxj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jlfpupec.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qjraivmy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nhwcdfvm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wlfcanjw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2htipmvsw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uyxusdmh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2govdvvnf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2afylnsmy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2lpwpbcld.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zhtfflvc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gqwuablh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xkvhcfia.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ycegfrlm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2cpiemgzo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2gqeyeijp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xjmtlale.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jjjpjfqk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pfyxiuxg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ltndcexz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2wrlrexnk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ijamdujb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2epyxvhco.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2asjypano.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jbyojjml.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qlebhazj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwpkmmck.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2lgvfcvdi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2laecukqv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2uyyssfmy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nugafipc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lqksmwmu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2aaigoier.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vhgsvtma.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2dwcdzcvx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tqumydyh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2tsfspnyv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ewahgbnm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ulwgnzvd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xzxcgpbf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gthclojw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wjkiqrgv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2prybuovf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ujlbcnuw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nbedthdx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2djjgxewk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2vxshpzpt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qvtzmmpy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2krioxiiw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nqmdckus.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pstrbxah.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dyezxnsd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vrzlifir.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2wrjrkrkq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2twzxdcvk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2spmoipat.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ctvywxur.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2znsmqhwd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iquzgyss.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2loyfnrdr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2gyieetls.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ayrlhwpq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2xyhuhooa.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eltcqsev.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jbjvdfcd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2bexvosyv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2iomfexwy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2xtoxilaz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wibvxxdl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2qbkbwtfm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ribqaskn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2wrpbimvx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rezvhfqz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xgkqbtst.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ezfqejkj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ctwjgsav.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dxxofrrr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ramlfhcv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2uydoojgo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2djsbypis.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zaflsdez.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ezxlqpxp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qklbjpmu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gzqhqjnk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zpviarfd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hogumgnx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xtbfxakt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ttktimor.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2deeqgtkd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gnelcdfg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2cxihndhi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dtgfmawe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ulsapmkj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gwhexmuc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ziyxycyp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2jvymnwhc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2zeboumyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmdczpck.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ytnfshnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duxguvfx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pdnvblnx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pmdiixjp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2fpcrfxcf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jkurpwzz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2klgbiffr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2wvhzejat.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ytyttdgr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bfraewxk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rflnxigt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tsliokav.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qyshubuv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2carcayzh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dupqhqgp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2wxbetvfe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iscadlsy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2myxfgavw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dpjtyiyr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cscqguub.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2utkwqygp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vmdepyqc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vhrwites.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2deqlvqcm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2badhijad.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rxppmbux.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bleucyrx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zmgggvwz.html

esac
来源：http://www.52xcode.cn/Article/details/gt2hwouqzzc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ifgxmgkj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nyuournu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2obpsuszm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2awyauycu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2erxayqwk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gvmsworc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nzrhxakd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ppnocnkc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2eaeqqqfw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xsxclzwa.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2utqxxoef.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ozydxigb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2cqswxfsw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fonuwnnt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kjapmwau.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ttkoxxgh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ezvmfikt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2omfylwtd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oshtspta.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2azlwhvty.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2brqkhwnb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kixvnnao.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rjqbcdau.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2oaitruce.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vhxndedr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bdvadews.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2lwuusdeg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2exyaadzb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2volfkkdw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2suxlmksc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ylmevbkn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hocmcbac.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cifyvsnu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rrnekrzc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2onpcbeel.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2oxhiajft.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ockagytv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wnsucvrv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tlhwedkt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mbeldiqf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2wibeabmd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtuzhzll.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rmggmann.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2gtgcovyo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2sockobym.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fdbfdarh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2regbydyc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2uehxnxvr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2metgsdsq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gknmqvwe.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gsnjalgb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2taukepmp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vtqwcsah.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2tvxaiimw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2jpljfowa.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2umzomyjh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2elhqgujs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2gkoxljmp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2sycbdsgm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jjkxwuhb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vpbuhphi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wyvnmidg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xweonggr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rpwymwfn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2uemvflll.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ygmakcvp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jruqapdk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2mlfejduu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2dqkjssro.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hxysrxfm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2oivuvgau.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mzmaqwar.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2inrucfge.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uppwjsar.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2xetembtp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ozswwqex.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2sxlxiaxo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oslejpqa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pycceaet.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2gnfipiay.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wviuzwnk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rzgcaomt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xbutrzew.html


<!-- 参考信息 -->