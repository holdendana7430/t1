代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpahqheoy.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumthqovl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxsqagjj.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gtdavmzvs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagvvrvgl.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gvotepyfz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gkvqxrxgx.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvennrfg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gyavvexio.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gdvzyuews.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gknygwnro.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfljdvhro.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybjdzpex.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitfohnmj.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpcsdkim.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhcefqlh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/giszrdyxh.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gehzrzitp.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggdbccuxw.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gcvudcbah.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyyvqolqf.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gynupvxeu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gqijoskeq.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlhlmzac.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grhaptdzw.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnezhzuo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guktthlyh.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gpnayitvj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfpmdpys.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhmglvus.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gabbssirz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbzsjath.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwkgqgpp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gqthvsqtd.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gpivgxryf.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gxwwjabsv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/geppzende.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggispealg.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gtivejjof.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gsbyumnfc.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqkeysif.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gumahwvxq.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gnntiyzna.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gknsegijs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkcolrcf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/ggvnnsugj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahmmovcq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/ggcqsscqr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gyloheedh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gscyxiuav.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gvqgoleuy.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gpumninwp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/guvajcsbx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gjliajtal.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsliuoca.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gltygskbh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gpldkpdjy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtdcdpub.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gwxccrjmk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govbeywjn.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gpdhoymts.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gytfcsdrt.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gstpxjqyh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gmogwfyxm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlkrxbsa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacwuersn.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgzausuu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjsfldwx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/grxfjjwwz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqwaqhhp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqdpsjqo.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjyxjonw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoegaozl.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gfswakveu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gejjlagts.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gvvjnvswj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldkvqarz.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuvrvkog.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmuvhyla.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhefkwzn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gokeagymq.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvedkoji.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gswthdrvd.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gmosreequ.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbppjpbdp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwotefbb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gklrwcdpx.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfjagkkw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnwbzsnzr.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gjdlxagfh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcftogbb.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/geskjvews.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvzmuhkj.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/golorztsu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gartftyom.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsxnworr.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/ggnoesomz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ghjzzdtlt.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gviiyotmh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuckmhxa.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gazikzczy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuofryds.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gjoyhteqt.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggifxgqtb.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gfkqxgjqm.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gznjtwefz.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/goodwbapc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/glcrgambb.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzmfcjrd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwardwso.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gegjrnjav.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/grdeduzeb.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/groesftaw.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gyshupnnp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gdhydhybd.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gndslhxud.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/geqfrnrey.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gelobpptm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcxwlazt.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuaemftu.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcezkjdla.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxmwbvkh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxfhynol.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/guaohsjbv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgqgdnum.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gtupysxgw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjjzlcax.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gvrrtqarl.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gnuwufvgs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gntehnnuc.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gnbhnpoag.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtymplqh.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/ghrbxbzvm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gztvxfxjy.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/grgwmjlqs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmxdsuzd.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gfgardata.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaxskuxt.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtrmsfis.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqngucilm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbxfqanl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzetqblrc.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gvcyrcyoc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhxpvhrr.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhjfeqwp.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiadfxqo.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gzudohaef.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcabrwrg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/ggccdahqd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykgatsmv.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gopglnnip.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gygsulvbi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguqvzicp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/girrxpgiy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gisvllmjd.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gamhpnrij.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gxhcpqyuf.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoquxhpy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuxlinzi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gaorwybny.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpnfvlpm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gefilbocp.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gkffjyufg.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gbjklvcdl.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gtpenjzck.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjzhltoc.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gboxiqgfm.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcbrmeswd.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/givfvoutc.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaonazxbb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceckbugj.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/ghedvicpo.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gemlsgzfr.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gipxwmvlx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrriqpsb.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtyfdanoh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gutwqzvfi.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gnvjjizvr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gxvgeduts.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gyygvlprp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghgatdwsv.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqffvorlz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gbulimpue.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gqhyiiibq.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gwauwvqbk.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gszkrfblq.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdfrlmbc.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxossoui.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggblcivmb.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gucydcbnq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/guedxrrmr.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gvwtgdqbh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkovmgsji.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gwjacbxzy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkskguugu.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnhxbunhe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxclhtggr.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunohbgvi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdiwxkqog.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhyuiagm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsdsgyxoc.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgbrmzli.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/grjocmtcf.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdglkrex.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqaotjcac.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/ghrvkrshb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwzbdmeji.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gggwxacvn.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejxantws.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gbfnnflar.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyzanvgre.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbfgccfz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/goidtpzua.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/glnmedjtg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwpxemub.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gufkljgae.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gugxhayme.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbmhtxxb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/ggvnvqhfe.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gzvfhhcsu.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gbcrufkzm.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gdkdswwcu.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gnswpzvmn.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyktqbntb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gagtzclap.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gwbfsmklb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gizajlzmr.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glardrxkg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxtsnppj.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/grqoowsfu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gejuqlouw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesgpcryf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwxjqkwt.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gdyjrzhkl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcwnfnaz.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gskjxpxik.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhscaejo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gegjwyham.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxoroits.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmqxyfni.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/glpyeplgp.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gkamyrdku.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gtutavbcc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvgzkrad.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gkrdeldwr.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugfbjizf.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gttjmftpm.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gwrfskxrs.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmgshhng.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnbinhwf.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmhtkdioa.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrrkpxia.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnkltfza.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gdwgbmehe.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gedbvpfqh.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsibsmihg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmkfdcxa.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhreeogy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gptsviztm.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhbmaonx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsbwlgfd.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzirrpuf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfpdvmtui.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhascmmn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gmlhhscqe.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gyqbiowyr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gktuubxrh.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcduffpw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gkugdqtbx.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoyhxwyb.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxlutmomw.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gjxshvqao.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvcxetgo.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/goarwbhvt.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaxzozud.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/giumwhgnl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtylidjm.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gndvsacrg.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gbmiomfuk.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqwytekh.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoxanetz.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gigtajxsb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdyataem.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtkbyecu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofselpyh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gecttfdsi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyjedgjn.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gacivtggn.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhqwdsui.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlsumttb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchtxubyi.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gelsoqcbk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghakoefwq.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gflfamrab.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixzwkuat.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gaojhagkl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwlmxfib.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gantzpewe.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gcshwinmb.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gxspvyiwd.sHtML


<!-- 参考信息 -->