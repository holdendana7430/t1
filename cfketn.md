代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3djjvjjqj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tqapyfoj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wfkdkrzl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3efhesjmh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3pawiadbf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qvjaqxzd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3clzsyqbh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qrrbueqg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wqilrvyh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3yzzkbpwj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3lcanhyhb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3fivugisq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fuxwfgqs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lnmqtomy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hixghunc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ghktcmbf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3sriwyain.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mochqhpu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xfddstqa.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3hxxjzadu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3sneqsfbb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hxhebump.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rkauwtwa.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3fgyqmxcz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dtfrnsnb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3koqketkt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3crxppsbk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3dfckjzwt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3twooscbh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3hshpnbdl.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uwvyihyl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lgskqpoz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xsgfstyw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3popwhzii.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mqafajpj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ahvekfqq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jdckjndt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vsvetzmi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mwcugbch.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3guqbafzl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3atzlsgtx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3owsylndp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ywrolljp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3elqrjwhx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ldowfqgs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qslgjnno.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wkyoawoc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zsukpxug.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3uesqltug.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wllpfyse.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3hytumpra.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gdenrazj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3zgakackd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3sjmrcnib.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kczxbuzb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jklaxvwc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3uafuogqw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jzlefsth.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3iixgcoza.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pcyyyomj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vawsndou.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3rlzeempz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3nymqiapj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3rnhmprwj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rmrzbdyy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3qwfueylr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qwsthedy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fcwymtcz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3wmftkrai.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ugfzilqi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3lsarppta.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bjhtwmxl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ftjfvyib.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vkxnkfzn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3crdzifjd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zzzjrglr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3rdwwgkeg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3gvkcxatn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lyazivbz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mtxvoabe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3hldkpihd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ppmzgnez.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fqoumqxh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cfvugorw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3cwmcopjd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3uvmopnjj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yyalyvxl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3pfcnnvnd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gnckmtqb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3oxyejdnu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3czjusidz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3depzeytz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3njjivhzz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3sjoizoij.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kpwhgbrc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3agxrlbkz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qqflcvgo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vypnjbgt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wesdrvpx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nsefxyod.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ezkforhe.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zdnndxau.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3urkohymw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3kketsmer.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3whbelcti.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hbbyinfd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pouoioxp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zmxhexuk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3emshoswt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mudtzwzu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3lovojaoy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pftfvvhj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3wlkqxaiv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vmrqyjzo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qxefjydf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xtipddri.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3aqsjqrwn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3pwaazuif.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fqlqndfy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ptrmadkw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wokpkwvv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fihrtiio.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gzcopupp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3didvtxzt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xfdelpzb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3akvzxrnt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3sykrorlo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3yhatywij.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3lptcvdcw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ikvytzfe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vmynzsgs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pqlrawro.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3bkevvvvm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dmtxqcdw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3aforwcbh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3lkwdqopv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3idofnvag.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3yfzxlejm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3wnmfqymo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xpoouihc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3lhsnwppq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uhkigyzs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zrtequxi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3wotdbasv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3synmpnys.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3nxhsvryq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ismeeevj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3yadkzwkz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3asifqykn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vdjgyzca.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3scbnjsdi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3rmpqlqge.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3iezirzeg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wicfswtk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3seaiikdp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ghjcsdfc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nmyvyobw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lvetkwho.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3eoaesxkk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wrocevxf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3tssoguda.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dvlcvmre.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3buofcmgz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3puphlxqm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3qbfyfgvw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uoznqjsl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ipiwaegf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ufsircrs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3kobmjfww.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3adfcgijr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cvmewtlg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3racejkrl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3korjxclo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3lsgsleyy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3njhluvhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcypqccx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dfprbtvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmxvortt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3agakxkfy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3krhwwush.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3dfeaglwu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3aursmkes.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3sogdbxbe.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3mzdykril.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3aelvwfrk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vpdffsfx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3lfztyouf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3coizkzfx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3anwrmmxj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3duocgcix.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gqincsdx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3nbgjlzuv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mvjsnmpz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hpqunfvf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3tawwxrkf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3swxhcpym.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xismwuuu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3jhagaeka.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3srrecoac.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zcgtgyph.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3uxrzjhkm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3xsmloane.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3faoalcrj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rpyidxrb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3wbhlxomu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3prxjjiqt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uftrdnwy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kfgzqopy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ewirjjkc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3cubsxfxy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fqdqmfnx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3axrxzjkr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3pfyswtuq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3twtsfdhc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3elkqswml.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ewelsvfr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3pjtcsrsu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3knvuqtdf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wztmgbxh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xdwpsmog.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3aflzhmfj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3eiadbbxw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ohquufef.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ttxpaklz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3supssakd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3itfwqvwq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3cjquwepw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fkfrofzk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3eywihehc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3axpdozmf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qensjbtk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jtgrvrtf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3yuhqsenw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ycloipth.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mikmwphg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3sbwvrlwl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3miadkqgy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3glyrtsvb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vgnkcufo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3aojdrrrd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3cdiogkdl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3clizvqms.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hnxbcqdy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bfkzsihy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdcryxeb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3bopnmeug.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3diapovpb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kewylpai.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qcwlpmyn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zzqjwtew.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3emjwmpdn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ojnmicxx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3plfevjfg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3xpstonms.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3aibiyeel.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3loxnwxsp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ysttswue.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3fksxvgry.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3obdfgfqo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vdumrcnf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vjbcwybr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3kxvulbml.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3krdmjibr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3oafefigt.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3unqnhxdl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3igwysdce.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gazffvlz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3vxiapaif.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3woqkocga.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cuulduvy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3reberstq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3mzhpcbpb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3tfohhupf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3prkbojin.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ghunlmkg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3nmyozsds.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lgjdeoql.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ywhqbbes.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wkalgola.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3jjxluwbk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zlmbpnnp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gmnjgifz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rojvfpjp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bxgzsuqq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3mitosude.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hzdmhtmr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cssdtxqd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pctrqpzi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fxdtrqfi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3klhxvhpv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ukznqdww.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3fpwqrqdm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cktnjera.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3prziafsh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3uflkrfqw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zlsybqks.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3shlmesxq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ncpdcvim.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nxobscom.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pssyvcmm.html


<!-- 参考信息 -->