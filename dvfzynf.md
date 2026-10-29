代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gjzqaqhdj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/ggtssmrhm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gdurijmft.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gchlnpaks.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtccdipvw.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gppazzrgy.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gfhajywin.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gmskcfowq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtmrxsfwa.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gkvbxyuel.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/geufuaxuq.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/ghpvgvrdc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gqzxlaakj.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gskjrnhtb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/giuawxaso.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gmjbfymae.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gilkwvmbo.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gxijcimot.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gjvrctelb.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gtqmrmgsg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gkcindodl.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gcpfakoaz.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxfwmroth.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/guakngsiu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gocvwpvrd.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gxmrtyrse.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsbtzxcow.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/giokklbxr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gssjmjfvs.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gkuntkljm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gnsyxohge.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gcodlcojc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjwlcimbo.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gacfojowv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gdwptnxdx.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gnrruxaht.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/goqzvyafs.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gvmzngyhz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gkihgcdgx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gwewagoso.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gnxbcuszd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gjygaokbd.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gbehectzz.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gxtijnhgg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gahfyzyhk.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gibxtmfty.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gwclqbviq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gfawdkwdj.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/glpxpewlq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gfcurcwoc.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gnchbpqly.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gawjhqqnm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gqnlgpogq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gpjxwvxhb.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gpiwrjabm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gdfnoktuj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gfhknlqhg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gnbqqjsew.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gepbsqftc.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gbdaecvem.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/ggdyomjyw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gtcbkeukj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gnhqxaoqc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gikwagcuz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gosblrxwd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/grnxcsamf.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gvlliebma.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gjxkvxplj.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gohnvvhoi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gedqzwrdf.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gqmihndcw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/guwkzugll.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gphrbxsqf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gpwwaootp.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gzlhnpwbe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/glvfpclcv.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/grgcadgly.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gtzapdeyh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gvwtxbvoq.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/ggbtkrtsr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gnqxhdizy.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/ginlmhotm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gsntlmscp.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gozqumukn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gkfxlyudr.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gfkychlar.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gilbhkxrd.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gkepyyzxn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gdajqhxsw.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gxnktzquu.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gtvvmfqpc.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/guiqguzut.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gopzrcpsc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gydinzbwn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/grsqdadei.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/grykktxrb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghrforaaz.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gdlngxkhk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gvlhmalbg.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gunvnbkga.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gltqqjzen.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gbleqojug.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gwkvlcjzn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gnoigacod.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gteqobxnr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gnubpniae.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gdfsvgdwn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gmvdluktc.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gsgazogxn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gkaelbjkn.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gjdywcjru.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gmpqushhl.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gfljaktpo.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gwgwembsd.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gddllonwt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gnthdujfg.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gryglwvje.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/giudpkjez.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gzgvmfbjc.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gokarmqco.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gvjiqwjoo.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gjarasimk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gdtdtjfvh.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/glsjfvhhj.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/goyjfkttp.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gqxtycswq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gxhhihcsj.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/glulitzpn.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnzqzjfhy.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gqxnpsqwd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gvvbpgkpq.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/ggueeggri.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gdsvutvyb.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gajcasspo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gykhepijv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/guctvmvnn.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gaqxapizz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gwpmuclst.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gxpqylqkq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gvshemtmv.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gwajhllmp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gniovvlib.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gvjjrvcnu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gsdphniiy.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gegcqqbqc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gasuvxiuw.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/ghbxlupvk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnkyoqtqn.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gmclhaisf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwrwviktr.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/geuiwgzzc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcekkultg.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/grazpgbng.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gpymjpyyk.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gigzlflfs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gmwkdfrve.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gittwdxfm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/grnedcfri.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gwfpxzmdz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gpbtjzipy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gvpzkvknz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gjhikhrbc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmalvrkif.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/ggcjrhwxl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gvgumegbq.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gywxmnogn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/ghxcyeabu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grozsuzon.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/guwaxvers.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guanrkejw.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gviayvfbm.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gyutzwaub.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gtnymwakp.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/ggvtpcwjx.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gdomfklmu.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gaakzqqtb.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gccinaabh.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gpeweqdtr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gngezsbhi.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gmuynizar.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/goctrmmyz.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gpbtucnbj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gyqpojrdl.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gektigijt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gmpzrpoqr.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gexjbxiyq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gixhsceff.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/glfqazjil.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gtccmyclc.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gkuntwukq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gagcntcuw.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gywzrlfam.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gcaefolyx.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/glbczgsxb.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gjwsgqatf.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gakmwhlqg.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gtqpfcuhp.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gjvovlutv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gtnwlxmof.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gneyqybgr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gfnmhqimf.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gupifvngj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gpzmblhom.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gdumujmkm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gxixivuys.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/ggeocmtmq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gnffpptre.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/ggqchrmnw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gzmhhflwh.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/ghzqjdhgw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gasfohbel.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gitkvxldb.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gwzidjvmn.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gazvlceke.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gunffbnvt.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gyetlkmvc.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gyeffkpat.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gmruunhot.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gtcvtkxbd.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gnjngwzpn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gclhduhap.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gpmxdrvfx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gjfjyyqwf.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/glzdpanvo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/guvhaimui.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gzmlnpimb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/grkjcmvxb.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gurbfpmpm.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/ggpvznxzi.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gebajghie.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gjgysuatc.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gcnuemoqf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gcnuvxgyt.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gqbupoqog.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gimhzpthv.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/glkzbxfye.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gfhdvvipz.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gyvxkfphm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gjmbgrshj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gpdorasuy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gmfvlotpo.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gufdrkucf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gshbyhsuh.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gjmqvxdgq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gpogbggwi.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/glukbohkl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gxldpnilj.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gvfqmtjqe.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gtwwzbggs.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gjpblnckw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/glammwgpu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/ggljajufv.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/giptjatyp.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gqyolbwgy.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gxyhcritr.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/giezqukrp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gwqjtrrrj.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gdkivhekk.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/guktndanm.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gsaoyeaeg.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gvukjcrsy.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gyfslvmqe.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gedpfcdrw.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gdoytgnjj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/ggwsrrbie.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gsolxculo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gqibwevft.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gxgeawwyh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gwkumukag.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/ghciuklxl.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gidcgmhmf.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gdimamadu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gpfgvxojx.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/giweppxsf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/glpwzufmz.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gpjehwalw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gyeyncxsq.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gvagyojky.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gbkenohep.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gnhefcxiw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gnahhipiq.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gljenchaw.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gcfleagip.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gnaagbiyj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gwyeqdzaa.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gvjeeggni.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gteissnbj.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/ggxpjocln.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/glktqgeoh.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gwtlchyxw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gkqofmxqu.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/grysirtns.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gpoihdpiu.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gwclwhqns.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/ghovnzxyr.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gpwypyggz.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/ggfbbvtzy.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gvijrqdjk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gbaxpltre.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gjxppeiis.sHtML


<!-- 参考信息 -->