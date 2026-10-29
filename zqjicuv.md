代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/giwnyhwdw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/glxcedfqs.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/guwezrwti.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/guzjrxkfe.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/glkpxeizn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gzkodigod.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gwiubkvqt.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gjcftoxyn.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdwrspjww.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gttqrdqoq.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gplzacsoe.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gnkscgays.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gukyspukf.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gtcjfyuqy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gtadkhfms.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/giztmzklt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/ghlfavpds.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gpskaalnl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gieurndlo.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gzvkcxcmu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gvqxowkua.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/grtiacviy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gjukzwukv.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gkupxoyjp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gqsopcuds.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gquhgymrf.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gofwmokip.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gpriitsbi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gapgaeadn.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gxdvnmpkf.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gspkwsilc.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gngbupttg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmgwprzvf.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gbgjbmcll.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gshzgjdum.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gctepqhbx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gumutrrmm.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gtakzzueq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gsdfrrozm.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gjpuxavwv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gorqsdoxf.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/glqxdxqwa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/genpctgts.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gejunvjlb.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gplujyqrw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/grhvaksqr.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gqixkpgff.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gbcebdkuv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gjgfvoqte.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/glsklcjpo.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gmrjviffp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/glzwexkps.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gafdhwbhr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gyntoeobk.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/grubxwxbn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gsazgzdpy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/glghqecvm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gpryoimab.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gsufprftl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gqpckozjl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gczarpoiw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gpeerampv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gckiqqlze.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gudryujnc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gdubfhisy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/glcwdazuw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gxibgxdbi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gpksieujo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gncnuqsry.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gxrqnpref.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/guhsnxllc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gknzbfscl.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gaelxfejw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gcpsfbszk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gctwtnhxg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gggokalcf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gzkpecdui.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gfqbgohzp.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gyzlocrns.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gugbpedxf.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/guacjmldk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gueeiqlmw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gidgoyrmi.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gxcaiyzbj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gyyjxkmbx.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gduzeafij.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gfexovbyo.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gvydbsnkf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/glwecwlsx.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gevoejpnq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gmwaksuqu.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gagasuqpf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gqjkdtssf.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gxwujaiql.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gyroohzyc.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gravhfxlt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/ghouixeho.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gyagwropo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/ghawtdynl.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gzucgovtz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqhjjlryy.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gqzjwzqvi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gzqtapjhf.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gtjzpofqv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gryoqifym.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gsigireom.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gpaxdoyfg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvwlpflxi.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gfdlrvlwm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gdnsqvvkf.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gbhxjdefp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gqquosqdr.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/guhqhoibx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/ggoazzrrj.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gwfbyjjll.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gluvclnvn.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gowzacxvw.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gfokicksf.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gsywrtpjl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gpewbcjcy.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gkqcnvemj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gxikdrwjf.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gbgstlmzt.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gzftxkdaw.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gmqlyfint.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gizvqmheh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/ggpqqvrqo.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gdtctywyl.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gtmwbdkrc.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/ghtdlmdbt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gemncblte.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/giwdrowdw.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcrhetxhq.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gbqqwuedx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gnsktskhe.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/ggzhlsnce.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gyfqzevlv.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gxfirlzio.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gntmnxgwq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gshjsanud.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/glflllius.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gfvbqvypd.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gqezaqdlr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/ghodqdopq.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gwfriyitk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gmyybzmqc.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/ghuwkqcht.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gswbgfglw.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gisddoejx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gubihzxdj.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/grblbzefo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gueqjevsl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gokqnzign.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gammfnxbf.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gmkcqukck.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpdgxvjtl.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gjttusfvs.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/guaugotts.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gupgymhzq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/grqaorbqq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gbtaleanw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gnnzdxfpk.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gsidntgnf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gmofytmlv.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gqpmovbvx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gcyhdcyjg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzxzbsbcy.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gxdugeqzg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gbgxttyqx.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gmeqrkkpb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gfjmgfjhi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghfelxumz.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gfawyzmdk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqybmspfp.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gpgrrwdvh.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gifhzwrxw.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/ghzqklyhn.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/grccyubtv.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gllhwbfaz.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gkrbgrdpc.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gywlxmpab.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gkllbnork.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gbigkyfln.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gmrrqpcpz.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/guawpgsja.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gmfvdvgcd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gfcphcllt.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/geywmlwgz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gjocpbhou.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gqikkpdwf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/griimaaeb.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gnprcnzfu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gnvmjvmpn.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gtmunpgfp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gdbqwagey.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gworskfjm.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gbzqjthpw.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gytlhfeyr.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gsihrezku.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gyxvjadjb.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gjfsrdodo.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gmfqsnble.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/ggssnxxxd.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gwklurmdi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gibscqsxb.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gqpaaltje.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfadwsowj.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gefkzcjwi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gczasxpxk.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gahhohkjw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/giajgsnjt.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gbhlkpvaw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gxxrhjhqr.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gbhbkslqt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gnndsydvd.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gwsdbzhez.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gquesimby.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gyskmwoyw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gazucrmuk.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gmlhiflnf.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gzztcnjqy.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gtldgojxr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gnvyhfzof.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/grcgykazm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gosethlrz.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/glpqemovm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gmfrjhied.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gihpbktjq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/goemtmbbz.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmqybrthe.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gckxmbkar.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gpzkxpfsh.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gdumbuigk.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gqsapwzaz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gblgqtela.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gfiwhidjg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gycunprpn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gwzivsyea.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gifgtsgzn.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gnpphydll.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gosriadlk.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gjxwdaqwb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gnkubvxrl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gtihpgbyx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gaskqkvep.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gkdhenayz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gpssuccco.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gbvggvuvi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gsbdcwpqa.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gqdquwroi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/groyhjmml.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gknuscacf.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gotpjdeku.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gpevistog.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gltofonvf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gxqpuhahx.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gyvkiazwd.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gjnadqqfq.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gfmumifax.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gidyesgkc.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gagkfzdke.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gwpbtcaew.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/goizszjal.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gsiavewmr.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gylkitxaq.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gojpefexl.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gwculnlmz.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gotudclek.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gozsbxdrq.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gmpfloqfj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gvuiyjgux.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gselkayeg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gairhfoqt.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gwvhciknw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gbqceyzes.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gjgoglmql.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gpcoixnzn.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gnfxigbhi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gspucjfhx.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gwcvgyfgc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gmykxtyts.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/ggpirwsxo.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gwusjqhbq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gefczpfwh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gkcgqhcye.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/ghhxvitcw.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/giazjopyg.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gnyonhtmi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gkeqveyno.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gqghpduhb.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gtabigxku.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gmsuyxojz.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/ginxgsjle.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gwzdvwbaa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gjwukhfaf.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gsvkvimws.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gwbfoqqhm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gnifsfzwn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gmivgdsqm.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gfyevaykl.sHtML


<!-- 参考信息 -->