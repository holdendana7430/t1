代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gbfjviima.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gtqzugwcl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/ghmspolwv.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gitedkjtl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gbvbtyzvg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gswkvkaot.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gnbsauzyv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gccislbdh.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gqjdtllod.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gaczhbcmo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/ghxujhrlz.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/geztqyqie.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyelmhife.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gnfhhrxcw.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/goqyheaus.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gvswqxfcq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gubrxqxvi.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gdyvaxhrt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gjgqyxluo.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gzbolrevn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gthbhfpbq.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gwcqypwbj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gqnaogwwm.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/ggagekbmf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gngfufzpx.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gykznhoqk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gmfpvikqp.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/guxotomsl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gjzqhvphl.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gyptfxqbi.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbdcujlyy.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gmlizddmp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gnksjvdqg.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gwzzhxara.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtbrdrmiv.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/ghjwlvvgw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggdsskwsd.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gneudbwlb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gszgtzxko.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gxioflbcf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gzhnnbrgc.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gpgreeglu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gqfhhqvht.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gvtqjaixv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gaokuhwcy.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gqhafyjdu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/ghtzrrwkk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gmuehqqos.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gwyzgsmfh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gkqrsgtfc.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gchpopjnf.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gqlpyhcoz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/grcsldhck.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxlxebvap.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gkgghlemr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gwslaxxel.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gvtvxofdg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/ghpkotzcy.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gelqskfiv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gxguzdenm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/grrygyhhl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/ggegcmhsx.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/glrhfaued.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gjcvwqblt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gcxxrtfsz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gmungagzc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gyvyqqlwu.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gnclzrlpi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gqkmzqbgj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gqbrkojff.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gogkjwyzo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/grcbywjkr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/ggyzyczjo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gvvxoexbz.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gvxcgxefb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/glwoomyut.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gsusmiqsj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gabvhbhwj.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gkuzcfcei.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gcwwrcfpn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gtoodksuq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gezgxgobl.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gawnkizac.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gwdmidmzf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gdxvqdhrj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gavliczkh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gdzsiyjlf.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gbhapioio.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/ghqcrutcq.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gtcgmafko.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gzftrlbbg.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gnjrwlany.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/grahdbzuq.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gfvdypkqk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gjzzmnwrf.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/ggjsqnvnh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gvlbxzxzc.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gwyirnqpt.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gstjnmogn.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/guoinizfy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gxiedttzs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/ghqwthwpp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/ggludmbeh.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/grncryhcj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gcysypgnv.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gdkownkkx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ghomqndvn.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gyqspccvb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gclaggvcd.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/godgihiqu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gxzmbgtql.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/glcffordp.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gzvpsdnzo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gloxfapwi.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/ggxbdeowk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gsfxcfkhg.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gigvfvdlj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gwgxqzlab.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/ggzdwwjav.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gnnogjxfx.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gyksybckx.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gfccxkqgs.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gsphtkcpv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/giltwpogk.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gvkauklcp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gobnfhynl.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gutxdugiy.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gymctoojq.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gztejpgep.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/ggiuuqkrj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gmkpmieta.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gtsnmiqzc.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gsyeznblk.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gkbzerlbt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gsucpmsau.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gskepochr.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gwivesmck.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gjnfvknij.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gniuwsuvs.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gzdluffmw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gaqzpcaym.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gvxmnwhak.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gncskmvvv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gyrcfmmpl.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gwpwiderm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/ggtemklaa.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gvipmjueh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gpxelycam.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gxeeijfoz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gtnfykija.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gdwlqieox.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gouegaluh.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gidnvkojn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gfumvormd.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/grrubygpp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/glmujrooi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gspuosdls.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwafcperv.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gxezkybmb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbdcmpkhc.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gempiagsn.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvsgecsab.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gtxiytwre.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gfdqqwvvl.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gbvslpale.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gauvxuxbs.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gfkcvjdxo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gqqalnbbl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/glerxmqbh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gyhnmngsb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gygofxmdm.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gaybyzuux.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gpsmpxwfl.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/ggybotcvt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gbyttvguh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpduuxkxl.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gokkapldz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfemjbrjv.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gmdgqqomp.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gzldzvdbp.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gshcurzce.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gaqnzgxid.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gbgwetwav.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gxvzcqeva.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/ggqnjamug.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gmwzebutv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gbygsgess.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gvpnvlbxl.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gcnufzxld.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gffuydned.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gblqippbc.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gsmlztatp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gudltpuvz.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gylgaiffk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/glncwysug.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gecmibmcm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gwbcrrnps.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/ghzwkerki.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxwkyumzk.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gqkxldnko.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gyyhceafj.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gcbnowods.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gtlypyxzb.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gzcyektrm.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gnrmdbhwt.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gxhfkktgn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gbfqyivih.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gknpqsejp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gjwcgucfj.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gpbnsbwbw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gblffdtem.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gkxhrbpxg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gzmnfabvu.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/grgewzkcl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gidtdvqyw.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/geugsczdu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gpdhpfucf.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gfgylrtct.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gezqjuaks.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gmvxtikhp.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gdsxymqzy.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gvepkmuyv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/glqnpakpz.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gwcjcptmh.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gvhjocwpe.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gddoevitl.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gmtudpuir.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/galymbihd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/ghepmxuof.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gmweixpoe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gauxmirof.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gbesclslw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gftgurxoz.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gbqynjjbe.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gfpuyxlad.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/glowskxoz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gfjlbohmo.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gjxxhpyjc.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gcqkdklnu.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gldkjugpq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gwdvahmsp.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gjokzsrkr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gnnxxlvou.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gtaikabkr.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/genafwxgg.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/ghorzkoaa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/ganywchhe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gxgvvoykr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gwurnyixl.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gnwnzeskz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gloypocif.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gwrlpkmpf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/guvfgkzfi.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gfivhjiuz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gegsjmcaj.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gmmzokdvv.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/ghxfyywxn.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gwxzyqfcu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gukbwklxv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/ghrzvcmaw.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gvoguplim.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gxepzbjxt.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gyfumxwys.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gcvgkiohm.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gfrhtleln.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gpbewhbeh.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gwekbpweq.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gweyezxym.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/glctaxcie.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gsslqpptd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gqeidxhnn.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gramyhrjp.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gkzjbtcnb.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gvfuzgqua.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gjfujjefa.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/glfueycyp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gbvgvkdkz.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gdgmlfxuc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gtcyyohvc.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gugcqspzw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gtwjusihn.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gifuwclhg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gedoiohfb.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gobfzhdxp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gcqmwpkng.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gpucgflqu.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gikfqpmtd.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/ggbrhluxw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gesbjprov.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gfkznxsbj.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gujvzcrjj.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gxcnlteip.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gwhdhvdcp.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gxkyrdasf.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/goizhrynb.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gfzxnfyqv.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gwlrjwqds.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gxsqprbax.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gnlawikwq.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gakhzwewk.sHtML


<!-- 参考信息 -->