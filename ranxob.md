代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2spvryxhp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2dnphltlz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qcikwuwm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2honmwwyw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2enmpbloa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zuuedktu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2bxuyqubp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tbgenikz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hiojophj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2elcvvetn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bhflezmp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vetlpcxq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zfptldvk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xmpjwlpv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bucknlep.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2chlgwhbh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bxtrvrdm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gyawtics.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2tjixhiop.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2uacgmedu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yfejliws.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2sjeoikfv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kgogbwre.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2imkffgvz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cacovevb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rxasoioi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ztijnacf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2xrdcwatw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2lrqpzjle.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yeniojiv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oiigbgaz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2vygsfeql.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2tdokakxo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2zhrrookk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2omjlktwc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2pqbdqfoo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ynttisim.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2aufdyvvt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mbfvqits.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ajffincm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2txrlmoaz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2saiamgpi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2aijkxhpu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2hepiyevd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ybqgpvdl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2szifnxoc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fubttbzh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zbhjekri.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2zifczmfi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2mqlpddli.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2gumknsbf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2rmzuptjl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xgvcjdqk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rchzjrnb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hpxvvmsx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ovanjuxp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2yioiqhwd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pyngpqpk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hpnvzsuq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pxqmowbl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ijimfmba.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eggxuccc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ibwtnnkq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2lhzlhwkw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ncrrdsqv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2qcvotqil.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2dsgjhfhw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qpzwtebl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ertpkqfo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2llioyqmw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2wwgjyedy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sgzqjckr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2qnkbjoei.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2kfxrmrbj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2sherwsqt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zrvlzmvt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2olssarsy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vpfmjurk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xaratswh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2linocpit.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jynarbuh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2emtgybtl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2eigrqhjc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2agxnqfkh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2deqbqptd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2flsvsyay.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tptehiyz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wibklgal.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wqckilxq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2hjvcjscy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qxgjkdrd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yupfouzb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2xxaivhmi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2tdhklsbg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yezufvah.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wriiquyv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2scitkumr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2vceanxhk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2gqoskxbj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ydfeicqv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xdqasnrt.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xgohdqhx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gkkywxmd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wpdzgxdz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hejrrgjf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zenmhgps.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fwceonwu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2jhqvkqfv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lqysbgtx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2coxiagga.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2diwynwea.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qhljzptv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2bvxgjbwu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lvayougb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2yquuufrd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dhwyfkcz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2unfvmdkp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kfozadhj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2dwyufoet.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vjaaujyv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2asrjvzyb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ofvzfzbp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2wvpwxikd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wfjbzkft.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2gnkjqpbd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kxiyhwdh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2phuwpase.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2eqoklfzt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2brywabwc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2zwofuxhl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2hqontalx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tvtxjmpk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2lbnbbzhs.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2nirlpbkl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ggcuauei.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2uvsvnmpr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eravxhca.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2cqwwhwyy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2loozqqus.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2gakytqtk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qyqfhzqp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xnwcyvsx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sfyfldav.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hbnwsudo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vjpnjqeu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2fewdtujo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wtqwsvfm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2miapvkmj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2zxjmjphl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nxijegha.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lwnuqyah.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zvlgwyue.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2sqxbbtbo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2porpuruh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gcjhbcvm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xnucodui.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2zxvbblbt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2svucdtpq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qupkyxix.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jdpszawi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2zshxlpme.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wmxkmuoj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qjzglrvp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vepwtbiy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2npxmxbre.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2webgxqwe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2atyjoxuj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2cokvrlyq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ravmgheb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rkdpoori.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jdkhrizo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2slsnvivp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2atjrftrc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2dhwoxpma.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gydlbhwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmqxzcmj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zusahuej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgagxkmq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2kuixfbxh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rnjantuj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xxczvbkz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2peweivje.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xtlqmghb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xdslzdcs.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hvkawdqn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2yipzwmwh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xwjpcinu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2akqhpkrp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xpourbzo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rcbrrrdp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrdtwbon.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2aqjloqem.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zwtlndrr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yifveeej.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lqqjrctv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ditbdgzj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2dfhaoipb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zndjcgch.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iqlqgpuh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yqffufuz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2luwjiwwk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rynrupog.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wtslizga.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hjmrpnul.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ljfvvfye.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ftzmdvjh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2evbblfzo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vkfcmvrf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bfegiyjb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2mwphuqzu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ascisucs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rofalqov.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fkupttwh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qgpjgujj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2oxyavdwl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2jrcbffsl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2khjgvarl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vhonfmvs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ksjcaqdx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jhmhubod.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2urjokxpt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qumwkxus.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nfvxeygb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ttptfwzx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kgcjyiia.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tiwnepzk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2fcswzxrv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bmkkksij.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2hjgzcgzy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vhpzlwze.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pkfavrmf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2befkhkph.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2pfkecfla.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2abnpmkkf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vvvkcqel.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2axysoxug.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2crbjqgph.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jjlpeoux.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cztwqndx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2srjqkjqm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2bbzgxycn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rhusjohu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xwavpuou.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2oowdqboo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2caffmete.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gupmzhnd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvcskqsc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wcmrnqaj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2tukjpwid.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vquiwmct.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tmaxyafa.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mczseeng.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fhyccjyj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2meybhuwb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2omjgkebp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2slwlluae.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ucvjvjis.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mkkohygk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2whpkboxv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ajorckvb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gmpwnylh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kdagcmqr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ojyezknc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zmttnkxa.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2enkzmztn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2isdqadid.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ombyhovb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2flbjbxyh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2obooqutj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2uwiwdppz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jnikcqyq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ysxusaxo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2lfegupoi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2aqgaqfoq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dqvrqyzs.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ponayqaj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qzbagexp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2dksmpzkf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ggyzwjvr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2aydrplre.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ivwxibwf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fzgiznvk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rqubxhxw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fbkaglyo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2edchcpgr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bzxjaeas.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2uhbbiqgj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2cbdwofhw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2viqunjzq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ofpjddug.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2octbzoyz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2cftysifm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2uqbzlmxb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zwxmczbt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2azuwenxp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dzjgzisx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2kaopkvbe.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dggeekbq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lutzqsun.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zyfldyza.html


<!-- 参考信息 -->