代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gzlhrmkrj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gurcrjotc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gurlowypz.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gcfykqazc.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gzfrncdeh.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gvywwejyo.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gknmlcuur.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/ghnrshdhy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxprapfqy.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gsffipcqo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gubfnrxdm.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/grmstbrgt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/ghxhjgmrj.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/glvzvukje.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gthqabggx.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gytxrxwyy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gqbhednmw.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gxvbegwax.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gonyqoelj.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/guuocjwrd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gkvbyxkko.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/genbrigbb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcjjjoswf.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gkjbngwbs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gujiemwjc.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gfqgmrndr.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gpfxrlics.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/ghhednasc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gojexkvdj.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gvicydinv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/grvtvkqtr.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/grcqndyka.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcvacnpkh.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gztfzvpbu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gllvdoixj.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gxzifbxlt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gkpvtnshj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gflnuhgcj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gkfftsgyz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gbgczgjxd.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gzdoasfmn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/guhoqinhx.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gvvvtctnc.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gyfguceht.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gixwhczit.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/geniurntq.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gdomabopx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gbxfszmoh.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gylbidckx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gokpkmobv.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/grvwpivjj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gnvqnxumw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gmzumhdot.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gotsepfyf.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gryvsfzrf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gaoqfaqum.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gdkagkpvd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gaesathky.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gvtwnqqyw.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gwbzsejpu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/ggwfltgkr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gooxptajf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/ghxzfgbet.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gcldvmuia.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gysphdplw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gztdqzvtu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gqgkbsyna.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gxvoeqmxx.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gonpyslav.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gzbmtlxrf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gecchqsob.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gvqubknze.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/grnjyfxls.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gejiwksmf.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gstcolsfy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gdihzypbi.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gbvvripad.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gbrsusnyh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gzbddufni.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gvlcfbxqe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/geybhjphf.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gjyvtisng.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gmddunxfd.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gkbkkgfqz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gjevrgpfl.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gafinfdjr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gvvixukub.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/ggzhtesxh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gcoqswsqv.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/ggrexoccq.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/grkmhqddr.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/grnxistos.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gqydeqdym.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gvrdvknew.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gzeugelkt.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/ggjoanupn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvslfqtuj.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gldcorolc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gscqgjkwe.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gywacogdc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gyzrmlvrr.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gnfzjdpjg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gpvgzxyys.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/glbkzwxus.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gscgckyim.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxnzeonlh.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gvnxkmcla.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gmqvslnem.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gfckucmwc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/govhucwib.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gxsbruggu.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gpjowyfng.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gorkobuua.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gwuicisbp.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gashdyukf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gprbndimh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/glsanhern.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/grgrnlqal.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gdqtwhvrz.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gllkdbrcv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gaqdsxfrx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gvqcxqlas.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gyuiveetu.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/ggsrttwrs.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gtaaaloip.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/grrjghevd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gzxqjsphm.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gcedrqlyu.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gvulvzlfg.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/ghbheszgr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gywtvoxyd.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gstkxtwoo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gouxdnmlx.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gnuxxckcp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gixukkdxp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gzyqcqfcz.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gyhargagc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gzdaypach.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/ghkuggnvk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gtatltyej.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gsyjjixdu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gelqlgkrc.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/glpbecnkw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gegildmau.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gfgiwuxjf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gffydwkdz.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gopxhgkbx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbmcowovp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/ghodyqckl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gaybzgflm.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gqmnloqpg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcqpxrhgb.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gwfsasutd.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/geyjtjven.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gjnbsaaag.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gsrvoqiyv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gqvkytsqq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/ghyztnfka.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gyjkpjrzp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gxevkwznv.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gypmtglmt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gsibfuuan.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzzpumryq.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/glqvwxnik.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gvmlbyzfd.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/ggmgevofz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gfddeutbt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gehaqrowd.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gyxmgkmxo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpekbjmva.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gsrinojdi.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gpoyontyl.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gpkkkjpab.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gcnnhozxn.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/goowozgtk.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gstgzvyxy.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gdxslgzye.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gxabipztc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/ghjgciodg.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gqhdwjwmu.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/glzvvocrp.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/giivjnjrl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gtyhxzicm.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/grmbfiufr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gsikvstmm.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gpxaaowot.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gtmgvkftj.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gamorgeim.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/grfvrbvfw.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/glowwwvjc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdaqfodsq.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gnyrfjlar.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/griqifsmp.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gktlimriz.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gvtjtjvqu.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/godwlncxj.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gftissrbo.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gncxdxcau.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/galqfvfna.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gendtztrc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gjyeqglwt.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gknfnyiet.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gvnijanot.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gngbbfreh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gpfxfsawj.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gdbusrxuu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gyqszxuas.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/ghdgovnee.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gacnmwmee.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gbeeqzhjr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gxlgztbce.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/guxggndwq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gwijpguls.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gutlkevdz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gilpkkgua.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/glmbkkphm.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gqxxdrzjm.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gjrrhhgka.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gzbnlhzgd.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gdzwlkphq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gecbnkesn.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gadmckmzh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gkjanvvnc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gaiduquij.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gpcnroyxn.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gendgmfmo.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gdjfczyqn.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gwgjrhaqa.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/ggihzoexq.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gwdswajqc.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/garbxbczb.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gvozsjatc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gpvgivtlk.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gvvfdhcif.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gaqdeggaz.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gcabvdcrr.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gaznrlfav.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gfrqezgzp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/ggjkiszza.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gthqijxge.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gdkattrxo.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gpgjwjndk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gzgcyohpg.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gghhhigsr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gfxzviofu.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gaoviuevz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gpynxtwjk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/glrecyhsb.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gmfqoggyw.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gxjnliesu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gnvufldft.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/guvvwvuel.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gclloayws.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gaixjvuwt.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gqkzffinq.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gsaflbmxt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gpwdhjsre.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gpbligior.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/glsncpjtr.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/grjoqfqzl.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gqyticmfx.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gjxdokbql.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gchsizimq.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gztjmdqwd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gcbeqvnkx.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gdfdcmxxw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gxonbodzn.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gbwvpfrms.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gyvwpmpil.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gdyiaaqym.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghfmrvppl.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gsngpwfet.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gxjlopetl.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gnydcxjzx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gjihvscgn.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/ggpjryhgw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gumsygbpk.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gizmdtqwq.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gokgklrnt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gatunmvqg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gotmaxxfx.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/ghaupklbs.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gioriavjw.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gfgteoqaq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/glkowbdni.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gugauvrxk.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/godqfmxwu.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/ghwlewgnj.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gtngiukqh.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gbujfvjyk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gfpltrdqk.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gtvtxpsyn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gacfnnxmr.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gajdadelv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gxstlzvhj.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/guhlvtkpn.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gnsmytbns.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/geqsmbtma.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gaylnfhds.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gggckfiux.sHtML


<!-- 参考信息 -->