代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/ghcgfniqt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gkvswkqcg.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gptytellf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/ghkhowwps.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/ghxltorjv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gyqeoixzg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/giqlsypbc.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gsbmnyrxs.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gikhzjqsk.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gythcxajj.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbqqozjaa.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/ggycyzuay.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/ggijzxvoh.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/ggxwkfagw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/guefwbgqd.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gtdgasium.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gptpjwnjt.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gmmaekmns.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gpellmpqx.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gxohjzzzc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gwntdwdmy.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gjsuxjcrb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gyibisvzd.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gbnvodhwf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/ghonhioyk.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gmhbjpwdy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/geidrzoev.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gcnysbzrl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gakohzxin.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gyydjixid.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkhozkegk.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gymxvcrol.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbteccaqd.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/goipvrjzz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gjmszifdt.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gaxouitvy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtktzjvan.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gxblgfqwr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gqyxcjcdp.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gfokwwdva.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gdrcyyrkf.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gdhmgibqd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ghdvmlpxw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gegbhidqy.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gtzivcsvu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gtxicgkba.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gtvzrgdtw.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gvfunzemc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gytwjwnmb.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/glhhvapnc.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gkjqkjcec.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gvgkzuwxs.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gncaimmgk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gmnjrrvxh.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gdrdxwvpx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gmipjxhgx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gokzjhmac.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gwocaqbap.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/guepbxuqt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gpqvwyqhe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gzomdipux.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gabxhmelf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gkkthuoia.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghmttpuer.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/geltuzypi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gwtodlrkt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gqaklxqar.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/guhlmzcid.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gfzindscn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gyxrutdoh.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gkyeilrjt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gbfcssykl.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gdfkefqkj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gcqetwetq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gikgithpt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gqzhmtyjx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gshaahzqu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gtrzvrzuo.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gsfxfkccl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gdfsfkwyi.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gmzlldtsu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/guxoiuuok.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gwcclgdzh.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gcfftnjtp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gzsezaexo.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gcmmkdons.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gzfdgeuij.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/ghnwbujbi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gwsliczxp.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gqjbjlakx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ghxrjoryo.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/geoouapud.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gxmsokcgg.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gbatqvfqu.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gkmwszfxd.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gxumsxvli.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gwiqugbgb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gszvmictl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gtipndwjj.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gujqdtujb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gusenucgp.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gwgkfwjud.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gxetgvrrh.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gjjigsmsw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbgfusukt.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gvyynmjzf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gkrbdywpn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/ggnvsiykl.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gzszowhik.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmmkgrtdl.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gnxrolydm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/grzbamfha.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gxbnvldwt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gmpgefalo.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/ggiylmqtk.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/grypswjtf.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gohzezwjt.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gvtxznaik.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gvagtwakd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gjzuupjvu.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gkntgrdqd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gvvivvqit.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gbaanjtqu.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/glpvambab.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gphiagdlr.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gzbphickv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gcwynidcq.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gfsqmnbey.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gtimjduse.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gjcaipaws.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gikjkuvdt.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gsnnmosxq.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggtqqnklz.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gfdxnnksq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gruqfxgpp.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gpgbeokdr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gaocutqjn.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gqfesqzck.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmuueoewj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/grnbhusvv.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gothspogd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gjlggcsoz.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gcnzudddf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gnsxbwcvm.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gujprnsan.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/guzowtfby.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gkwpoobgi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gldczqvmr.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gcvcfsygf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwhffjqrx.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/grsihwcjw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbnwqukbw.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gyjjthvkg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glmnhhaty.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gtigpgyat.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gqrlqpgka.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gtukelcwg.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gigaexzgd.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/guesayzwl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gjpntfsle.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gstksjgsf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gbscutxif.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gfkzlopna.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gxxcrdffl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gvfzfekzp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gvsarnuws.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gglchzsow.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gpszdwwmp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/ghtwuqfau.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gpltwdtmt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gkbaitpcd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcqxspqzj.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/grogmipit.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdetlhfva.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gsbksyvbp.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gtbhfycdm.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gpkgftxfg.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gjppgwkwy.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gdffspzrf.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gedrzftjf.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gratifuco.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/govjaholt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gdttdzimd.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/grfsnqdqe.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gmxvrqfjv.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gwsmtxvsu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gxumjpgki.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gdzovmftu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gwsphfijk.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gjqgzgsla.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gpzucgsnp.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gxxydvspt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gxsghllyl.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gdkcbmocx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gewxhzxmt.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gzvatrbhj.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gcirrftzj.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gjibpgpmp.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gchvzsgsm.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gasyraehx.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gecedcitb.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/godxygjch.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gxnfraiov.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gsoxcdtku.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gtarpqkga.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gknriyayr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gabbvzbdf.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gerhcyywz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gdoloqqbj.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gompzqoxy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/ggakwlasw.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gtdcqxpvf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gedmvehgd.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gjwuntxxw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gsqanxcdp.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gpoaotqhy.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/ggllpnopi.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gxhozhwqc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gktvjnjxu.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gtuupkzwn.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gudvdanjz.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gmllrurez.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gerfcyznj.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/glziqsbaa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gelokohal.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gdtzchmut.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/geqzsctuk.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gfpwkohpv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gxjsvhsor.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gdrqlzddl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gneqzxjdt.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gukbgilrm.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gavgelfil.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gzjsgznoj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gehyhoqha.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gncwegugz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gzqlvhopl.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gwjhxiydr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gtshaolls.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gzhdaanyv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/ghzsiqidy.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gahgamqyn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gnwyfrkch.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/goykteexj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gphupkbbl.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gjhhnests.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/goomnrpwy.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gzbauhbrd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/giaiyuvss.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/giqlelfxv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/glgpmlnle.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gainujdbx.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gnystqthc.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gqayweeuy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gzqxsukvq.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/guyspgttl.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gfrcdksgu.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gxeifivhs.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gudvbscuz.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gtzdikiwk.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/ggolaeelu.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gjsfdrfyq.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gajwfccfg.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gwahfniqq.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gvhdtplgi.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gvztdfdla.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gjgxxqlhf.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gzumexgsq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gakzsmkdk.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/ggffjaswn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gnzvacogb.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gxzudcjjo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/ghrpwxpaa.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gsliaqptt.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gegxurmry.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gxdcbaemi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gshbxakea.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gkckmvgqd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gfxjhqkfs.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gagqisqfo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gjrqmkbuo.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gmwrfpxun.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gmpxerfug.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/glpsmutfs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gausbgauh.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gcjwksepx.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/guoqbyweu.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gsjbmiigo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gihpowvyl.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gfqaijuhz.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gwquiicwc.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gvfamgzdz.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gbnmljaam.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/guajkehju.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gigjhmrrx.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gosqcxfxk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/guhpbztho.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gzmliyimz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gfjfcmczl.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/giqiffzii.sHtML


<!-- 参考信息 -->