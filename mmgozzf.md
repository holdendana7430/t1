代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrvgmsdt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvbgxmni.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gaudgyicw.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyfvomsj.sHtML

SELECT * FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzxqbnxbt.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqqhhhvm.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghldmoew.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqubrchq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/giiixgkce.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/giywwtndt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwyxdofr.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gopdnqvqt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/grdtnmulx.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gzihatjon.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gitzruulc.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gghnxzkpj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gliiogbws.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/grjgihril.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbihxdnd.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gxktbdmzd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwogigaf.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/ggudzqqni.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnddycjcc.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqqszgob.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtmzlyma.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxktzwrcs.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gupxobbau.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/gzcdsrwwt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gotvwznev.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gpnkarapg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gerfolugq.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/goreuoiqc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgcxcybu.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gmybyvlji.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gptiwkyiu.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/grcioogrv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcoyidsd.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxgjvndss.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxsysxth.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgxkyzgr.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gglmiluap.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtijcemxe.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gukxwayqc.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbupvgslj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiipaufd.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjlzhtjv.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfojjjbl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/glgqrnqab.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gjcpgfgjh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpnkynld.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzrdcjpn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfskikuse.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gvpiduxdd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyhqhctn.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gomahppln.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjebxjfp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gjtdwnuxq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoqwbuqn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gddcyahee.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gqgvrjrgl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gutskresk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gncvhstdx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvvmbsiu.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gfzhehqov.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gaxmxogel.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxucyufxt.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/guzjligdp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gknmshyfk.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/giuwtwbja.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/goewgcrrw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzobinkz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghulgxbal.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzzjsvnr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/ggafhoyop.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gvsnyymbg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gizwoqeqs.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgabpuje.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giygrecce.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gqtxcjltb.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gqnzpxyjp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggojhsykq.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gtduuiwmw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gifuvlwav.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbzkncct.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gimzcpssx.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwfsokoa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gtcjtamzy.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/glnkmcwco.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gshesyvfw.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gblzyucxy.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gmsqqlacr.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/grzsewswl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gfrtpfots.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulmghsye.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gewgkqaec.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gozmlfjpm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtogvcbug.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmmgcbaq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuezdhtn.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlsnyjwa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpirkskan.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gmglupsot.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkmmisbd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtnphncf.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gmdigpyud.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gqycirosx.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnzwubar.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gklnngloy.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/ghojvzoqo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gseseylef.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpjrypvv.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzavzjkx.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtleesnr.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gpkpjllxn.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/ghmrqgsee.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlndccxu.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfncqwfnh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/grkeqawxe.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlaucsdl.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gfhmfayrr.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyienzrja.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gxxtcbiya.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gcnpidzdv.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmearnjv.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/geupcmlxw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grthfgqlj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gtrfxcgvp.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gefwupbvp.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glhdiualm.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/ghyrpiumd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/geancfruq.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrxwjqxf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gvrwopdca.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gmjfsqeta.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxrmqacw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gjwndunhz.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/guwyhjzmg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gebghxtls.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gmyusdtok.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gbepunrlz.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gkovcwcvi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjobqodxm.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gmliaitbl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdnlhdxv.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdflokqn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjpkunte.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsdxyqhx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzhqjnde.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtkgiapf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwtevcsz.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gysdihdok.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/geylsgssr.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gawsjyhni.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzfteuzcx.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gawdfakak.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmjklinf.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxydhieu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gvzqyjuec.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gddpoabnr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/grzmxbxxl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gbwskohje.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghziqosjt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhdwuuse.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggblnuudp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/ghlppmyab.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gaciagvhh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprybqesn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtuyfxoxq.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gumcmzjpv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkatgzaf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gevkgwabo.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgdcgesg.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gxzusoxgr.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gmpydeyfm.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwugcwogj.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzriqpova.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyaelvih.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwauzkjs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbucdwwk.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzclkliuq.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtxmgcuwe.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gtziufrap.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnrgngee.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gaihniula.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gtdbcgzol.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gomhzibbh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gkspwfwpg.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gntjqqxbf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlhvdnkw.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcevbffv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewwfitkj.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyewognwt.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gofafjqhd.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpjvlemz.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gzqipetyn.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzgxbzgr.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gkpnwmpem.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/guvajbaoa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghrsfpiga.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/ghssqsikd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnfvzjec.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gycqntrpn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzohyoiq.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gywupbpal.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/galsvgfur.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gppetzajy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/glosdifxj.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gmxjlvhxd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsmtfeuq.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoietcfm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhphvxnh.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwyrkxwi.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbhbtkvu.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjefyekn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzkhmsod.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gugqnngox.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixgsltzw.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfyilymt.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/geposyeio.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoaextdz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsfrqxcxr.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqpagnvl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glgxrumyo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvateepz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnwqujokk.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyddtnglh.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gemoilmet.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwzlxcvg.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/guuuyueyw.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gorgnrnug.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gaczpcxti.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmmvdenho.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gojxxwaip.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvizukjkj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glogtaayr.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gltqksass.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbzehmjl.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokbwzkqt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhonesum.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/ghvbccise.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gaboadrzz.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gsszquhte.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/guwqktxuv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdesmnqem.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdumwmlgb.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gskfrfscb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gynnsqrjw.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/glvvzszqm.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrpaesnh.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gfhiyfgcg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gicbqdgin.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcmgpykz.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ghhzmqelk.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgqpuvtg.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthvhhuwf.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqwbfgqc.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueduoaij.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzgddzcm.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqeqckros.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnjddcpp.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/givcrrrqz.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzargktv.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gsktdafqj.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/grojdddkt.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/giexzhqyk.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvpongbb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaisxlko.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzndqsca.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgvieqet.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdamdogjt.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpmzyqlt.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzltxbtat.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/guwbchnrc.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gypgplvcd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzjzabjb.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcyfxvex.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gwbaeqdxh.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gypcmrlqk.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxstpcnez.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwbceodu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwabtawak.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatjesyrv.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwisziecb.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goffxszwi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gtukzgtib.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ghakaiifc.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gszjtauof.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gtilkfrpb.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxikorazp.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtquahgiu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/ghmlbxvfz.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeokdlrv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/goqxveegv.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gtgqovbgg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkaryebm.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrbvwlnw.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gtzenmxwx.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkbbghjxk.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/goakuvfag.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gtrblmqiv.sHtML


<!-- 参考信息 -->