代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/gwcgglwdx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehsdnyyh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpyvkunx.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlzbutvn.sHtML

SELECT * FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gthkoyauq.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmpaouul.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzvqgusz.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvwqcmcv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gajdovcbu.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/guagwryql.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gbqtfvjap.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gfiixkwnd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvtwfvdk.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdrmgtqy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezerklzt.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gvditteaq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemixtaxo.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/grqbhkzzw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyobujmzm.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gyedehyvk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfyotqam.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtndzfcq.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvdxnkaaz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsttrxef.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/goeulqvqz.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/ggotwcfkn.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqucorgjs.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/guhakhdwk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guundhyho.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gygoekwrd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/glaqthnxw.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuqzlexi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glrsnzrtt.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymngwnax.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/glzjdawxc.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gtpthtjyk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gngwiuywc.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gksqbcnfu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqmqdpcp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gimdeehjd.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gtzzvsphu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwibyired.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/geelsrjqz.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gddbgfmet.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gqznyhdjq.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzdhlpyr.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gjagtkgsj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnxzspyo.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbyuxgxd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gpfbnniwq.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gmbepavvo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzayiqdyq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwkaltue.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuhifshf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/guldetvqg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmvxhwvg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gxlewyyur.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/ghqehrsrj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtagzkehu.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gjozcarkb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gakukyqsj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gitxwudfz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gtszxetlv.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gmzktmegg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gvofjbzaa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmfwvlro.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnkskwqc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gftdtsdbx.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvpzkqmj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gnpviraoi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ghclynnon.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gsffdvgtd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcuxniev.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gjssxabyz.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfwbqrvn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjaxyfal.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkwnxkdh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxhxhekl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/ghbvksmwk.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauooezeq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcukezzyf.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/grmhvyups.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/ggdwvpkdh.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gmqczclxq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaablrcf.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/getlwukef.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gjflwmkdi.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gbynrliet.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlyyepnb.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geltyygep.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/glexvuquj.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmgvzabs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziyfxgci.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/guyqcyydy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvfmvcis.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gawplvjrt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgpimzcw.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/grpkresjo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwycmuwqy.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/grjeiojjm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gehlutltz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptelvada.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxvaycjv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdborrzkb.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/glhvsuqdr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gnxoqisgc.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gtqaotxnz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gacbtomia.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjfwjabx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gixlrngef.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gqnemgbtv.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvefftur.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gatnvsihg.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gtbzljbvm.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviwcfeco.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gixglzllr.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcjxeaqr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gefepnzxl.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gtyhakvfg.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqgtndbwi.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gaieafymp.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/glrfqmynb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gwypryrcr.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiijanxy.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbelsouti.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gcnpidryx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnksukwfs.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdqlemqn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gggomyral.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gekmckias.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/glaofesme.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyshesiop.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gaqfpkhtw.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpomxqnj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gypijglfd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gjffbkxmb.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gmopdqlzi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozhsisbr.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/guahdxujx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbxwazzo.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtcbhxkx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqaggjho.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gidkmnvrm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gqueebmfu.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gmbbxmxtd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gebqagdia.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuqdyviu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpktvsbry.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gafsdmfwx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjjinbmy.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gzfvjnmnx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gphpyffzl.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gvwitcmzf.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjfkarjcu.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/ganqfjhvg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbngtvofh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxpczslz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsnovmcm.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gkmldwqpi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gehlbtyvp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgecwssl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gbqddosrs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxhjooccq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyikynxa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gpkjargnp.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gajtdtbnv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gppxjvhif.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvjucwnl.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeferbpu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gaixjpyfj.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/glilapmsz.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gghwlissl.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/glusxaefp.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gawthjflc.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gjboetall.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grwuhfgkw.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gdprubnsw.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gakmfhtwc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmdtzyft.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrdltcrq.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcjvsxag.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guideeath.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gglsesglv.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqhuurdy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwopdgvs.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpmmienl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfqhhgdzj.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvspgmsyn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gljbmkpzs.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweyhquat.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvbgqxqy.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/garpajmnv.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gbouagaax.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgrjsxwy.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gacwdxjhk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gghgexdqt.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gdehmaktu.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiwcjcxl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkdcfvmgf.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzeliwzd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gulopsxks.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gmhaeoczy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gldurgkln.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibkendga.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkszslnoi.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxdvtqlx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrblttbq.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gqbltygiy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznqebvma.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhzfuukz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grwfbzrfy.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdwhdrjb.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvmnadelb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcufqormi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glnbzkidy.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjycwktno.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzeikkvl.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwtjtzyi.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjwgrcdis.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gixbbjqff.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjxexnix.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxuffvco.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkrvvyte.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gnboypvfv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnfszeryj.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjsuzsem.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoxmgzvh.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsissekt.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gfosekqgl.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gplkdmqyw.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/grsonuldz.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gspchekna.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwchpvezu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmzhtiuo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzbcatpl.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/genstazto.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqveebfaw.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gihbsigoo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gguajfkqq.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqfpwqos.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowvkdzvk.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gjoltzwxt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gnlnybhbx.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvtxeksl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehlafstg.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gugylpqvx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gkhgfxrzy.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnhwlxnbn.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/grycjdywe.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gadavjrmj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/geuwbkghv.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/grrfklvfs.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxodvywj.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiofsfaq.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/guwzjepvd.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqopvmdjo.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoblpcye.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazdndmzr.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvrpdfiw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gissxofyd.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvtwjwkg.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gxxclcxkt.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gntouqdcq.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaowkerj.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvjuicbj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfcboklf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/grholkuoz.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxocuxow.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfmlvxqm.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gdisxeeuc.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyndgrpvk.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvffetiu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gculqiuri.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksbleejw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghjssfnbs.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gwunjvfyl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwmhhzqp.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdpzlboy.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzobvvyhk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gccwfrdhx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gvbqszjfr.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gndigasjc.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gplfbggrm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkixlltb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvhlzkns.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gyesuzfki.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/glvsufdar.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicyivfvm.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gnuurvjad.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxbauduk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwidjprc.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmpnlwpm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gvmomsihg.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsskxmqz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gqlpsswzw.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gocesulis.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gfwygboze.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcptbmwx.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gkgqxothi.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gmpppwzka.sHtML


<!-- 参考信息 -->