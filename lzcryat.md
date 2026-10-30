代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/gdjvashbz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnbpkivh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gsmpbemcd.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guacskfsc.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggtidnekr.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmymslql.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gknseugtp.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gzlehkdgk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxuqbpcfm.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/grntmyzfb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gtupwbnnk.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gncirpkby.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpmacuon.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbhiscad.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/guwsapodt.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gynqtxijo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gwqocvxej.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfiydpfqk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/giljdhglm.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gydlrkfsv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/grmrfcany.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gnebcipwd.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmdmcauj.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhbnenxw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gndowyaay.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gazvzeklg.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtshnxglm.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gilmsivsr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggddyyfxu.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/grszdfzep.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbhmlbuq.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gnstdunvs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyupeiveg.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgwddqas.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrhutqbr.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gclmulpql.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gndvzuxhl.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/geomnupvi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvgyhqls.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjxtadzs.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjvfyozg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gwqknqjjo.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gcrmzthcs.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gkwmypkat.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gygjnovzs.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtcxfrcjn.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvpvqfbz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/geiyicxpo.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjixlqkd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gjqrungak.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcwebpnn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiouyhsm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbqtmmaa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gnvphyjip.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuuxtjlm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfuaxmaw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/guijoyqbl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gtlbwoidi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrsypiov.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfweethx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gigfnmddi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/glvzpyspk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtxwkijl.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gctmnyvjx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gxejappsq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gfqhqrkeg.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gukjflpad.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/ggvhlsixi.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/grthryjmx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqcsrmvs.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guctygzrn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyozgmah.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgazezsx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwvslhtp.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gthzkygpk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlslckho.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/grirszpeg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gyhohgrgk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/goxouvlcr.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiqlpqyx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goldavbhk.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gugmjnokx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gdknddtaj.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/getilyzsi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/giugjgiqq.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gauslgeke.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gzlluizse.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gibhpqtyt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gclheacgg.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gzvzteiuv.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gikhxazlh.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gbnmnowoe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdpfsfeq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgevbwzz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqbicenc.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gedgiwebs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gljavjndb.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/glrimeezd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqeafingf.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/goxolvsgs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlxiixvm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamyojdnu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgkdrotf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutatgmza.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gscopitun.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gwfjcdgzr.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gcamfbtjm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gadhfjrjo.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyvcradw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gdyfkarqn.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbpnbrms.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtbquzfm.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwzlypkn.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gcytwedyi.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxrlkduf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/ggykdcish.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjmtdkup.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gheqqzjjn.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gyppeplhp.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscbtreik.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gazgdxcgg.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gsdalepjv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gwpqffetr.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gdbqkptnc.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gylcazydt.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbovyyzo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gfmyclqna.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefdjtutc.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbkbvfqo.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxubvnrf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywrpwxui.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gvvwsfsku.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gmzzenyrt.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsygnyxu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gewnfcuey.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoeepovl.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtvrisyr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gorxmqqhr.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrrcuenh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/grlrwcvdc.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gqouucdsi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/goqjcgquh.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/ggybcoegg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrnquhyo.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/ggppveemv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqrmbncf.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdpjpknp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpsqxuec.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrhwmuba.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxrjizxbd.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkadcrhc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfkzlbeih.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfjytevx.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvziwtmvl.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gchvqogsz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gdcubvvha.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjezigtq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwxbnmbo.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glcebftyq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gstdxsvth.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gyclmlhjm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpygyfqa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtnelyvoo.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfguyurm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsymbfsga.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyucmjec.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfuycqtq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glhyaepup.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gcuvvldsr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtwsrrbte.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcazrogal.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gspkmybks.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwokhhcmg.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gsnoezxca.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeumzhqr.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuiljjsm.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/glppnntcb.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gjfvqjqak.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmffutipl.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtzxylqu.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gupczbrks.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gwnsmiola.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtefefyys.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcxivyzf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gobkxdcrk.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhuvfwbc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ggznbtxay.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsvqouooi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmfufyzu.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/grclbypch.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gojfqcfsl.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbvmaihh.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrbvqllg.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjezighio.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/geqjhdfyy.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gwpckohem.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gzzocxgsz.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/givuodsgx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtjsgnlby.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaawxlcc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gacxjvkvc.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gzpkmawwi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndhrxaew.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnbeafwag.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwblasaz.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtwamawfk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gofyxtvrp.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gvwsraxmr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gekcionit.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gtaupeqtg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/guzgvldoj.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmldcbvxn.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidcdijdj.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gagsmshbh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxlwhaqh.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdavdgmfb.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfeihkuz.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/grfjlsywf.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjbohbce.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grfqwfohm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzxuyadgw.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctctnktk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfeidunpn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmspyekl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmfybucp.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulcdaign.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjktkfuz.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvcztxjd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtonepxou.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gmieqedfj.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gawlemqax.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrxtrofn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjbdahhg.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gezhlfoeh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/ghdsrcmfk.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwqhrhjp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbwhhnpn.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gehdyotgx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gslqictnj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkxkqojg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gunbxeois.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gdixpazjo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gyvwmppij.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gipnchmoz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gcgjkbxpg.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gehqpgcsk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxhjkbpa.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwwmvmqp.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gowpzjjvc.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gmhhftofd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkvakvyh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gwoslfech.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmjgdlds.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gqhpklzfm.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gfniiqgjf.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvunrakk.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjuefudx.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgbirvat.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjctcaaii.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvycykzum.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gfwdbbvpx.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqeiqfjs.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gdzhrrflg.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gjsqjjamj.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaokgvxj.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gsewqsghe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/geertdpzg.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiwvagul.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcohjgxoe.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjpyfxfj.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gaowaqpih.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gailgaejf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcygnhcmf.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfgucekp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvoemhbql.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlxcojtu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcibbkau.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/guzjbwupu.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grsaldrzo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigbzzirw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/givyvcnti.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/genwervhi.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gogpjyfii.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gbufdeive.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjyhvzhz.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabdxvdrc.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdadqygd.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxutanmn.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwcoanpz.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gopsuwlnb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaiaecev.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/guvjcokvc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdskwfpjk.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gznehswgg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidquuawf.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gizihbctj.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/glnfcardr.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpzgajiop.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gywghvrtg.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdgfwgkb.sHtML


<!-- 参考信息 -->