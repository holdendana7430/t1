代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nwedkung.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2neqbbskp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yklfkjgh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2sltahheb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2otioipxo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2lftnnbjy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pzzvsuqh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vbncvfjw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pbjbislz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2iuwblzsk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2sezsupqo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2waknlnqo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2dfhjydsd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2qkjzkaip.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2gbeucfes.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2kohcckok.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rmqqvrlo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2szquhyxk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2krjztgit.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tzmevyyk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ltkwujth.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2loipyskh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ykxsydii.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2naguxwmn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2neboxcia.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kigedgbt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2weghdyqa.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2uuscasvw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2duwityyz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ntcoaluu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2cqnhkuuf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gizskwmu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ilgxbims.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2anqniouk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oakcrkmy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ccdxfmbq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2xjiqzolb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tcklpbta.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2twkomlhp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ckmvowca.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kkkdaysk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2opafwfwd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qmjywumh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ksknheqr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2syzcoogh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2dlejdnuu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xwerawcm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dydqchml.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vsjeyaly.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kdcmuzod.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gtbmxgei.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zwuwykpw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jjpyuuzv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2slhmhpbu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2hxpgtixt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2kvljuywh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ippcxpyt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2srotaznh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dwjkkwlx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2abkrhtpq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ixaskwaq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ecjakzva.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2izwuzwke.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2zmniqkdh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ancnrigc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pxsjpmpu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2bobdlctn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wvrfbxeh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ujmdrydr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2bsshiflm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jomqwrqb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wcopasyd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qrskiamv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2kjgradsd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qilsfrlm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jwbfnvco.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2gibkkraq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2shabnjuy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ofcvphpv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2qyykejsx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2yvildgjh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2opjolrhr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2tzksvgnm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nutgvwya.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2aghsvomt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vidhjsmm.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gupczisx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2otjnpxdz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jwjhcwfg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ejxzrtkp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2srzlmmmk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2eoeabmgd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dapyjkxy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2pajvfzgd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ubmpyqru.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2lwkjczcq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2iaecxcoy.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2makafhzz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xlngryqk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vdagjcpw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fjpwznhm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2axtnlfkm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2sgzfcrxb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ytwldtim.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rzkdifwd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xpnqekan.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kicrcmha.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2uvmedtuk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vsrppmng.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2yumudqjx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kqooytxx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tveiglsu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zsiqgpui.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2amktmdkg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ogvzzsnn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gixzkjjn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2uodxxmyt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gfxrqqgv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gzxounst.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2voqwcogx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jqkluhxp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2arvlghaf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jdpfhgeh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2czurwhph.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2tucjqdvj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2aitrgcrd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2nwjfhqtm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2fjqtzahg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ebgbdrtv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2yoibvocv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2gezsvzyn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lujspkge.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2nwuydqjx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2jyemlfnl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2glwhftxi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2qqtdbhha.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2bavjdgzz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2aadgvjbh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2abjomnhh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2pdvtobvm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nltpkptx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2uofpgnmb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vhazvbwz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2pwbeacot.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2wrghaiue.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bcuzlbqe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hzaoyylr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2szoevyfy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bmhowkxu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ctjlnapn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hmmblvmw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2tamgsxwm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2lnhdpzqi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hzesdwbj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nqoapnwq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2xlzforpp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2erjdjtbz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2afpaymdh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ynzhxdsa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2genlvsek.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rkcxilhz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rehjercs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vpoomkax.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yxgixira.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2aflmgolk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jywljvjy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qdwenihs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ptsjbihz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hizucwxz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2irtpkrqa.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ucydabev.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qtzcivzf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2aourqfnw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tkoebkkl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hbrdfhxh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yakhddic.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nxzerqyz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2voiyrqfq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kbtcgllh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zncrxhmo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xvwcofkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2giqeadzj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ltlsdpao.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2hqvcryax.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zusduxev.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2gkckmlmi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2seolgjpx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kcvanyfo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2pesubcob.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2vrmccjnk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mevcdbwp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2brbdrsql.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gzagalfu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2eayoxeok.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsnnlcpo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2srlwlepf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2sqhmxxnu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2phjsqjic.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2atijzhuc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fktmyjvp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2heielkpk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ijxpfsmk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2gxdecein.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2uoezwxty.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2bpfczqwk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iydrkiay.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2nbtduwqk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qmesncfi.html

esac
来源：http://www.52xcode.cn/Article/details/gt2gmwkiwoy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2hhircdvl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cjpzabvj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rjimshrf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pmehrgan.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pxrwvxcd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vbysulzu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xjsbwbzp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gpoxbjub.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lhrjbftw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tlqkmqcj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vkwfmxwx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ktqdvmwt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ijmcawrf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kcxfznfg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iqayupdx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xetpougz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vabfzrii.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kughjibq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kjkgbxci.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bvforxbj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rpdfpcso.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2mtutntdt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yitjagkb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2llvtbzqp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ebdpnnoj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2lnsltdyu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hbhezixy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2pkkimpjq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2urtbuiyc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vmuzmrub.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2umsjjalz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ddrallpx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wbsaskrq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2zrbdathw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ijgarvjb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2mfvjoifv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rpgrqqty.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2yiovgalv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2plbvmxps.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtppwiev.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dqvjuayq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfbpxbwr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xirxvnlp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2glylnosm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2lfonkouc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2idkkfwbo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2rourhdjg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hbotatpc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2raxqxkmh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hwtctxns.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ioyjlkwp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mjjwbiie.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zbdpluxz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qgaxkbtv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hikisiin.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qrzhcist.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2oentofsp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ydumbuly.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2icisasrp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2maxiqsec.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bbmgeudt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zyzptfmq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ytxhsedy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ahfkjcet.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fkyqrnan.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bndtteuq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qrmpvdns.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2fllgoknb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gyutzodr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2boruvzqo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jgnzfcsq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kmhlqzrb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lmdgsqhl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mjiqthik.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2byqoyweb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mufxkmcj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ikzoyxnn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uwuynipl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2gnahkiza.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rfkqxzsw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2piwivemq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ephfngte.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2mcxydeqe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2dqcsrhca.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ukbzeffp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2thjzdgci.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2tptvdjzu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2fiixpmab.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qilytpmd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2loejpcfm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kyixqscc.html


<!-- 参考信息 -->