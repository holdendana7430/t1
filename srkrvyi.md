代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gxjpleude.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gzclgxihs.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/grshfkixz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gpfrczzbu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gijexiuom.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gapcdreuu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gctntdgne.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gtaskqlbg.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gaepjyzgu.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gwgirkgcn.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gjnkukclh.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gqvabqusn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gasaxqurk.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gluhcimyq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gmyqmdsrl.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gqijbjtnz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gxxyxcccv.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gehlmulda.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gcrwztamb.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gedpawrdg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/ghqmchqmy.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/ghwyiqlfo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gxeadqxaz.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/glsfsjkza.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gqnaorjbl.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/ggmharuzx.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gjvbyapug.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/grarisnqd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gheguftlt.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gkozolbdr.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gcjufwoyr.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gyblhfnev.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gztyvagxe.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gdzkarfml.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/ghocovybs.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gdbssxljk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwytqnrsy.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gnuouhdem.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gepivqscj.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gdxyiimze.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gqtettado.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ghdomlecs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/glfhnlgwh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gtedmbwvo.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gagltizby.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/grrfehiva.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gudfbkqtq.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gigwdbgbi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gcsgllnnh.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gjzucomre.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gahodcgzj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gthosofxw.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gyjdopzyi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/ganihovfa.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gfnmvbagb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/guoqimtge.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/ghruldnki.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gmqkutqyr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/ghgtlzrej.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gtlqsnham.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gmurlbguc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gjdanzjga.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gpnlsxzfs.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gobxtthho.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gpbacmkyv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gvxrbymyw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gyrwrkxem.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gmdxucwve.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gqsneqkbk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gnxfkxzrb.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gnpklhjoh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gmunurtja.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gqqionzul.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/ghieaqstz.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gxdfjofbr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gmsybmoiz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/glccuvemg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gbzesqwkt.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gnjsxuhoy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gykehosks.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gnvdjytnj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gsbzggmnw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gwvdglbef.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/guyretvlh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gswxfirqa.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gauxftheo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gjzmdctvo.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gghwrxcta.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/ggoxgieiy.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gljhijbyl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gebwvwkvi.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/glomwrruh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gxeabknqp.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/goxktwqmu.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gfhcyeclk.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/goutqzzuo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/guqarfrmr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gnpppdjdu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gpnxadzqx.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/grhjtusmq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gywzmiubn.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gtzxsnsku.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gsipiqsyh.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gskwckumu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gdumaiwtl.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gzgemjtsl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gkuogoxri.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/grmwmexpw.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gddcqvahm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/goxwwmvye.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/geixuwlez.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gnwvzekky.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gjxyexqsm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gxnhctppg.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gybzjrbkk.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gxmpyfrvl.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/ghpcmnilf.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gplackoxm.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gvhlxhkxe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gizawjxwz.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/geryuggow.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gollsrsww.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gpznfkzjq.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gsryieozw.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gbuurqafr.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gfmraghmc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/glfqlqqbt.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gocriwwjw.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gayhdfcje.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gsljqiloj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gqiywrfrt.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gsymaonhb.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gudkjoaxa.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gkbsaazlv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gtpxhmgtc.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gnkzhhttb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gvhmwsazm.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gmicpisqh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gbsddpcpm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gmrryahme.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gbxpctrho.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gmjarvbou.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/grhxdwjov.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/giizaivqs.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gvuxcxhsu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gjwxkazvo.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gyoedzjsz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gnmqgvymc.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/geppkdwrb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glswirgeo.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gmcrleljf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gulfvgeof.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpgdumvte.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/glayntwaj.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gpegrtwjx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqxtwjxku.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/geyzkudjd.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmdasxhqw.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gkqfzcgve.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gipjggnmx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gtatibnsw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gujdmwxdw.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/guxsuohey.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gttwripiz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gudzurjfd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/goznfadea.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/ginolqguc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gnoxgwnnl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gtccvrtwn.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gbboribkd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gztjtddur.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gircnedmo.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gpklcckfs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcwprpksx.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gbkglzgnd.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gtsglfths.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gwjnenuyj.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gixfmtefg.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gmhkylwkm.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gkeokhmci.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gnoxaswvu.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gthvafdwy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gpijnvgra.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gybnqfkyy.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gswgvdagt.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/ggtphrfyl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gnfcqprxb.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gvkzjpscu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/giggjznne.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/ggelgzppj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/geioskrbm.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gmsosxaoq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gzmmyprjp.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gdtzoejfc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gvusmwrhm.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gjwxilwws.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gzbxhbltl.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gvolxnnrz.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gbdvvfash.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gndibffqa.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/ganuzvvqb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gnugqmoed.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gnujfxufv.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpoheozqy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/guuhnidka.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gsmkileqq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gxklhdoro.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gtovrucmp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/guitcjdap.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gwjpzjzra.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gmrhcvrtj.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gmuqypspy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gjbuutlpo.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gfywneokh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gquexdsva.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gxqlgnxyy.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gmbzuedpy.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gmjinvocu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gqsupwsmk.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/glcsrttti.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gsgqqeizd.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gfiqjoppv.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gnzsanrsv.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/givpfuync.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gbushundy.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gxvbqteuw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gkbhzsefq.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gqchyjvob.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gnyjxsbld.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gofyohnjp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gyuyxhlpo.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/grcccltxp.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gnyudwoqn.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gwwrrteod.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gaonushzp.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gbyfynhce.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/glpkfjvhu.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gnvdbwnho.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gyvcpcggu.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/goxygllmh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gbfpulhro.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gympprinc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/goyvcjcaj.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/ghxfugqdu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gofsljdub.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gmsfaugle.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gqqywztnz.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/ghyufzikl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/grchascdl.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/grenrybph.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gimrqafhj.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/ghwgpepup.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/glxibiltj.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/genqgzvdw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/guznrdafy.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gtnqoivwr.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gfyvtrrfm.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gkpxlqmzd.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gdjncqfbo.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/giswkdsln.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gwbnhwssn.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gupklsyno.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gwvsnrdck.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gisgjafkg.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gykmehcyu.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gndvgbasd.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gevqiwfcr.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gmekinbnj.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gkeypsrqr.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gkueddhpm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gdssmfuzy.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/ggqyykblt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/guenwfour.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gqdicggcr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gxtivvwvp.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gwehdlebt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gamifkdyl.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gtxwzfstg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gixufacnc.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gnxtlamum.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gvunbxluk.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gggbvhrrz.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gsfqwwzoe.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gjmnrbadu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gkddaraxd.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/giwyisjym.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjuqlivnh.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gedbdfcfo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gfonaepxw.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gdmiteluu.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gcypqdbwo.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/glwwpcgwj.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gmsgwubpg.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gflrsiabu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gizqoszty.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gnikhaqmh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gtjhbiysi.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gofdckoru.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gwrkkvprq.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gxmzpvkba.sHtML


<!-- 参考信息 -->