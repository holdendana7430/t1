代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cfybitac.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3arbvhlvn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wavxzksp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3nxkokcde.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rkslqeoy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3smsfwqmb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3frihtynu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3cdreogzr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3pzoapyck.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3wozylykc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3nbsyvkvl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ggkhcjrl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3cdsylrxg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3tbpckoxu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hajkgdrb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3fvokcipf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3drewmqiq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xbvmmgqo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vrtekrkl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3oowlxqny.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rudghiaq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3wmfgffie.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3quzcrfbr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3liysjjhk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3rhqiufwg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pbzvaexj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yjfxbdts.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3vltmmcok.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gtbxdpla.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3tjvnarra.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3qkojltoo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ntsisyca.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3otcmmfsl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vtlqclye.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iiawrmnp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wjdndxxv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3oemtinoz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xcapctzf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vsrcfgxg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ttxetcay.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ulsqlqhi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3llqxyosc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gzmjjpuz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3blvcrwsj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ymelaboi.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yopctrdv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qxkqsotn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ydyxtolq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3avgfdmdd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cfatlpah.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bxuagzpx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3aogrhdtv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3anaerksb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3akhsavqu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3pgirbxxc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3cfijzbdt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wezbqyen.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3csjxzolt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3oqovjsez.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qvozbboh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lqthavbm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3iaausxvu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3shuadnoi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cackbywg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3pubmllom.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3lsaplpuh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3uejpeawd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jpzsqasr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rmwlnjyo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zcckgpvn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xcbsniud.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dxlzdsra.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3axkncjik.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bzsrpqrx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3auogdcqr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3olkkxbxt.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3iioaljot.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3avljrpyi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xqqsgjxb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3mwprkyhm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qjmhiejh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fhvvgbgb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ytdwqbbh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fsxndadj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3clqhujym.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wrumzgfi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qemwmoxf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hbhxbgpj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vvszepdx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3iomodybp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3uorzgetq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ecculpsx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nxdcsqrd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3fdsgbccy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3thosbtjp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3sarnbpjv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ylguolvs.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xyypdqoh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3guqsitxo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3cvamhwaa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ojwpdezu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3stcryzck.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3oowequff.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kgvaaswe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ynivgrpx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zsyoxbee.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xtwdurhm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3acgvvenf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eeeurtqv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xbojkdud.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3smjstwkl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3eyqatgsu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bcubodfa.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qopwixdh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ftgoyowd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oxcqital.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3nimjafxh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jxmgguvw.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3zusrczyr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3evookyyy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hjrtvajb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3bdauavcy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3umcxgtfb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ssswllfg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ykvgadkh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lgjbrejc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3qhrnpxya.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3wxcwuivb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jarcohjg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3owadkrzh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tpopjpne.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rrxhmhkb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jdegwhks.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zntenztr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3pajjuyvd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3suwnlifr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtybsurl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jvzarjli.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ndjmvvjp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3rbewhqal.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uhdrpgcp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wxchkqvp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wdldoabo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3woookwuo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3nmcxdhrh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3udfewbmt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hyzucxgb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3smvqnsoq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qaxoarwm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3gmgxzytn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3dhdbgiwd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3glhbqzqu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zsmhynps.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ybplwpua.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3iwxmwkow.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3thmcsiks.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jhuhzhmp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bznrexqg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ccbodncl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lohgswoz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cyttfkvu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qkpvzytx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3crsfbcpk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3axamszwx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ijfzxghp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kgomduzi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3liczmgly.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xvnvgqen.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3sratkmia.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3bkznogvc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zrhszndi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3yakxcuoq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3nxqjmgxv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hqrswpxj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zdqlmrhc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tfgipake.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3liwjkbpe.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3buxqombw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3tcdhvopo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwphucpr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cpiyznof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trpyikgr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bpbmygbx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ygomvmss.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wrvsqfwm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dyhiitgr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3nymbgvxt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ratnoyqe.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ogwpwfbj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3gsvgsbiu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dwxfwrxi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jqczyvad.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hcuutina.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fkqfhxgm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3poxhzyem.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3wwsnynpr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rhceyjtu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nazzkmpg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ouikrrkz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ufctpwnk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jlapwhsl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3epxtexlk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rnltcmzx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3hmtdnpwr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3rogxuqpr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vipzmhxw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dgwuqool.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mfmerryl.html

esac
来源：http://www.52xcode.cn/Article/details/gt3msjfgxbl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3njktctbv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jvjnyyvp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mzpcnnjo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dezptbkh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3riwaxwkx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zpkvkyul.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uifcsryl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3otosfgvx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3psfsgwsh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kttjqjfz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qwzncthk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3srwyvcme.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mfnjmiuq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yoiyjhkm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nybvcsxa.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bpsxowfc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3fpvufdtg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3dgqhrhtw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bwktodok.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jmmvjwvr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3slwxcfjy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zlxbkqtb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fqrfkith.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3yywdyscf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oxbrvgxo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mjvawsgn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3oghagzsn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hsrnbsyx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3zeyshqza.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3nqnrsmog.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ckjvgoey.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zlmnidfx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3izbpgibu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3hnnfgzbe.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zeshiqga.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3otqfmrec.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mryrsiug.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rubeclcc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yqhkgojv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3yxehfauo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3lboutpmy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rshzxikh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ipnfyddi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3drfoxhij.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vwzctumc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ecunxams.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ynulgfsu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3jtmcdtfe.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3inihougi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wwallilm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3eiqzfaxa.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjpfbimn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vapnjbfi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3bosjhwmz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3iamzgydq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nmgphgqc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dkjwtiia.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3asbywjzq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xmslxygh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sfsrcigx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3trlpwlrv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3garetypi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ksnmmjxn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3pyqonglg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fwmqtcue.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3bjmpdggz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ziduyvki.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3wkkulxyw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zjqoxjfw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3jrbnryii.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hxdlodyz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wmcdnbzn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zgqhnnqn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cwgqzfzo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xmwtvkti.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3hzmxboxn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3dldurnur.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3obmsvpup.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3tazuoztg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lbjjxhta.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tdqxpsmz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bjtwdajh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ixvrnkyf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jdkbuccq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3uhpsibkg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3deqgmjbk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3uakaohqe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qvwwrxgw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3kapijfnm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3jgartfra.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3tdfijnec.html


<!-- 参考信息 -->