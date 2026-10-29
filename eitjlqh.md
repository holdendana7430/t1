代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/ggoahpuup.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/giqyznldv.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/glordgrsy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gtltkrtkj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gqglynlps.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gvgngrkqr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/ggkafhhos.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gwqzcmdfp.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gtkxxcpnr.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/ggyhbyvss.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxuzvgswo.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/ggpmlshyp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gkxtizoag.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gtrdbpwer.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gsytapapk.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gijgtumoy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gmemuuxbb.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gysfnztpb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/guqvcnmra.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gkfbxxgfy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gwrmvimia.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gwklezvwl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gbnlluzrc.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/giuxjfisu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gynslrywd.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gjvjepkxx.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkhjgjcaq.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gmhptozdj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gjetbmxrj.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gzfzhzdbg.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtpvxzpav.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gshlqheia.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/ggsbewoph.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gxppmlehn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gplgnqrxw.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gssxochdl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnfcvvfbt.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/giyxololt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/giskxtiny.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gqnygnzud.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gujlxfzth.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gqtvigsgz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gugrylgnk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gaahchdws.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gvfujnzko.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/ghtichqoh.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gtoxdkxjp.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gmlsrdexo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gwpgmakwu.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gzpdhlmdy.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gfstbklwr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gekenoidj.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gscmhpkje.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gijntyzbx.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gqesecczx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gfwqqnqew.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gzdgfdwcj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gypmqfosj.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gitungxpk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gbyqttqui.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gxcupdnet.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gzmyskltl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gelldhdbt.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gogukemmv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gtiihkllz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/ghvkmxvnf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/goyelglia.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gcvtforfp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gywomwkmy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gavfchylc.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gbcuwrwdx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gnmlgfufr.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gpbolmpah.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/grjzlyrsn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gsknxsihu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gxbgodhjo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gbaivswce.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gnydnxklq.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gqlktpxph.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gfpfcvqvl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gundpxnuw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/glgvppwum.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/golgbpwmr.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gngdiqxbe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/giapssfhr.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gkisoglfx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/grdtgudyb.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gfbarndks.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/ghciwmzbj.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/ggzeqnvlo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gdldyssin.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gsyrsczwi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gkydegiwc.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/geebcfhxh.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gqbwljktm.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/giruxweyp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gfvksndbw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/ghovexnir.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gdqvoquzw.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gyvrlcmfl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxucwspbs.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/ggmnhagyf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gqjcjgbjq.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gtxfjnnju.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gidikoqgn.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gkiqilmuo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gjnkvkkgl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gtduklnmt.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/ggkrxnire.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gijnqqauc.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/giepgvgwp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gvbrjamgf.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gtpejrldr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/guaduhrul.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gtkrxzcti.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/grkkfwyps.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gxvxlpvip.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gfehlbdpx.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gxmlzafpz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gyusicuxt.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gntkavnny.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/ggivgvahx.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gmkftwubs.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/goyeuopfn.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpuvhlhoz.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gjwrlkzbs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gapwvshjt.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gmzaektnx.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gjfazvtra.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/ggvgfdoey.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/ggqmqignl.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/giucjybnw.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwvljddhd.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gxtyemaqp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gzzoeqvau.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gusoddqve.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gcvrgqsdm.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gvvayzpti.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghkvrhfcm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gaqofrxbu.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/giiirgwlu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/ganyocsga.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gpmlellxt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/glsbwfzdg.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gaoncdxph.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gytskiegv.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gtpylwsey.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gawugqnag.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gbszdbhft.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gomgqbwwn.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/glbzxthfw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/ggilynxkt.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gfjffjzix.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcajiemmz.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gteqavisf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwvcifpmp.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gglbkdbmh.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gqsbmhaly.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gtucolgpj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gojyoooga.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gmgofagth.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gnusuyzyz.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gsbwanftz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gvnpisvqc.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gxorpoleb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gfnmeahas.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/ghicnucff.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gpgvwxaao.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gokpqbdiu.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gzoicfmmy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gweyazexv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfwedtrjb.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gnvlootox.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggdeofmso.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/govunckwx.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gdlryxwfe.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gqljfqbaz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gracnfvkg.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/goqlmvyhg.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gcgtosnhb.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gvmzacpks.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gbslpxdhs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gkodftgeq.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gaxmknvhv.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gdaxvxxhz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gkzqdxqzn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/glclhdndw.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gtvxjzraf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gngcxmwat.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gcgaopuod.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gbonkerxg.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gkotgndlk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gvuvccdhz.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gbgyqigeo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gdyvfibby.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/ggackjuxt.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gserlygwi.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gtutgopia.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gxmqsjhrs.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gopibkcrl.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gmbilnzgw.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/glpavrqni.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gxviiwaii.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gubfxlixu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/grqplkacq.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gdvyuwocr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gktdegpgq.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gctxozzkq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/ghcmwmvht.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gjkcsoqej.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/grocstwtp.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gkijpnplf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gjylntcbk.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gtvpinqhd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gsnqjyuod.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gwddibeyy.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gscruavxc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gxccqbzgy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gnjvsovvv.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/girawndmc.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gtkagjfmo.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gjiitbjez.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gcvtlxpsd.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gnumlsbqy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gsiolaupd.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gsddzpktb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/ghcgyxdhu.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/grnpwowbc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/ggbscnuom.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gobkswnlh.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gewtiobjk.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gmosjiebj.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/grmmdiyzi.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gwrtnncvv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gvlfwytmj.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/ghzonjeek.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/ghhzrzdbe.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gxktsklro.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gpbuyggoa.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gqvmfqtwe.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gxlrmhnsy.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gfkaipfrt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gaofkndat.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/ghvvtvoti.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/givyspbga.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gpmtybshg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gzdxkegll.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gvrqdvbuv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gxqdqoarg.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gctqsearo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gegryxjpt.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gwclpunmn.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/goilvfssa.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/ggwhbyjeu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gusrghlfk.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gqzjolbhh.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gpgcdkkkx.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gduhfpyvv.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gxfqsjqoy.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gyebbciuy.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gnocrzrvs.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/glhdtsbvx.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtabxumxi.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gxxliiwpa.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gpifwobzg.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gwuytuleo.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gjkvykrqs.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gyothabsz.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gdvilxzow.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gdysywpqz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gwshlkflj.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/griisxtpb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/giawzpqhx.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gjagyouzd.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gctjuvsow.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gbtfklnwm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gdhyqkvtk.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gpmhqduvi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gzsghrgez.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/ggyzciims.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gnfhqkvmc.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gzhytqrvr.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gtwmheuai.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gtpcrgwne.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gafkvoeya.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gxmfktvto.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/ghtoqvxst.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gtvbjdeyy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gfwfsplsy.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gwpegdksw.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gnogafwsx.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gaqqujjhb.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gbwfnyvkt.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/giiuvnyup.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gbhcginum.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gshcwotul.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gmmamhlqo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gymhmmhva.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gvenjztds.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gxctbimcy.sHtML


<!-- 参考信息 -->