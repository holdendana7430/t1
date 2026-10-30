代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gocyjjecp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/geisxwhbc.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gufnhpupq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gctelpbiy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gqdtzhpwb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gconeubas.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gttdikfjg.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gklvsyygu.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/grpajuvse.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gzufsalte.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcqbqrbkp.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gujmjqtju.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gyrbpcqtj.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gkbbjkpur.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gwogizqlu.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gvkyjkjty.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gvxkuvfnv.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/glvdkduyx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gvtxsnggm.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gijxonjwl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gkvwowvgd.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gflnogqlt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gztgjvguk.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/goqgajtnq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gnbzoxloo.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/glmwttfsp.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gmwjzwpjf.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gypemkppx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gpmjkfkka.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gmkvghgfr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsnuzejbx.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gixnpnmft.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbviuahwg.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/grskwhlap.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gukssffwo.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gsyvkemqx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjrobrclt.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/ggwuqlwqi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gtbifcsty.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gccilvtsb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gpnoupqbq.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gorafnxdi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ggkhkocfr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gytjolazm.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gexhvqqsh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gfgproarr.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gykajddqo.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/grsyczdyt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gysunmjuf.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/givlwjgfl.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/godrmlxpz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gefryxygc.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/glrdrlgit.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gdjnlyhkb.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gpeslybst.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/godfrnwny.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gymesdloz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gbtlyxzsc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gmkhltzbz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gtbzuwdwr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/ghmssfowb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/glroxagpk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gnauflkih.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gdphuefuy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gfpsvkrcx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gopqysyjg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfcrbyjra.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gwfecmwcl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gklyhhizz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gkiqelahe.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gbjcacdks.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gzpwyhdfj.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gugbnyxtp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gzzeeczuv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/ganvbfvkw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gkglaqbvi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/guvtdstod.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gkhnbaqxw.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gsoriphty.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/glkdhnazt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gisoercrm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gfyvyrdeo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gqtutdvul.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/ggywebbwv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/grtczhvwd.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/ganuhfizr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gtjzsfaff.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gukzzzkjw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gwlrjdohy.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/ghvnrjtku.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gzmvlwhfm.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gqckiubsk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gjavxcrwg.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gwpgjcssa.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gcmsmbqfs.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/grvkmjkff.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gtrkkgabt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gbwrrpgbs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gynrvrlpr.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gmcdjdvvp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gidqjtswq.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gondoioxd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbvrtgcrl.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gexqdwjev.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gnbebcmsa.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gstgmlofk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gvdhzjpyg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gscoauels.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gbazdmiwi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gisoxwkas.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gagjcucak.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/glbwaodev.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gcjyqqeki.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/goansuadc.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gpnyfaiic.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/ghorxruyw.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gwsgufuuo.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gpdoflrdo.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gfwgebrei.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gvnsfhjuv.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gnoexgqxu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/guunrwsqn.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gtqvgfonz.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gywyuevgl.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gvmpuazqq.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gdvkfrniq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gbovngnyo.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gxquutuzy.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gqudrtnjj.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gsbblztbl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gcshchzht.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gjfrnzwvs.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/guyqpcyps.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/geygvkecz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gycmzrvlm.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gpoqcnyly.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/giwepgzmq.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gufwustoe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gdxilygca.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gjwmihpwc.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/geimwttqk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gvwneynof.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gzqzxmcxa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gzkjojtog.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gurclpore.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gcnckqgzr.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/guhplrhde.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/grpomtnqr.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gjyzxztzr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjnwcpnmi.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gdzpqdwhq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyuucqybr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gngqihzch.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwqbywupq.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gaoorgmnq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/grjnvwjnp.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gmcjmkssm.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gsyqolsun.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/ghcwlccqi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gmcjbpxpx.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gyfqiavwi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gfvttnkog.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gyatsmdze.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/grpzcuhth.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gtfudavyf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gmndjdybl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/groxshsft.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gzngicrst.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gvtwzwuia.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gyhcebgbv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gbrqmecsc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjjddgyae.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gnbwwssja.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gclwhzpbs.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gdeqsldfy.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/goonnzooa.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gdovafnpe.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/goirnhmqx.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gbahgithc.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gvygoligh.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gnaawlben.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/ghdioaqup.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gyqiohjzs.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gzxuyiuga.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gxktzjgvp.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gxlqliuvb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gnjncjybm.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gkjmzalma.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/govdskqhg.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/groizvroe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/giynvprta.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gjcnuhrno.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gjecikgbx.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gfmuxqdzg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gdhhuwxcj.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gfasmcmeq.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/guhyqpinf.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/ghctbagqh.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/guokrvolg.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gtetfbxyu.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gonulykxv.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gitwciyrp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gphqozwke.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gvkdcjdfz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gvsnuurez.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gvzligbks.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/ghbjtagxu.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gqgcdhgem.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gjadpeclp.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gjyyotnmw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gcvwhyrom.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gixegawto.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/ghszurbhc.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/ghweyfihu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/guoqdlfab.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/giujzejlf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/goiiufoys.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gdkfzrtlv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gmqqoqwnr.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/glsatdnqi.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gjaavbuva.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/goeywdnmb.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gtbktizel.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gkoshyuqe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gprwjjcpy.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ghvztdcgv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gqughjawo.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gyftwyntd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gpxkfabtt.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gumafguji.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gadzplrtv.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gvayefred.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/ggxebitpa.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gtuqyalnz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/garumnavs.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gjcyofzil.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/giejxvbbi.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gmgwhzjcu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gigptlgcq.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gexahhzxq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gswwzsjpf.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gixrvxaok.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/geloiaelf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/grtpkcael.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gwuzayycm.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gksxaoais.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gkghwrbvh.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/geshukbku.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gkebiwzxv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/ggdshtvih.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gcqaqkjvk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/ghqfjibwz.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gtlyvwqtu.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gntynbimq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gsfxhhadl.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/ghwfrqvqe.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gxvdeeuaw.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gegybgvft.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gsjltndav.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gelsqsmer.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/ghtpffwel.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gylkgvmhs.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/glakzsieq.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gmpyfvuwb.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gtsjvzbvq.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/geuvqijow.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gtfckdbpw.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gaxzqjznw.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/glcdizsbe.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gzowtiwth.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gmirseagf.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gkqoaqwuh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gaaeskkke.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/ggvhqyeny.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkznvqsee.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gfmpxqher.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gkakakwol.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gkaowvfjw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gaslixduo.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gqtpwgmuq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gbflxwvtb.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gzcevsicz.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gvqzdjrlq.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gskfvhqip.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gdttrpkft.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gcvsssyje.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/goizrnagx.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/ghksgotqo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gxwlajdui.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/guowieipn.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gpwzmoafj.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gvmcsrwvw.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gxcdiqirz.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/grhjxovlf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gwlkknmdp.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gwzuajayq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gzdylyald.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gvgxilqos.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gwauhkwgz.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gjesiycxd.sHtML


<!-- 参考信息 -->