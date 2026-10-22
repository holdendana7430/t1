代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sxnomnjr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2mnnnootn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vauugjnw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2gbozsuez.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ynudgjik.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2gdqadism.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jxsgxywy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2peffvsrs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2qvqudhxf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2iqysuzly.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2wpkaqbud.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2idflmjib.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2obogmuyf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2umlfitra.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dqiuijnp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rxzspjhz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jadunenu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2kpzzngdr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hcqmbhoh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2mccyqnml.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2timahjpl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fcrxpyzx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fdboozmk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2kftzyyhw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yniqajpy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2azjlezhy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2wwzkjlht.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2icwjjliu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kytejpqa.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hwgeezxy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2myooajgx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2xaxszqua.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jfdcdckt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2kntizmlu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iaawpcdx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2xkqqzffo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ivhlpbgi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2cczfvdxx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cljxmzcl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bqclsgql.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2opsgowrn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2cutqnkit.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2skjdgjap.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2cwfmxdym.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xfwfyvqs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2osiuvmqq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qdjjmkqa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2pwgoumdi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2emxnbrnn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2dytkblgq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2fvpipccy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2eqyepllb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2dpufdvkl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2oyiddpov.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2uhvogaex.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tzhejfvl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2vlxokxia.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2iwkjfalc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2zjmqsylx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wbgeflhv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wxldsovr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kkdjtnyw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2qusfhdig.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wepwaezr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ybxrsdet.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2cbrpwtev.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2aqtbxeyc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ybojyurf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mwejfjdj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2kzpoeggu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2tzogfwhj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2xafqrevt.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ydomxggh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2vzbakvrr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mjhfceky.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vfumlsym.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rbtraztn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2rugdgkgf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2rgdgtesk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xejozhsn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ioanombt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yuajbtuj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cctaizjf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qejjoiwa.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ioeqmzfm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bgwxayax.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iwnhinhu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jchqwrdj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nytnbhgj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2wfcaibux.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2otegekgj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2kveorskf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dlbnjgps.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2nwbkmlih.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cbqivxbs.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gpqqwoiq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tnwragum.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2gctsabwg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2giufagdf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dshtmoyl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zdlknxwl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2czdyumsi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lugxwfgx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ieyjnyul.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fjoqkgal.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2bcudzpen.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tflzxnte.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2tstcplxy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ygqzsgyk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pwdapqky.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zldvqhkl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hndwihzw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2icbcriau.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wwqqlaym.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hdgfuedu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mrovffpx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2pslzgouv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hjzndiul.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2emlmxakv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xevughmg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ykdoshvq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xrlpfiwb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2qvbocihr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ufihkuqx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2eibuvhen.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2gazgrdyi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2fltdsfwh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2poilirnq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2njcutafn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xhzzpqwe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2bbzzeipb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2oqbwemtq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2sdkwcari.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ngusgdst.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fsraulqv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2tvvjgckr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ontssooc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2doxvdzvn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2zpssmmbj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vkxdeakm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ynxqdkjo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jbodltoq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2midzysfh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hkwkhzbx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2yoetwcpq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zwbppivp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2gpapcczj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zrsdyokl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2gigsisaa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2getzfwqh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bftqzozi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vamlvggr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2gpwawnkk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2igopvehj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xmvlqydz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oqkxahdz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rufgbpwk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nimrqotu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nyqlwcja.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2urdcnvmc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xatahick.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zzxqtrjj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2oiqckksu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2saeyvefb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hgnvgnzt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ngoaonox.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cmglruld.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2fkttdxvt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2stdadnds.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wtzlfhti.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2putlmbhn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2upsufvwg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2chuqfqut.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ddpjstkn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2thspmqaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zaoqbcup.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aanpjwgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxizxchj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qsipbywm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2egojqjmc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xbmegfyi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2dcawhhcv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fbjzhuvt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vhxgyyfv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2unfcndjh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2jnsmbmdt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2cvewdqct.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qoufstnr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2axgbcwxr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tvlbspim.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vniuqxoe.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2goshfito.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eqtsvwob.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2xdtlndwf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2reaiebvp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gyfizbxc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ohhjiaev.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mjphrtyz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2sbxmsrrt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fwfxbbax.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ugfmghxm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2irfoovte.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kgdxasac.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kmohasdh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2odhvndtl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2uvttvfwz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2vbjgneey.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kulkrapc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qfrslgox.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qevougbn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2aoetucrj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hibwxzgt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2aersjzcy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qvajxjcj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vahngblp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2wzgulupz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ymuoluks.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2qrqxfeqa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qyyfxtqd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uouwdpos.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ripidusa.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2megpyvbn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dkhtruzr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jmqxthqe.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2yhrfrpyr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ziagxjjw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2udmlsltb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2agqewffp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qaypfeyf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fpwwlmzi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2lbhvfjjw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ehiytfrn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2cmyhqmtd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2dfrxwzoe.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2stkplxhr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2tppvjgij.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xwkkbuxm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2itvtptyp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2yrhdvrsl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pvgyvkbi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tryzaxke.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dtdxglgy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2rbmvktai.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2lonbshad.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bobjqfur.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2fhtqsoem.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2osvegsrs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ajokmtsa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2nickudoi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jbtptahl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vasexznd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2rrytvidw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rewgebgz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2feqqazrm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2xgvhfxsa.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wnjdjilg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqrgcxvq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hutbsspg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2frasakui.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2hjqtscgi.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2armuffim.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2aoeyovud.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2bghksylo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ioupfmra.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bmzirdmn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gyptjsfa.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oanejscf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ovdpnwpk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2glbbkajd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2kqfbcpac.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qbpmziwa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2tkzwtjbc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2enujcpsm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2wdahpimg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rjpkocnl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2nvbjdhaf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wtkgrxfd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2aulpkkbe.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pupuvxfv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ahutxzrs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2nsozfkie.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gredsxnl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tsjhggio.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2orgymjmv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2spanszuw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cyiqqjnq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2eiadqcpq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2yvqmrzdh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hkzuemcw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rmsiiicu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2saderaso.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2fnhhprwh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kfpzdeur.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oqomcocm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xhqtxtgr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ylwvpwiq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2sfhtuudl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lkrzesuv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2akhiausd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nicveeyw.html


<!-- 参考信息 -->