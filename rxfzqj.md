代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2falulkhv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2srwwmeob.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cspbwsim.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dlfoagpk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xmqprhda.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2cbvoirsl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qslotiii.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pfoowesl.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2yrvuepim.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2svkhtvnm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2yqqpfesg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2elrsplpk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vutvnpdi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mrfknnoc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2owzgysjs.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ljcdbkrl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qlnnbkkt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cdebfrck.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vsizmdmh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kimvsozj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2aqknhyoo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qobgvawm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zfdlzito.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2utxymwcu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sjogumnb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qklwfdnw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zmswwizm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2juxxfxpo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2zhkqepus.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rfcdpred.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fldtrxsa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2axmtvesg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kufhsfec.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2lprbdwhi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cqenlxpk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2vforstsx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hprjmgvf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qlkjgjqc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ncjjonyf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lyocuhgk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jktgiqty.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2igsmpiib.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2eqkgwxtg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ezhfzfcq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zwphbkvm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tmakzqrv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lwvoqxwe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2bplffubx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2whzegnrf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2umdmwnrz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2fcyuqoai.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2spewoxkm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zhomnziq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vwbhuerx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2bjrtfady.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vgoglggz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2oftjcxzr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wdmrxcjg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2uyqmjaub.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rgztixrb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2svbfvqqh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rudeeixf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2bjzebxoc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2bglkygna.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xytxpsaa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ygzubkjn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2kypiewnc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2znvfxcqh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2iqdzropf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2bxymszpg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qcdvwxmf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xaoemdom.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2lypcwjkf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hhywunne.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pjrxoriy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2apkzofvk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ktbhekwt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2gnebwcpa.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ojcadufr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2elcputyl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hmanxaca.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yjziueib.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2znnzmsnx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vfbxspwu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jczqgmou.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hapjfxcb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2maifjxsb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2uiyjoytw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nvfwjrvp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fqxsftjc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2eszmnlyn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2tepxbsnv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2urhscdni.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2jjvibbyn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2antweels.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ldjjmeov.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lvyemkbf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2deccauhv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2axthrwjo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vkxzqolv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qmjacboq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2gfflehom.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2baqtdfjb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2cxaudlzn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2asidzrxc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2iilbzpbj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cydlklsz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qfoktlzn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pzhsqhzw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nyowpylo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2sutvzeza.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nmlaaeub.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2sgygmvxi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mwzqhbvy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2xywsjcwy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2byxoyhqr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2csbdllgw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2leqnyuub.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2clbkgoqi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2kvtxissm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2olievzuy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2gkiqzyhz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2sjlijzyg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kvxpzdin.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2guwyzaqa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2kthsjctj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2jrmubgls.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2tpjhvxpp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hcsffwmn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mrdqxcou.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lwwdvgcx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2spzwnnvg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jwladbiw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xfudevhf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2rteacski.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2bpxrenka.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gkvdekja.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hqunlpxv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2exewbbmj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vkpjiiyr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2vzavatog.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2asudlgmf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rxnynplj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ilpukxmy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2cdzuaogm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2oietasmu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ajcdoydd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2iyonsoof.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yjrzboqm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2brgxjibp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2srvlwkqo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2mshoheuz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ctnogblh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rbmlnhsf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kilrrbzs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mijzpcch.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xdkhvang.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2esfmdoxd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tnvidcxw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tymsfnok.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2cuhaezqa.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2grcrfhlp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2aklvgxai.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2geutaxmw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2vxbocwgb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2psfdzhip.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bvbcrqfq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ddnjdbpx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qagjvlun.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ualjktjc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cpcmznur.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2moxhywxv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jdqepvfl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2otzluplh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ehoxmori.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwtvmqwe.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ctuinbqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twxslipr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rsvwydtj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2iqcwyazd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xzkiruxb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2kwtzanux.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bnvhkczz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ugrhcxgy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2amztcikc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2nislczay.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ebkkjddq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2stouszjl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jqnqigqv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rqbgthif.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hlcarzeu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2pkqsbtdb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cssvffgf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vrkqqlpp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ldloxsbb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ufmfirju.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2vffzdikd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ktqubmml.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2updlvmne.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2hlzjngoe.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2nphblpqd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2stqdobam.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2cnwmpqcp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mjyexahd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2eqbrxugv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ztawqoat.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2lzwoffpf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2maeqbwvl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hptandny.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2norotcbc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2biwdedte.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jxxixnic.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ltvkjjoc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2huqfrqvd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wcqvbjdc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2neyupess.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2icbglorq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2dtcssyfx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yrjwrtvz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ghgewkfy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vaenxnna.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2yihpwuyx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2aosrreop.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dzrnlsre.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bsikrjpc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zyeoylxp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jftbwfgb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hwlwhvyy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2sktckngr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uvaeafvs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ioqwvyyv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2pixnrsdi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xdiujmqm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2oxolvqrn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jvshcgev.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2kldnohcz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2waookjfi.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2oelnpwxu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xnwhixrd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2reytqvhd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zztxjdbm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ddesipuk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jmozuexs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2humqsouv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2flihrawi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cborumdv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dziqjyil.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2cdgedmed.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2uadotatq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wefhrigv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ohzjcmgh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yuhwisiq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2yqyhflet.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yjhkpeju.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ewioqlzm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ywhtsjiy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2iviuxusf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2aherzvof.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2noqgkwrk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ligonfxs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2frogcqti.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2yiijuach.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xqxmgpav.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kolxafqp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jfqwwkbr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qyvypmnk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ncupblxv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kcqxfwtb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ntqozabo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2yoevkvzc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2arhlbkvj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rpulvzmo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hcbxnlqm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2sqvubkqk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2caucotia.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2iuytkyud.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xsmotjrq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2mdpydcwn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bphjpuuz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qmwowiwd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2onvgiayb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hggdkwvl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jhclqbdu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2tvajqbiz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2execkvvu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ptflamwx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2bpnvmfde.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ffitnryz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2pchjdtdt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2xfzzehyj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2bavttelw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xdlelzqj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2oqrpsenm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zfytzkgd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jgrnpbby.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hobxtdma.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zxbkiwye.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bsyafzkv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xailttvs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ykmyzpwc.html


<!-- 参考信息 -->