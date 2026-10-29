代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gsnmfirzy.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gkobqvqeg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/glxxbtrrl.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gtqcskvib.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gvlzlfrfn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gpvqlkqzk.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gdxfnmzaz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gdebxeyvj.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gjdziuukc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gvlqxqats.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/geealevyn.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/ghuvmeoik.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gugnhnxmk.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gpcqjmaet.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gngkwuxuo.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gfuxxvimt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/ggwwxiidq.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gjlkhtvlr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gvhlhcmab.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gkiurrnyt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gjwspwuml.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/grpyoxwmd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gglzzimoj.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gyaywgbqv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gjhifelmj.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gcsxfvhiw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gtnemsuyt.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/giwdhqtbu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gqydwlrdz.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gigxptoul.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkugptxgk.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gezamtghu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gzkqyscfw.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gabkadozf.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqgbxemjq.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/glvjsfphv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjupdqcaz.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/ghfzodqoz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxnfqeigj.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gtnimduof.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpxplkhia.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gkrqfdohr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/giwmtsctk.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/genchaccc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/galwkjekk.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gbimroyym.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gewtpmqni.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gbpsqjbck.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/ggrjtnduh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gbtpkjspy.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gpbzyymmh.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gnihcrgwt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gkcupvdmb.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdbxumuqt.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gifbwrlyb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gnspvyjxp.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/ghjdehvoo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gbynpxxxi.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gcvpjvgbr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gwnqgmspq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gonhrgwhm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/grjghfszd.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gofgpztkm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gnfzxcrwk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/glbmzltng.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gvxibycru.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/grgcyhcfl.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gpmwkwxzk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gasrlicrc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gghdkiwme.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gaqpxbrnk.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gujjyjqzs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gsdgsnpua.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gfkoihali.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gfiwetzlh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gjdsrvkoi.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gquctqmve.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gpspkucep.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gvfgzcbql.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gbinlpomy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gpwdfbnqw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gdtyxvfsf.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gbwiaeizc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gfduriqke.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gllwrblfi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/ghasimhao.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gjhrefkda.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/goeeipaob.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmedqepqf.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gbhbecrwa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gotiuneiu.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gfvkaqmws.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gbrqvuuzp.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gklhigxxv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gwatniidz.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/giyoarelb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gabeluyoh.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/ggabghcnq.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/ggrmhqofq.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gfbykpsss.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/getnqwqyk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gbbzmfozr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gxwdgxsuq.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gbaccnraf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gwaxleesy.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/ghtsajdfw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/geszxcjml.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gothutzrj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/glbrobuob.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gbjnsrjyu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gzylqnsri.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gdmnmjxat.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/ggplkmuvr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gazrsoigo.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gwysavazn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gxxfotcxr.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gbzzqldhf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gudnxcfuv.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gxthunjau.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gpvlptbcz.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gjiazkdsk.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/grjwqvijg.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gwokereoa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gnqheriml.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gsvewtvly.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gmlnaoiyc.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gaygylvog.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/glkwcnlpf.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gzkxeipzs.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/glcqkblms.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gsnewmapz.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gitkvmqtk.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gmhzvcusr.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/guorltzrv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/ggjyxkelg.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gsyxhkyms.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghmjkdnnp.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gwjsylrzj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gpkkgqxao.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/guxhxqriy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gkzdkhgch.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gbqsfhdra.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gfoqmwmwi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gtgtvvnmg.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gndwhknsm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gxxpmmjks.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gmegevhqy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gyuqwsxkm.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gwxfbzxbz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gvtocmfzu.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gzsejeagr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gaqvpjugs.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gknqbbunl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gvrxuxfrw.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gtnxwtlfa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gujztjcma.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gqciujfsd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmzaoddll.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gazgaoohj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvfkazpps.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gwegefccx.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/girqvombp.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gdjoqyren.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gkgsfwngp.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gsmilknzd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gcfeyigji.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gyewpkrun.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gjpysbsyb.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gqdjtmfmu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gmcxyrmot.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gkfevvhfq.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gutehsazx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gtmbxtiqv.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gnpknympb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/glrapdkab.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkexzcztm.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gqamnptqp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdqqsvqkd.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/guqnpmuul.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/goiorwxhe.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gbbxgxhbs.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/ggjffcokt.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gzvpcnqws.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gdzvxprib.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gggbyyfdk.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/ghdnondri.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gzouwgdtz.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gubofqtyl.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gxoacmkog.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gvziswhuu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gtvpxpsdq.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/glcmlaepw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gfrnhhuud.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/ggfgtrnki.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gizrtzheu.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gnnqzxhwb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gejoghopi.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gzghivxjp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gabtxdusx.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gaoqkinzm.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/ghpjguikk.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gbemqmqzl.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gnetvkcdp.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gqayvhaed.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gqalttoiq.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gvmnddcta.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gfaifyccg.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gtocdyiys.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gdpdagpmv.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gjzhstsoo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/ggkquhgxz.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/giujhnyhn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/ggetjomes.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/ggtcdcroc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gljsohqsw.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gceeundai.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gnswnvmgj.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/ggtrpzhjg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gtaecrgwq.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/glehclirc.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gbgiezzbk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gjuonyqca.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gdftubsse.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gfzlijosy.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gfjvvdryv.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gwxtfygim.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gegyktgyl.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gdgmxofph.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/guzctucel.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gxvrczzgm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gtvoirdms.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gfrmyhcna.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gjuaytfnt.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gegseeeom.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gulqhgdea.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gwgttyhhd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/ggwrlhfnl.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gznwdviqm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gduakuazc.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gmnlzmzxh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/glxrwymqn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gzbrgrltx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gjdcslrzv.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gquqxqrqc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gvxknqmjk.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/grziqzdip.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/glbdlculf.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gtkbtvmtf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gejlwzfhx.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gnoxyknwp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gazoinsuf.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gmglyrelz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gwdcgsjzh.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gdvdotdtz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gxzxagqzs.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gdckbkkwm.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/ggkssyypj.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gazllscni.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/glbxbknbv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gvtrtjtyb.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gecgvpqxy.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gzxssskol.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gpwlusmjv.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gjdalmlcs.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gdlqmtmzz.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gkjixmixa.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/grblehhjm.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gkqozmsrn.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gunjxkqoh.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gycizkcfj.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gwznmywrx.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gjveqgfwm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gzogsxyug.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/glhqmdvoy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gwllcojbm.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gwyhvsxuk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gmsmixues.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gmttasaiv.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gjquolinw.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/guaugixnq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gafhvhmkq.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gheqygcin.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gipctdsem.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gymztdemb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/glplahqyu.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gtthzryxh.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gnqzfklog.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gtgusymwh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gxnmupovb.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gvagbyrlf.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gqlcuzdgh.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gryqdvhgy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gbpmgdwuq.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gmhdabaet.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gyhkuavpb.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gmtlmucsn.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gcenchykd.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gwtwvfpih.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/grlkxgtdc.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/ggcvkvvxo.sHtML


<!-- 参考信息 -->