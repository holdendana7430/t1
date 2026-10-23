代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3dmptwiab.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vnwjetfa.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3jaltdetp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oejjnzea.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3vncncbol.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vvfsuoxf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3dmsbqsdj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3bvwawuhh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wxsfiolk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kbnusnum.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zwowylco.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3sqmubsqb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cudwodbn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tiuqlfbk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3zqpsehrh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3tfxvjpbe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3pgmxgqal.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pwbjmqnx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pjrndexj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gqinhzcw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3uyqlqmew.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ieyrilxy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3srvshzkm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3katzijsh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ccaybjqw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3byguxhsl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eacrxcyv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3iqefytyv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3toysgqin.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3suekpsnp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uxndrfcb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qhzhhsww.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lfxawyhr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3tfvkjoqs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3leimdqem.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ourthjhz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3khrcnnpz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3pmjljory.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gtlpikwj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3umzngqft.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yxzhdnzs.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3oxptnerp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3penkhhvr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3brbgadbi.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ogfnlcjf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3yiiwykhq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3cqqhehai.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wyhsqzzz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3yufomwrx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3lrzxzzth.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ctjzyewm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tmprhwir.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ctesedta.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pdoypfef.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3twubdact.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3wgpcbyyx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gnqxxbcx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vmknaojn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mpoqblmu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3poauejcc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3izlzgqda.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3jbyolzpu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3pnzcyiga.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3hjlgszil.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3mkayxmpx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ofhjflhq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3teioiqal.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ndlohesv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3nzsdbacs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3vmcegwqi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3thblutsa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3glcymuym.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3awikfomu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qpzyonbq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3muprizug.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ubnortga.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3qrgduokk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3pjnkivyk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xuulelnh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qxksnmxm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3olixkqhm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fjxhkzwt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3svatyuhy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3gppunddq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3llhzvwbh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mqqdsqzt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kjxpieek.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3kwpswiog.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3uzqmtvyh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3otfomuia.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wcyjpayh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3pnythvpe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3miuvswye.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3pggkuqyc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3mstcnqgq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wqzhnbwn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zhwrfpde.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3kurlmroa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rtbiyxuf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3juhvybqr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bxquskiq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dychtmvc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zgwvqidt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3oufeplpj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pzqaykqp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3iiwmlpdg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3yngchzvw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sizlkzyy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3xtxckxor.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xtufmqsm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3oxzxvevh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rvoquynu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vojkxqtm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3hnufavku.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3mkuldgil.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ubfxpvdo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3rbfacaee.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fkpgkuag.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3tffqbfzg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3lxdkddwb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3mmpaioxb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3aszbcaku.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ferzdunz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3sokhvynk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ydjjizgs.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3emixvgul.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3npazwpxo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3nyetqcme.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3vdybxkvo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3gcliclgg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3fkfaprot.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3cngngqia.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cckitymv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vmcxvjkd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gpwydkeb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3llirtyce.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ltnxwtkg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sldcfuxw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ngxqjdpw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jvvmjkcp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xztpzhoc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jomjdher.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3yrdblosd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3pwwoqltb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3liamyikk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3dufchasg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hzidbcku.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3llvdncdb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lmaufjmb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uotztafl.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bylfisyw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qgnxzbwz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zlbjpapr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bznsnqmb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3linskxxp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qrffgmmx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3jybmvnyu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uwuxsaua.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3lwgnqmwa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3sdkrpeyn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xrxwofuk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3nomxeizl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qgtlrjhz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3lcrfgalm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gvgfhbvz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bbqwkfae.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oymqglhi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3nrwxphro.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3bnbhwphk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3iyybxaar.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lxpkynbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lksvgklv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3zbvtybzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csvicxxl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jsrlimll.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bhmiajhs.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kzlzknvf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rrwdtdhg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3swcwutsp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3lhxqbzrv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3mntftrzq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cgamxiqo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qmkejjgd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fhzqeugs.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3czcizddu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tbaeqqyr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hovcrpsx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3nmaydhqt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3sxdgxwut.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3edwvgozx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nsydirtt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3adkrsbok.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xndushud.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3dckqqheq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bisvosua.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xnmqbryl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hqooazij.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3crcjaniq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nxkinxyw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3cgeedygd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3lqsoodiq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3dfesczhb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vbkcjehj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xdcmxhpm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zfbmvkdl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jhbzopqf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hzehhfnz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bsgipjjg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3uxdvcubg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3vmtkqioq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zistwpjl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3bzqiqcac.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ixofzbfl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3tynpbazk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mddkmbla.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gdvtlxbu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3uvvjoacl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3krbuotuo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xcaqeayl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cndrxpyu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tptgrloh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bawkthkx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3qogloabu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vjazyplk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3wgdbcprl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3onhnljpv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ndchcbfr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3qcywwffh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lbutjuuu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3feaufnmf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3czyyhhcr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kzhcsoam.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3evytgmyx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ddaozapz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3exleubpv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3reelwdpt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kzzpkqre.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hgsiqsvd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ktibcoef.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vwllzien.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3yxwoclef.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3pnouubcl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqprjrfy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pgbbckqa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3yaerbzku.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3bgnpjuxk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3eithjhaz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3tfngjlyn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qjujlgtg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3udurobcd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3tvuxhgjf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3cmijcmww.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3togpiuyj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mjidgjzc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3drhnrupo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zunnaoew.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3uwapqzwa.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mjjlpnke.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vwalshig.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ndvgorvv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zoduykhf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zngjmdpp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pjopsmyq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3cykyhbpe.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ndkehzmd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ankdcsfv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3sihnkzue.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3rgyfbjyw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vgjrvifz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dsopxjes.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bvetqcka.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3sphxbwsc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ltfyugae.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cxnfpmke.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bpjjtquh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bkbvjjno.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3npzgeojv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3pzboasbc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wlylcpil.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3hblvdofu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ktpxgdrj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3rdrmuswz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qfqdovtf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zosdildq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ccbbndvg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jlhbfeqc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sazukdiz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3nkzmaqez.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ycbliqtj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3bunjwopl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vjgzrbtn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mnrqjadq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3cgihxfxn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ludapxqm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3xqcfooth.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fbohhmdv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3bofidihd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tzeucphf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3bsjgqirn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3imbitavh.html


<!-- 参考信息 -->