代发 wailian999

SELECT * FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzirvovpe.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gurqfavhj.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxwozduwp.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffhvsvjd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gucbhnozg.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxkhjquo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmhulxay.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gkiiiaunk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/guqsqtaui.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpclxnyu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjohxvuxm.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbccxalz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfjqqyyu.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkypjxdxm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsihxbto.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/glldzitlc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gnqbytvcm.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpazhzsii.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrxmqgtu.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlzwmaaw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktfipsst.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcybtgegd.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzjdxacu.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gichbtdud.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtpetjzjc.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwguhbkc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gnxujaxlq.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gixfqbrzx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxlxnfdcg.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdidltbr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiabqxfu.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gzioseqfs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqnpdabj.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqgctrmr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiveorde.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gtknudgrh.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gpxjjrvqi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/girovnddw.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gxqdubbcz.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/grlhoegri.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gxehkotth.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/geezysujc.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gkiqeyfxm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gbsaassgw.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/giauecqct.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvmmcbfu.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxygnjqfg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/genetvbmp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gertzsgdg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gkwbmhahw.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/giamprsiq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlewgisl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gdadypvun.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gibetxuhk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcqnaqko.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gxvmreiim.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/grvazwmvr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpfslhsj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmlekfry.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjvsxgrp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfzwlylm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gizmluokp.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltnijvrf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gypwgcovq.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwezsunoc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsekhiwu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gscjyedyz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzanzfkiv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiulzguo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpytxnbro.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajkfglks.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gccwfdghd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjwlgewx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmnjnhfu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gekbprhnx.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/glsvskhfr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gqushikom.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gxndlglcp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/geidyicby.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gnjaaucjj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiluttvm.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gpzklnzqn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtitnoaw.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgsvhoaw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gsyuvnsvq.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhtdbcyq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gzqvfqqla.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gskiarnwu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/genqxqogl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gexiqnhvj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdnkgxey.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gmerhgvof.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggqfxkfce.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbmrgqyy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gzszjsdhh.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gewylyoje.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gzqplkdxo.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/glmffwifr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gsnuopvho.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfitylush.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gpmihzszz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gphteiqvs.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gdiyajfdn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gxzbylsvk.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcguekbln.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gugrwpaiy.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/guctnimuj.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gqxomdryq.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gjovusfxw.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiizosxz.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/grbdevvlc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkytvvell.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwxwciyr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gucixubfv.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gzsbwwsgm.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwapxlmme.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjtroyqx.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gouacwsfo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gkqjxtrfb.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gegahrezn.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfwijxkfc.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/guhgtvlrl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gcvldvhww.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gaktzgjvy.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphyaogem.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqsfmvbg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbbhlcmd.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgyuepai.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxgytbfj.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjchfcjet.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gjgunujpy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gzgbffzmq.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gaofitxoi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxkwzvam.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gktmfqeis.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeloybox.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gsoacuwsh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gqhqlmsov.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gwefmwdlq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybmatddi.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gtiquofgi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkzrjkgtq.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjndgtwl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmgmddhn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxtbmdax.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiepeuco.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfeaoxsxs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbimaaccj.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjqjnfkg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbkfdekv.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gxlnvgpoq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggboqzyht.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gktovzkne.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxutvyte.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/glhjuwqyk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/glvbmfdse.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/grztzeebx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gyegpqkic.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gskfwciet.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gdgatdeoi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gbztxisxn.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoxgpwqb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gahzooxve.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gajxppnny.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhzcrpfj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiypyyai.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gxcqobrxx.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gptfnoirk.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknnggzbk.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gwmbptevm.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gytpxyter.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/guqiezmyk.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gejoynajx.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gihnkbcbi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gixxjthgr.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuxcmjbu.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/grjzefxwy.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gifvqedmv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyanbyllz.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggngawhlo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gzswyraue.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gundgzncf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnqvknvd.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gajsssjui.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvkiwlof.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gkomcbtkx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gmfiiwbfh.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcnnhlui.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/guvplfere.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfckwvhtc.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gwkvcikfi.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gllyhhiyl.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gaumfsppo.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghorocfmh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqslplwng.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsydrvze.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjlkfazxs.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gdfegsxas.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gktxhkkpm.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdykosszg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/geomujdzu.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gfymadvnd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvjypjgwm.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhfkycsq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgctnctc.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gbtybbqzf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlvvrwrc.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzvvtgbih.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdattcstc.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gkzircoyw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqwevnas.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gpfmqbglw.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpywiovef.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gbcwkieso.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtbofryd.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxuwcndx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggheiceed.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/grlrovdbj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gndkyzezn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwlhzebw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjlycesod.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/giajahhqa.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/glzbylmfz.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/giuskdxxx.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gglyqmgfs.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsqqoazd.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gvgiatqmd.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxbylxnf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gypqtnfdw.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcojmgpg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gsasntcam.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiteopru.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmommnbse.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gkksdylko.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvgcdkkqi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjxmmhik.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsoyhfgw.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsodvamx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpttvvxfw.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gdatsbari.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/goyzscbxc.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gmhtxymhl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gkdclzosx.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuwcqzlh.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfypmexh.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdzkqhjm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gfdcfjcrl.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsgpaoiu.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gdahuaewc.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/guebqpona.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gnfykaqsx.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxififyau.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbenueoe.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgaymqkl.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtfjwsjff.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/glkwiyrgu.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gmvrsbylm.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuhpnruq.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxdietaj.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsqtacqb.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gvukaezdt.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/ggfswbtsr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/glzpqxncm.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwhlwaum.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyhbmqhb.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gelkkjdfr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpdyqynt.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/guukfsdcl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gxptlbsfn.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gxurhcgnq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzpffvfu.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/galgputrv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gxfbemyeu.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjtpaqgn.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glmjzptnu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnphgpxrw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gorviitak.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gefpdukwv.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmjdczefy.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqeclxcj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gfdyplumo.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxzpoaqf.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gjstghppl.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwikjssqu.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhkcfetq.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjodvujee.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdyucmvu.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gcfihwyql.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsiqysgm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqdzhtwr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gezxanxcb.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmegtvypk.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncdqdcdd.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gblftnqco.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gwbksyiba.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubotknhs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjkbjopz.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gesmnordm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gnsgspthx.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/guiguxxmc.sHtML


<!-- 参考信息 -->