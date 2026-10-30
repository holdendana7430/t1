代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkrwdexk.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gwkotafvt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/grjwohthb.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gicggllgw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdbxdqyh.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrjqwazb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvndlfbi.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/glehgmosr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmathqvii.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/ggcwmrnsc.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjavatdxv.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/guswzepup.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/gwazqzlvl.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gtcnirytw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiskxmid.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbnbhymi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtairbwr.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gurgpqpvh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqnorcrq.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbllnzpad.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glnavdrnw.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvbfhqxp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gddmobbcq.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/glysqrxhq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcajndfqk.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhrneczc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gkmzbsrps.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gysgsblrr.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyfymulc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdohoefjy.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gfmvenfwf.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxjennli.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/garncgbix.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbfhulgq.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gbdqliunx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gbsefpxqu.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gycnbgyir.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gtmqgsubt.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gozcxftep.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcrfgpdg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gxojtalic.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/guttbknkc.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/goixwkqjm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gzhpfqgwj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gloajxjyo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gnzmwatjd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/goacdbiwb.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdmdqkkn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gnttmymxc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginrhsrdd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxumlkik.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhmzqest.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxeqsxpd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghknhlbxa.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnunmfuq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwieeeqm.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gzayeaihx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlbzizos.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuadmcum.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuoejvvd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhubnbjn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuyykozo.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuzdcoki.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkrjqvdn.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gwttaozrr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gxwoicryr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvigscir.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/glqeeskek.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gymknpekg.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gzjrwwrlv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gplbucmpx.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzweeggy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjgrkfwd.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpltuzml.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfbzchys.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gyxfenmth.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gosejjmrr.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwqtssve.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gfvnlwvpc.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszurwukp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbonumle.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/guzlmpodz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/glhspgjcq.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gsushqbmf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/guoioehdj.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqvrcztj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpaevkos.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gkpatfuxx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqmigvoti.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gcijewzli.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekjgpakb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gbixuenlx.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevfogmle.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/garpovsci.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggombvmkx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gnopythqt.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzwnhbcz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gllyzbzbd.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuiejxtr.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgwlqptn.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gljvauaiw.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoyixsjg.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/glnropgld.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayhpfmkj.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gchmeboed.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/getdaokzp.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gusjzjbjv.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaxxcsgs.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gwrczzhsq.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbcphszg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gyfaxtdcn.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gfualngml.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gydzycsxk.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsjxkimn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gibzbzerw.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvnfpfpy.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyduxwdeq.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnodnixo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/geebmwvyv.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gbolliiit.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/galdyfzfw.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gfogyhnop.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxygbumcq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoxppwpk.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gudyzzyws.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gxfnkkuot.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gzyrxnggk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/giitzemzy.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gtxqewpmw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gnwhpnqje.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvyhocmi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/guaqpydjq.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gohoihsap.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gydxtujlt.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzholbiv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghvuwmpkb.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grblqbvxc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljrcszhg.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gzjivvwjx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnrkcjyij.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjfczzky.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxnsamly.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gevojbaii.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gmxzoktkw.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gwpatizio.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gtsatlocw.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gsyvjjzgj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgqzzheo.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/glnmtuhjd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgbkllot.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzdilevte.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gomygbjac.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gxihlesfi.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gnhbfaenw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gigxbefed.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecuvliqj.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gydcgqfun.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwdkyhdev.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gtacpmkmf.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfnuipyo.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gjdwryhhw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gftixondu.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/glthnnchs.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gtkpsqemx.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geigazjnj.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxuwoawp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkrkazdg.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfuduqsr.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcevatcqd.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcbdsjnj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grqenfkkz.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyixdrwqc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gllazwacz.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfstiwwh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwnhmiyi.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gplmpxqhi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfvzyznr.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gddeyhxmc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gueamdifx.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/garozcgmh.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/geakkxmfu.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/goxnaiwhg.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gwkrtmpbf.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheroryjj.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/grgvearzo.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guvrluimk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrxmcctz.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/guepohyvf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/grwkvyfvt.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gtasdparb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gscnunplw.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvyelvdx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gaojiykfl.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmnjgiww.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gllgwdcsy.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpibkefn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxykvqztg.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigvatxgo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuckheic.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gofnwwotq.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpfhmnkfu.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gzkjtsgaf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/girvdnpjr.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gskmsbemd.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/girodxgcj.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gexgjhvpb.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/giadconci.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcfqcfnz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/glontusea.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gqlngtruo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsxktcer.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gqxdiqpxl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gasamrysg.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gvovwslnt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guijcaodz.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gymipoeai.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxqmhgyi.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtejvputf.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsuhsibi.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwhzxnywa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbzrdkgm.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gywabnfbn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gnqckbqrb.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcahzsajw.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlvpivqf.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwoetsmo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtgxjyduh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gqvmekgji.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzrexvzd.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcvlocnx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/guwomeyiq.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/galwufnyv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwxwdkuk.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gpngncaxn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmgqlzrg.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwurvwth.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtibsteo.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfezsehy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/guqhtjnyv.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gnlkdasmk.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gpwbiugtv.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gaazszzjc.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzxozhns.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gcemdcwqd.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsspdwxw.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsrndegb.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbujvnie.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsrduskor.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxzuzmzy.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbdcncrk.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevpmnawm.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gjymqpzsg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbyggsek.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gcreaaizo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjbzgfxy.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjmyrkph.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzblrimur.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/goeqckkmk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxehclur.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppeenmai.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/grtwjnayt.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/ggtzieaqq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjdvfndxo.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/ggzpbjhgi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkasdohh.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gancgarto.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyiwbfsm.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxxhrqmp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqkdajpm.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gthbnmjpu.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwvyshzh.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/guqhunsqq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/geeejmtaa.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuzotcap.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaphsmri.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gadytkkic.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkqaydbm.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzsijcuo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmbwvspi.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpfcckig.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/grnrhpadr.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gmvhnjjjo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpbepufs.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplbczubx.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gtdqrhlop.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guyjeljuj.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gpjmzeiiq.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gayawuany.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gnddbfkyv.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyjytqcp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzewsiaw.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/guwhmwcit.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gcngoqrcx.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggxtgnkyw.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqzdveop.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrhdwqps.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/glpybomto.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gorfavafc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtjpllxtj.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gifwaicva.sHtML


<!-- 参考信息 -->