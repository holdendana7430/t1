代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gjxrcvmqf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gcdkhsuml.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gkclgffyj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/guxjyapts.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/glgryigeo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gdjrvdkom.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/glzyzsokp.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gwoexejbp.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/glcuqdjpb.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gkhcsaezl.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzhhcmfmg.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gfkdclhqj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gimtlfscz.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/geilljaqe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gqzsujhap.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gyouufdst.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/ghduxdofy.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gwvfqwxdo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gcbpwurwp.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gxmphmjrs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gmiovexjt.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gubzfegok.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/geidmkzds.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gtmhpywzw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gmmodruay.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gbymyjonp.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gsrorsexu.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gcasykmez.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gjbzukpox.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gvpjwudio.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjudibnba.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gsdvixrcf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gahjvauft.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gxybmlufj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ggypjknmi.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gqsqvybcy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggypeygkd.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gkfdierrv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gpukejkem.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/ggbnsagbe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gbetlpqtd.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gxcdwmxxz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gglfthjql.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gibtoyzxn.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gxprqlnmf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gnnzxkqik.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gkhxgonjz.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gegribadr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gmgmtdibn.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/glwrdietn.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gbmxuwykv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gutmvbkqo.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gfqstwpub.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gmdnyytph.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gplzdvfbf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gdhnlgvxw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gprmgutkz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gedxdgibk.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gvqnasats.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gaawedydy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gkdjyaabk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gxszliiax.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gvqonmdut.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gyktnwfxh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gbbdamfhv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/goldycpef.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gjzhjqgqj.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gnlmmjqah.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gvtejbabe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gujoedtar.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gkpjoawpu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/ggegsmgoc.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gvbxwoqxm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gaezjpxwx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gosbgmbhj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gmqcjefzr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gmqjkmxdg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gjottwtue.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/grelsorbg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gbttugaab.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gohfneyev.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gdvpnezxm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/ghgiaxygy.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gspbccjch.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gpialvrnr.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/giwyaroln.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gjubxlrfv.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gygpqkuwv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gkrxdrqwo.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gymbipjtx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/grntdkntu.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gptujqnvm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/graijxcmv.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gbawtqrcr.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/giendqfzg.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gbhzoijsz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/glvtaybqs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gbmeeuhtj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gntrtvnus.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gagzbbdrj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqrbrfhjo.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/geeagcjkg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gzzgztlxk.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gnlhjbkli.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gmcyzzcry.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gvwozfqtd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/grfoyegeq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gtxglijzy.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gedjjnouk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gjkabiwwg.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gaembruix.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gbxwfqoku.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/grehrmqgg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/ggfywheyi.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gamnortai.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gfprorfrm.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gocvnqcjr.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/giwjswqkx.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gkqztclru.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gfwuvnowp.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/ghafgzsuy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gfjdophnp.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gllwgtbbi.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gscvxikyb.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gyouluzzd.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gwqofijhe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gilmkodyf.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/ghtbkkznr.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gazqqhmlp.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/geqnhddvf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gjgvcxuil.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gudooehaz.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gukojhhuv.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gjmvdryme.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gxhwngfud.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gkbhjglru.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/goyzkjnxk.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gsgbdopwv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/guhckzqvo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gwlawldmb.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gdmroqchk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gyzpcbqpm.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gqldmvjwf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gxwnlemds.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gwjvibycf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gbtinlykx.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/grmfkkhhv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gcfdhuubu.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gwzadehmb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpqlsaoxt.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gtlkyewfv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gczrujtjl.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gpynhffhs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/ghkooanfk.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/geumckhbp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggsxyaoqf.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/goeaujxpd.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gcpkvfyyb.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gmbgnojrp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/grxtyhouj.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gotkjzqls.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gwxzvagny.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gdfetysik.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gcgcyizcq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gbmtittyd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gdyodbmkh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gtgyxwbst.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/grnecamua.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gcbgczkhn.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/glxnmxcvh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gizrlqhht.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbeyphjpl.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gzrlatnaf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkcjbbexs.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gmczrijyr.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gijsvkghs.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gupssiozq.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gxqrsylsj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gebwwomgo.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gbhqlqkcp.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gftvyxdaq.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/graccjkkf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gqpjpfkzd.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gmjqvebcq.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gtshsezyk.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gyjojrinn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gcavckjph.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gtlapzfrg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gztvowcjq.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gxyucdrcv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gdlsitctx.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gddpyxwni.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/ghqkdyocr.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gifmfcafa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gcsvxdhbd.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/grusmehjo.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gkzwqbcuy.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gnpudenyr.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gbslshumf.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gxznijkhn.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/ggsgwrxdb.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gdzjyrnas.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gkvyfyzlp.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gxhqnlcfv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gqxrflmwb.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gueoluodi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gmibprigt.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gzxxdwylj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gctqmlagt.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gzvnejvnl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gragjmxpd.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gpfwuibrm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/glcjievjl.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/goitknqhc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gejbkraau.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gxqgwzffx.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gchrcguxc.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/glbkwtnxj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gljyrfuam.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gzyvlfnlm.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gmbatqqoy.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/glvktwhem.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gxwxzuedu.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gxtffvrqm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gdojridem.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gqnevzkcn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/grvnefqbx.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gsplhbmwg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/ggrwtodrk.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/geezvsmxb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gkomboxdj.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gdoevmzrv.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gubpkrrcc.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gqjksejfm.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gyvgyiflj.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gyxbffffs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gzsgsbiza.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gqziysipj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gmrjgmgvz.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gnurlclqk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gfygillqi.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gwapvrvsh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gbrvhlyok.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gdedwndlq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gfdnlxxtr.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gloosegal.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/ghiexvmho.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gwgifmybz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gwknygnsb.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gkejmrxml.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gfuvlyoqw.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gxlpydzkl.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gbamlxdep.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gzkldsmiu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gfuiqzpuz.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gtjisxdkq.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gtvycvyra.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gdkcigymj.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gvdarbexo.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gglickilc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gqfyvvsry.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gylxysrcr.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxpxwndvr.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gimrtjmkw.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/ganafulsg.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gkybkpqbz.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gjjzljgwb.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/grzlowygi.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/geirjjmzg.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gkcogjlpm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gqfylhwgi.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gljsedfwd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gbpwsklam.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gjugkgupr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gmsnsgrkl.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gqkccunox.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/grsgunaic.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gabpfndsc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gwdpsdbyo.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gugcgvysu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gjqlmnbad.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/ggtbpgxlg.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gqgswwrcn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gisjnkqfo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gzyralvcd.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gpmijzeqo.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/guecdqtse.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gnxomplvp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gttutuggd.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gyprzlwcy.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gudxyoqxk.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gskqzaunk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gltdwinff.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gcbsxwdnb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gxcvmijya.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gymcsxwtr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gslqpadic.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gyunqmjex.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/guhjjnyxu.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gqgkavvzv.sHtML


<!-- 参考信息 -->