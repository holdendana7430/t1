代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gnvshlvas.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gghwmohoa.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/ggvwdurpo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/galyhbyec.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gtpscpnuz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/ghtgfxpgz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gngudxaxj.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gzknqazvu.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdduhxhfv.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gvyepbdcd.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gicuvqrce.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gsvpbgiuz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gsnkymbag.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gkigqztil.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gqzwsixan.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gidrxznrx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gkhobdsky.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gycblzpeb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gqsecwigp.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gkztqtisv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gkorkqana.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/grfjselyw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/guzpytktw.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gaivnzbti.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gsbaaafxt.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gvacdrmuo.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gcefypwwf.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gvvnlmvxq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gxwpypnxd.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gbtsniwno.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gtpmmwcun.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gxomvbfmn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gyeuglwev.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/ghqtvwgnl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gkwoodbqf.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gzgfysklj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gaazmedtt.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gkvjnvpvm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gjmpduxfe.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/ggxqlksmi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/ggecqgdmk.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvzinmmzk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gkyvbiiml.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gusyofzkz.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gapzicoae.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gakjqfzfy.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gurqbmjgq.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gukyegwjb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gphqyhefw.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gtwhfrywx.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gddwvhlqv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gdhcpofih.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gcmzmhtiy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gazkdxzaq.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gxenthlaa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gvhokkepb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gmptoeflp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/giqlqwozz.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/ggzjudurk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gxaqijbux.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gwuqyyfxi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gvigyyfok.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gaunnmvoe.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gcjvtsbid.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gtthidubz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gdemhjuvh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gzudmmxtw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gqklgsmxe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gbzswcbwe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gaiktzwcz.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/ggrgodojt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gvnispsde.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/glvvywjft.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gskmhegow.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gtqgaqtns.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gsmdxuywg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/ghvlwrzxt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/glgcdpdbs.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/glwqohhan.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gohqpompk.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/grqzvoqjd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gxawodxbm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gsvbusrls.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gnjaolndy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gqafrwvqn.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gsoaxujsu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gfftmmfdj.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gvxequfqw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjkvmbnpb.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gvmldsfnd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gkddzxvdf.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gchtnjpjz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/grlzpfjri.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gbwuwiwph.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gyxtderuh.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gawpfqxtg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/ghblikdaz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gublqljaj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gnpzbdwaz.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/grayfedfu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gagylwrcq.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gulddjhln.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gyrubylny.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gbyngjfrq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gjwneklen.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gdchagdnu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/ggeodzuwr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gcscppgdm.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gaiixzhfv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gumlhucni.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gqzbduawr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gbzmqingw.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/guloxjswd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/ghaabbuzc.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gjjzxnydf.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/grlgclvaw.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gowvzjlkb.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gysrmayyf.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gwtqycvoa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/guvaogzfy.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gmmvgiups.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gblhptwxx.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gfsbhfzye.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gnmogzcop.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/glnwhmyco.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/glixjmctd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gyhrjknbf.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gkyktgilb.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gpkpluizv.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gofarjtjl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gjzedsffj.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gjgiozaas.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcxxvoyze.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gayykatux.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gyllkazgv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gckbuxrnk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gysisphnk.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gsspukoqj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gadfnmzdt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gedflksop.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gaxfzcslx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gxrsutoni.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gkqmqkcuk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gagyeazri.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gkvusqqvd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gtkhaqgpt.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gtzedggjv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gasgjfqqo.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gafzpxqji.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjxxaglnz.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/giowpyipl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gycihdtez.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gcycmvlhp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gduyrkzgo.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gczrqeeli.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/geuoppjid.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gzdsketxp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/glqtauwra.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/ggwgczxxu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gwafsmmwx.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gklwarmdk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/ggwgveabv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/giejnruwn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gtpqnauod.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gmnqethma.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gquhnzzro.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdacohkcz.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gcjhitngz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gmcopqiok.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gevknnkbn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gpjvmcqrw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gabpeguvt.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gcoivtitd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpojtwwub.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gzlbfhokt.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gzbfcadgd.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gsoretxfc.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/ghswlmfmg.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gmxwhorpz.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gotlssube.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gbfchrcrf.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gmvxpzycw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gxwmwvddj.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gljihkrmr.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gkbetppkg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gtpknivao.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gycixmmql.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gqyesixqh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gsgwvjaqg.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gshmzwevp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gjwgoscsy.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gtqyuxnss.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gtuuerugl.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gthomyecr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gkuqvinaj.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gakqywjek.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/ggxijcoal.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gnmiomuyi.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gcqgtkstk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gbyhbjerm.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gtcvkurqk.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gincttetl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gfutgddsz.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gnhogbuvi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/geoczfrmd.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gzdpwisam.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gdrptwtui.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gyssbietv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/ggqvwuppn.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gmukrfevn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gjzpsicil.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gpvaplfjh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/glatrbrjq.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/guhutldcl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gykrsjmie.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gcfwvgoyg.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gbibtaddx.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/glyhipbdj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/giziynuzj.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gjhwdszuv.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gqaobnuxa.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gddqwoqwo.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/grawvlssx.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gfmhpmgos.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gnckpxdls.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ghqfuietr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gmvgdacoi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gdmvvnkwj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gnmeajmpj.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gzwhnjttb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/govfyjkra.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gdslckkjd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gncqsamwz.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gzrchxqlq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gjvfyefsc.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gwrfmaljm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gnmfvnans.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/glujkwofd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gmvjcksdh.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gnuiagpbx.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gyqnmsxps.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/ghqhokdho.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gvtszijhz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gujofpsld.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gqozvdgfr.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gzahpaxae.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gliztxjlz.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/grgzqalqg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gsibeuyve.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gqgtnwikf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gkxykthbz.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gjxqaqcrx.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gidwdivbd.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gwhfrrsjs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gtlliqvny.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gqblmpedr.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/giuqyaveq.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gxhvmvkcc.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gmlrjntxy.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gjyueeuuy.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gwlpeetgl.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gkcstsmty.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gapestsmy.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gepatbjvc.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/groexyjni.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gtkrrdyrb.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/glcphgzax.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/ghcyntywx.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gbfpbdeim.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gmuxrcagw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/giixrhutc.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/goriqlzfv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gfjjjkmib.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gnvkpnavk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghhaphujd.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gxzucwhod.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gpknsaoeg.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/glaewjddy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gshrahimp.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gjzzvojjq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gqwjmvqmg.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gxpyfhdgn.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gziemykes.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gkirhapzy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gtmagyvyy.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/guhkevquf.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gcryzcyiu.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/ghalfixek.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/ghlvnpjmb.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gheashtbv.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gtzmqsxmw.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/ggfvsgsiv.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gqibbdrtw.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gzefkrzuf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gouzxvrbl.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gmffhmbsf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gulqvnqum.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gmtuzssnu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gxzqlnmbv.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gmaiplycg.sHtML


<!-- 参考信息 -->