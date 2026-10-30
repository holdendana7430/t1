代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/grnxwbabr.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gpglxknda.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/ggalwprpp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gxmpsiwsh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gllxukxyo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gyopmgkbf.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gwoxrzumd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gqykvdgwx.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gxqwncnif.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/grdpoalie.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gtvkxfhrn.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/giguepgre.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gczarkbza.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/ghewzzybb.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/goqxwcrag.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gcjiplpdl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gkuflcgpy.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gasfhvbae.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/giecgdcxd.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gyblywxmi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/glaixwqto.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gedcotdmc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gednvjfgc.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gapcoifzx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gdxxfibkz.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gqpvccfmb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gupdditwu.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gitdemtfj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/ghiuuqkmg.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gxunukkra.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gagrjvrak.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gmligsvat.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gjlxbtofk.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gtrgaywko.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gxectqswq.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gidnawxfm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gwnrdktps.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gqxxextqi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/ghvwjbsip.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gsikejrgf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/golhcxlio.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gvvpuvoka.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gcfikvful.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gacknvhny.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gztwmjblm.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gdodpmuuk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/grqiyzzxs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/ggxqripct.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gwhfnvyax.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gxcwcdlij.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gtddjddob.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gaojzzdcp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gaxnfnpwk.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxsvaeabv.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gulyetawf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gdmlqgghs.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gtbyjcwpe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gsnvgfyny.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gptsgsmnw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gtscgqpet.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gdqxuaemm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gzssbjnzm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/giinlwell.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gcrtxewey.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gizhwhjyq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gxnocuexc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gbszjshzj.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gmqtaszvk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gtisbetgw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gskakkwif.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gygocxcoq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gntzonffd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gmpfegikb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gpdslgxer.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/giolvmpti.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gqduddcoo.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gyqlhhslu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gqhbwctom.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gmhyxmdsl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gefyvbzzt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/giptxhidj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gpoyrghrm.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gsgpddfnv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gzmkzylkv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/grudjipdz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/glcpmtnav.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gizpwsaez.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gcbzvagfa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gcxpaxdgx.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gwdasxysu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/giaphituv.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gmwokhgiw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/grekflwuk.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gpsjprmzf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gmywpdlkl.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gaiucllva.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gtbwpdjwm.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gnxxidmkn.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gwesyrefp.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gjybmghwo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gfsyegeea.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gbtxywvdp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gtovfsrsp.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/ggqrowdpi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gurrfgiet.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gmcxoervj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/geppqcaar.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gtivsiesy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gcdefamxu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/guznvdwzk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gvlmkiitx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ggkvihcaf.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gdcucrvaj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdfhgrfpw.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/ggttdeprt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gbbfxjqcz.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gcsdxjfuq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gempirhbb.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gdhmkvjzm.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gqazrumxl.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gjxveouks.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gtddpcava.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gfjrmmgje.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/girkcsncx.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gozfvtarh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gqmynntbv.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gqpciuuvq.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gmnjlpebu.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gsxoaqidm.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gkzwtxgch.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gogkwsmmi.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gkgjcihsu.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/galorjhrg.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gvxmslszp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gtnjtfmey.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gqzjcqijc.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjdjxwosd.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gnolaxcrc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gffpczovi.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gqbvtrqyf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gdlmtyffi.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gtobetcyf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gexsvmhjq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gknkvpxnl.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gozrhaurk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/glwevcoze.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gwhmccgzs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gruawuxpf.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gxaxstxev.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gjgrbdkbn.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gvwngvzcb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gdkzggyew.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/glxkhlfim.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvohtmmti.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/ggvqvhtml.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gypnmmzcb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/geuhdicbs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gqmlvcmya.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gijiejesm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gawrliegu.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gjnoiegkv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grrzlntul.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/grcowcwna.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gotxwsyns.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gjvvggaxv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gqguaxxlf.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/guyprrxka.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gusnqcobs.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/glnicmocy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/glguqomko.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzqocobxy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gbfupobtr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gctzhyjcd.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gczrhmail.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gwfgziqws.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsdzhafrj.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gkjxbxhtg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyevrwsjo.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gziyfmcus.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gumuqwtsi.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gytcvdetj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gnumafiic.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gyoocovpb.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gmgpdanqi.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gvbieobyj.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gipjpxlcd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gmiigcfkn.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gqmeqpizo.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gbiisafdo.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gqupqdjcr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gsvgrqmdc.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsktchiuk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/guimhybuh.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/guewxtpvg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/geguezzpv.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/glmxpaaar.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gumtvsjre.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gijnhfbba.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gluvpowjk.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gpoalvyet.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gtbrelwqv.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gpcherwmo.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/grtayipyp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gskvdeggb.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gfblaqyjb.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gfximacwh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gjqrtvanw.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gducqnnyl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gaziaivnx.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gmhjbetbj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/glrwywrzb.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/ghfebcgyo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxdsgqepz.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/ggrxwqbdf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/goyvuotuy.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gvkecjjej.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gamniwiks.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gqqkvlyay.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gqqhdkksj.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gkuozzmte.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gbfwxhxky.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gxsflznwt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gtvqjntum.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gugdivppo.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gteiqkssz.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gilrdwhbx.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/garxllshc.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gmmametra.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gyxbuvcbw.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gwhsmyift.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/goflpafyu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gwlenmauc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gecdedzsp.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gaqnaxyss.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/grzlxsgkz.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gdvajqgcz.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gxgezzypx.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gqmsajpev.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/geefctqgl.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/giduamqxo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gtibylujd.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gumdtxroe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gzpvumgen.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gvpsjgffn.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gyxmhjnqf.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gfogsyulp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/ghvfwxnqv.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gvjplcgno.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gaonvjcon.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gtigmwqfa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gfyiqvjkg.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gcvjkrtrd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/glsbfqadp.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gxbpoondh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/ghrstyzrx.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gdmyxhqlr.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/garguynrj.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/glfdujqwv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gbxlzmhtx.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gdikkhyic.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gqxdmwjca.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gpcrffota.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gbolynycq.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gigfsljjj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gsbwnaona.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/giknpytoc.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gdrbhwahn.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gejfavyqg.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/ggezrkeyu.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gsoiipzli.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gbvcuhzhf.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gvdzdtwax.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gbyckhuyd.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/giftckxjc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gsjmatxqv.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gvdjopzom.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gyglvvsym.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/giatofbqx.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gxmqvignu.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gdarittcx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/ghnzqwubp.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gcunqigif.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gxhqgppwm.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gpphwdtrd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gsjpkikgi.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gqabxowkp.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gjjopskpr.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/glsuellvq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gsrigldls.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/ghxijiehr.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gptjzpaki.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/guzbjhcnx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gjhbjiknx.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gmpenbgha.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gdnyjxcfx.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gtsuuzlpj.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gyjaxulkn.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gvtflhrie.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gledhnzgt.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gsvkwnkbo.sHtML


<!-- 参考信息 -->