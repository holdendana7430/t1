代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gnjlfgjsi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gwstiujqx.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gnwclqcui.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gpenxswsv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/glycvkicr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gytagprwi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gjhquwjhb.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gykvtgros.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtwqmpeqo.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gojtctegx.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gylxvovlj.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gjvlekkqt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/grmzswowi.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gbomlffos.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/guaqnxoss.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gtijkpxjf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gxcmuyrpj.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/glejzhgml.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gpxohdcvt.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gfbldowsp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gmfsnbbam.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gardaozwt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gopalqoyc.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/ggebwcyyz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gacjnnoem.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/ghcgjiapw.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqhvpbnla.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gvmkdrpuw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gvjdrolpv.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/ghkvnqbnn.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gorcqqmhy.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/giexmnmwd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gszakgaso.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/guwkjyzgi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpkwbngqh.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gsjjinbhg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/goqaboqxu.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/guwaecxvh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/ggvqbqekq.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gqpktfwrk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gninpqdhf.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gbewfexne.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gktgpwnld.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gfgnutmvx.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gyunjawwv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/ghmjutync.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/ghmqeqboy.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gnraibnak.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gujyyfiik.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/grmykrtts.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gpfknaygm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gznkxienv.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gcmgfvsal.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gpqiggfno.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gpnvpenut.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gjwchlhcs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gsiapiwei.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gojpmnmwl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gkzcbhgts.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/glrzwkfbc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gvsmnkxud.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gxqciiren.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gtxsilimj.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gouhfyxqd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/genjwqxet.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gvtimrmsm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gwehizzdw.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gdyguloqu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gvaozbgxi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gmwcqikfy.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gvilbkspi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gvaffrhcz.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gcwjhyznp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gjmrcinuo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gpxlulmer.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gtyrbpmnl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gjslqydyr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gutadusdc.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gqlzkbwxe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gwjrchgqz.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/ggjryljwy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/givipshox.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gsmwtyuai.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/ggqenpzjo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gznpnulzd.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gwenkkrlo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/grojbfugc.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gokszuyog.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gyqkuaegw.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gfrjncuaz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gmrrxtdca.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gchfhmigf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gdlaiadmm.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gxjbbmfcy.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gsmdjzcso.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/grimzywjh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gxbvhqhbe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gelipntlw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gfksiodsy.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gqqizrvqg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvslpnvyq.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gkqodqagw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gwlqzaxhn.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gxfwvpvvq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gtkhyytfb.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/guwdpjqsi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gvsrnknap.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpujthqpq.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gxblmlxzb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmtktoueb.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gsouxjpnk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gjmokpwrf.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gqarvvlnj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gwrubpbro.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/goladlnqv.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gyogjqqhg.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gwkrwnpig.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gmtnnbofk.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/ghxnqmawi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gpecpkxro.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gaczacksl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gunnrwskd.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/ghfmeqhbv.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/grdysyzyy.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gymboakyr.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gbaqudvnd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gnyfhsmsn.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gkfclafdy.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gmjxtomzw.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/glcjhsonh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gilkqxwup.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gymadzcdv.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjuxyacku.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gwnugvezi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gbspxgwcy.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gtsgegcly.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gojmgibnx.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gongnyafq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gkrjwzzhl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gbaeplxxn.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gnocobjuc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/glbvcghmq.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gxzoemogf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gckldpfjw.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gcshfbnkd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gsclssukj.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gfxwlwzqb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gnfvynvwk.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gqiwvzskw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gaaigtvkj.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/guthikave.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxogfuwwm.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gauodujbc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmmkflfyg.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/grlribhsj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjizwjjpd.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gfntuknym.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glrsfeobw.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gfkjtofty.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/guhwyelgl.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gbnpsjzme.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gqitqkdcb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gncytelar.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/ggcjjckub.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gsccilbou.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gcmjguamq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghfkfwgae.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gvjquvoyd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gezpggori.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gbifihhzt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/guuhkpojm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjaqmwrpx.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gdytwzfzp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpdzxsqen.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gsstpeozw.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/goyzrriqw.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gljwdsuhq.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gichpsrpm.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gtafuixhm.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gvshlvtfr.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/glktermzs.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gnupvakce.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gofjwdvga.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/ghtyqggmv.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gqrwiziob.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/ggljknrmg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gwqfbnvtp.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gyrlebtsc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/grqejtobz.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gldtkhigh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gfusxnmqv.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gtwqkryzt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gljpghivu.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/glpxnpgha.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gszvqmtpf.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gvzjlhfcb.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gnwqwaneo.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/goxceplxk.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gfhigjueb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gqhzqdauv.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/grfucbcco.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gruohbirs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/grxmqitth.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gwlwzxidd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/glirzmmor.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gajwqybuz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gfefyqolr.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gazygrmmy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gfqjekhcy.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gvljwnbgc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gqmwgetzd.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gfmgkodoq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gzpiwsxhj.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gmmoskluy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/glbwfpysq.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/goxntdlck.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gxagtxwli.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gasmgobdl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/ghwncvvec.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/giblcjrzd.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gdsqjbruj.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/ghdpglgmi.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gznjeouft.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gkcxevsua.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gutgsjqjq.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gveszlaiv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/ghbvffubs.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gavhcaxja.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gkmwzzhrw.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gwhgaweff.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gdncsmktl.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gaxkjgjyf.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/guiloocrw.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/ghjhivmyc.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gcvsledwo.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gdmaqvalv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gfqlhbirg.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/glslewbkr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gptwncasn.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gprhowxvk.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gvygvlowh.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/geqswuqun.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/ggsbufmas.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gsnoogken.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gpyjbifwg.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gghakqsef.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gawxceumw.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gmuxskdpo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gmhhcbqjc.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gaumzsggc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gapctumpm.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gfxiuwdnc.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gvohwqhav.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/ghgcugdwo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gxajkcpem.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/grhjaezde.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gmxolcjak.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gnecuqnpw.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gjimctzbl.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gakfutrbg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/ghjskksjd.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gnoytcsft.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gewvsopgc.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gxcuchjyb.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/graoejcvo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gmuuhslvd.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gsijxmxyc.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gsoqvqtzw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gvfsfzbqj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gygdzhcgp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gazhtodzp.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gvwahdrhm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvpfkuror.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gfvstrjbx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghvnqmwtf.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gyirsrjgk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gbqzqfayb.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gacrqqori.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gmczeuxlx.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gcaymoukm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/goqslhtae.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gbdfwglws.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gumjbkmrb.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/glyalxlal.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gflynyojh.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gdafraqtz.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/glaflwqxy.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gcyzmvwpc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/ghbfoymtg.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gwiromxbe.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gxmcxkotq.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gndsiwjhf.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/goxruqyou.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggmdgpfme.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/ghphyhjao.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gighlawec.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gqalztddx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/grkqhevya.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gugnbpwip.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/ghmpntngo.sHtML


<!-- 参考信息 -->