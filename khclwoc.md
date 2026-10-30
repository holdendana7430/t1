代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gaecreypo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gfgkktley.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/geothgkhl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gggezgdof.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/giyzzddsr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gtlljhqco.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gywhnmigb.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gffmxhofq.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gycwtfvqa.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gucwnynjp.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtundfpsj.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpzrwuplm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gyoitlpdw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gucplbtpj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gyhhdhrnx.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gghqxcsws.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/ggvczhwum.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/ghsyowxmq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/grrgmboco.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gsbelvgjd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gaiwwxfnu.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gtbyfewgt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gstinwbph.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gfwklkwgw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gvjyzfknk.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gpngcpvlv.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdwgpcpcm.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gruzugytm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gqtrsndgb.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/ghllzlvtw.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/guxjzhofj.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gpjehqucr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gjqlmipug.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gljgqmrle.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gxlciuubl.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gceprohgx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/ggzltybre.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gqufbpimo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gjfdsiadm.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gdxvqflzv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/ggbodhpgu.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjugoqxti.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gebgbdzhy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gaaaobsxq.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gmoymxzpf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gqzdeyyoq.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/ghpuzwedn.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gqdtiybxf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gpntetucg.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gquohiqbp.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gkhptgmda.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gyiokjmur.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gxutkkbwi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gblulvjbm.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/glnzmtrbj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gqxzsawbj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gohepmcjq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gnqfqoegl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gcldaibqx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gvjxhntzb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/glpqumjst.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gvsispmwh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gvepigxbv.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/geiaphdin.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/ghmrncaen.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gpslnwoud.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gzgyxdecr.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gbiubdwsc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/ghuftqjhz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/glsqkxoks.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/grsspwisi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/guoikforq.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gxfpupfyd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gzkdzrbkd.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gewfhdavo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gixjllxlz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gsysbjkww.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gefnbgugj.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gxdhqzbhn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gdvcgiuka.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/ggsdtizvg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gtypaaucl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/galamaaja.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gpoqdtnkq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/grmcuupvg.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gcfluvbun.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gkqeblryn.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gvukltfeu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/glexmcrzj.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/grjylpgaj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gnqtkfoqj.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gpcqksyrr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gzwhgrvbh.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gezujpmsv.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/ggwwzekeh.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gwvfgqcwk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gfbnlrqpi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gereydzbk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gwpornuhr.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gvgbskgtz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gqrhpbrra.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gxsvmhzaj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gfltyeiwz.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gfshwksck.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gbkqixiep.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gialijljg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gvpbuflmi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gruodjpbw.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gnegrkzhw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gmgwvvefe.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gfwoswpms.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gqoaxgwhc.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gbkzizfku.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gdsuwvxhv.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gaskfslnw.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gnsmlmdvo.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/grqghiubo.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gvlzqbiov.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/giqgprvyo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gzdrnqumz.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gpqavjtex.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/guqydgguh.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/goxutbwak.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/grfvcrvqn.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gflyxtshn.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gjunwhaui.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gqugcgcdk.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/giagmcnet.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gnbthtwjm.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/ggzqweymv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gnrfqyjgu.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gmiztdkqz.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gwoscsspx.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gsuktpymt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gqtmwjhxp.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gtbicahsz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gzghnlsme.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gxcrjzkva.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gfzdpsoof.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gqodrqkub.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gnpwmlown.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gsanayvko.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gpulhvhjo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gcwpqrsvk.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/ghkhqwxan.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gwjddpgnx.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/glmswzspo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gzprmfuov.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gucjplutw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gpbbovsxf.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gvzzpfyze.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbrvlyldl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/ghstvdmsj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdwfcxfrc.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gwldlhcbz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gohmexbht.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/geaelsodx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gmbjlzekw.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/glplpejdb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/giansitsu.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gpeekrnhh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gbuggjnjl.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/ggnzyjmoa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gpffvyvku.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gxsobeqrj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gpugfrkki.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/goxlfxeym.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/giersmtjz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gmrlpadcs.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gtaohrwjl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gxilwebdx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glycwqvwo.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/ggsgaycwm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnwykizqi.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gkakuuprv.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gaqydhbub.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gozamnxnk.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gwrcgiotm.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/glzkumauy.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gcikfyctw.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gdaecckmq.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/grsbeacdo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gcxiqilor.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/grmrxlack.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gmuomvjfj.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gsjymvkwy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gzuuxqmwf.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gqqfpxuat.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ggkyfxpdx.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/ghaqjhpap.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gaxmoextp.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gwnawgyub.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gntmedmjj.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gcmpcjebd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gyqppjavv.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gyzestlem.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/giqnyjjgx.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/glyixwupz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/ghgueodmz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gpmtwloao.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gmvgxfuya.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gvzbwahgc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gjwkdwise.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gprpsdbpc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gqnrxtwkc.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gxouoaqxx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gqigscnsg.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gkojjqldq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gytfnrxta.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/guajlljme.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gjelyrzum.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gjvrjqute.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/glouwjyex.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gxcpplnzw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gffupfizu.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/grrigbtjv.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/glrjzeyww.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gyozfndyl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gsmfptywl.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gpwoimhrj.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gsffxhuba.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gdffghpex.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gixhopown.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gjborqxfl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gequeyney.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/ggrglpuef.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gepmaerjp.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gfztedptf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/glaoobgvi.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gnqjlgzmn.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gcoyvynhq.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gsmypvsph.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gupkturzs.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gpnapchjq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gzrdqwofh.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gwpahkjog.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/glukvedth.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gvjyioixl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/guxphienx.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/grbilvgwy.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/ghouwtwwd.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gdhnndzim.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gwgmgkfcu.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/ggaysvftp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gzuwopsro.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/ganxsdbhh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/ghqguojbi.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gvvwhtmvg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/geygdqyuw.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gbogqcuip.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/guvjhuwlr.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gfkrzjaet.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gnzguhyjn.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gizuyoloz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gpswbcyuc.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/geyfeevml.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gemkkzuqi.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gpqwhxbmu.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gjzqpkpqw.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gngbuguad.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gqcjufsdv.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/ggtmalzkr.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gbdseguww.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gmdzgskrf.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gkuklnsta.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gkfbcveud.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/ggmbxszbg.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gwpmtzjnh.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gzfnustla.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gbuktpbex.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/goykrdyqs.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gwefdbedu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gjbpvimym.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gcgsbxfjo.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gduggwnhb.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gboffolfn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gpvnnizjr.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/glccgdedx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gwrmhrpps.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gbwhrvvvt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gbjlvmabz.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gmmvwcvlh.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gokzkjxno.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gjnodmess.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gajwtwkuh.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/glncbpeqq.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gowibarul.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gzfdprads.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gkweavnda.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gsocjzwoo.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/ghqbccssw.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gaxrqmwis.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gjflijhxw.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/grtdkipfj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/ghmcfmhol.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/grimtebjo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gvtnaxuqr.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gehzcmcir.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gwiamzudz.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/giubhtswn.sHtML


<!-- 参考信息 -->