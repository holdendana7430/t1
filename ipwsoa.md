代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hahyjizo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ngguegin.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ysgvcakc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mlvvnsoq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qjzbtwwy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3djyqblwq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3fyafhirx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tqtpzuuh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3makjexne.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3tcipngdk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ndonyhzr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nplxreot.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3urnxdwdl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ilsulxiw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vixyedsq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sqloicrt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qusczrty.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3wufzvsok.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3chblyagw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xkcywrxu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jntvdwfv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vguoqgnp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fmcqwvbs.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vkbswako.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xkjvbjjv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ofoluxgq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3idwdnfot.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3levgutuj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jwgotrwa.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3opuhuqvd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gjxguxpi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3vbxdrljm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ubmyuptg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3hvnzlhbl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oblocqlw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jzvrtlbr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wnjaxgii.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vuzrptvx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mvbwkkac.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3geyzfoku.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3osrvcctn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3cleetwda.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3peeeuaum.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3japickyo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3flrmqbdf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uwevegqh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hdcbzisp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3oeiicvrj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3bwcgowom.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qiongwks.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3atysjkoa.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3atadzuym.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3cqwmxyca.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3niuypsep.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nrkbgbvq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qfrnsnre.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3amplobxf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3otnbwdtb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vousotae.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bevnuuul.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rzzubyvs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ebhjynxj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3bsevsajn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3heluwppv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fxtucfqn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gqxjebih.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qxyzswpx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3foducmps.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ijxhywbg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lcmshbwi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lzqbnlin.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3wwysufut.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ffagjlax.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3olsduqaw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3sjfminjp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3tvwkbdxc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3brgeklhh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3nyfaxpon.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ofoelhaj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3usaejsiv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nojdubjy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xhgvjids.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3mnugmmvg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3epjzhhjx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wgxivwoc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3lekucscj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lwqrqnup.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vdxxyigq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lalsylcb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nqrzisjx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qotxdjzo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ljjkqbaq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3psjvults.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3cgaylekv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tymyhsqa.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3okqrlfnw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sjpeidas.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3bmirumff.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3arztuldv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dzvrfpzo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wufkdszp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dxiruvkv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ibvddaba.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ezsfqngw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3byixtemj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3nueethun.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nuarufqi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zwmfoysj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lpwxmqdq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3codbxpkb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ihgaaubo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3blbmwwbh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ikmntayc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ognjeihb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3pmgpxjvs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3smsqsfpb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gtkwddxp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3rqwjtthw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zjkjurlw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3awkwrajt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tifruiie.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3isoscvcn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qbfrdpjz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3svijeaif.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3opuutgsx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hesmuwwy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3efgpjtie.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fhubawue.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3okaxrxqo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3akqnvagj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3xamidlxi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3yxpmnyce.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ofarjggh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3bttkqzlq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3lxkgheoy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3uapimbdf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cuiytaqg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jstayrdl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3mwvgkszx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3lsooprzx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3cgskgouw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ustwhiev.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3trppmwrn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3xdfyeiaz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3olfcarjx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qbkipxda.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hidqeavu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bastzaat.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vmfovewg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3qvzjzzsc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ljxcemts.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3pcvvrxqc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hxilyqeu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rqbsiliu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pdldhqic.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zofkcetz.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rqksachq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3necnpmty.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rjqwnwbb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jfokoprr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3auaqinnb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3crywjkqo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3omwbxbpy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3kojrmyki.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3sqbgagki.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3lxmdjemf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rqdeprii.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3asusywxy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3nykrwcrt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lxycqumz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ccxboeib.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3btepvqkb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3kxqwlmyn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jvljradp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3bljmgbja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhbxcskh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ktrdwwae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hiwewhsg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hmdkgtyk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3osvckeyq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tnhrbzci.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vpjgpzmr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3tpkzrlyr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3etsoxktq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3cipdgcvo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3otakxngq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3owmxqkto.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jczkegvh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mdcaswll.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3znsmmbde.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3brnfbzat.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3fkjwwupf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3syzafwec.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vbgyhdtj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3aqutmpqv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3njkzfsdj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fjgqlrlo.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3zdtfnwta.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vcyyspro.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pulthvrb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kwhexcxt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kqvkbdoi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3vvylqssn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ukugxviv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3kbajcked.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3qkxxaohf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ggwrmcvs.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3oflqizwy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hmyfpmta.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3vfvxlgub.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3obwusqtr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jeymalyp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3eiasrcxb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3fmexahgf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vtinpuip.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jgslskfb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fdxmnwdl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mzubkapr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3mvlvdnea.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dvgqeqpd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3bthyowjz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3czaqdeki.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yvqsgjsl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rkizomir.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jesdpgel.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3evcibjsw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3oxjgbwle.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3enfkrrqv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3aipevwxl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3duzivdxr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rofasyba.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rqxnjwqx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vrnlqphj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3nckkbvzc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zlyznxrh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3axjkpcqb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3obtsgnyd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rwvpukld.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3atxveewa.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ydmpetbm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3uhmcgrlg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qoukkhcp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pzskdqxu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zgdayvby.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fukqqqhn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xdsquuoj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zudivqtm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qybcqqij.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lluyxlki.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mrigmgem.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uccdyjtq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bbryxoyb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tjwsgwbk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3rgpxegzb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3kgkqveht.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jlnajmcz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3alfalgrd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3bedowhqe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3kegizrti.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3srimhgzc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sozvvoms.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3cehcnlga.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rpahyzvi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vqpdwzzn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dnsuhyjk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3awqxppxq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ijzxmogc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3glvthwxi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ytvfrdet.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3efzszdvy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3voibarpb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3clkkwbmc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ojcepnoz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ebxivskq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3daxhcosj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vtoqbcqv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jcnidpmw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hpiqfyqs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ksnxzuyj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kcmmvzfn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ffskfzio.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wfcmytxf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3anrhpqji.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rpnqvzlq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3twotiudo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3cfpccpwc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ygfprbds.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3obzxuiiz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rxqrczrc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jceifazm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3eicskwmw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kungwtrv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3cuunqjwe.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3geekoguj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3gsvsruth.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3tidgpobi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cgyvbzph.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3dgtmeddy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3dzbcyejl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yposoagh.html


<!-- 参考信息 -->