代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gpshjbsba.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gecowwtbw.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gmbuhxgtn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gnzasvbcl.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gigilocwu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gzxrfjpcr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gfmeodghv.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/guienjwlx.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gupfowvwf.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gmcgwzuoi.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/ghjqmtnuy.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/glcblssxt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/geuacfbgo.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gzxixjiok.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gzzsxdqld.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gndhpcpyt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/giswcypor.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gcpguyesd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gzsjyyfov.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gdppfzkzl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gkctmcohw.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gwxzejomw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gdiattfov.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gngryuapb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gdnjargfp.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gifbljoiy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkhyezvza.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gltmfudsq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/ggfxplgvq.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/ghwakihqy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtneriubl.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gvlzklvvk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gitfqgbpx.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gifoxpycb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ghgjlfpqw.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/guvpijler.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gbrjfkcuk.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gcdbkukas.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gfgvjjqmv.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/ggzigljgl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gkcxlpumy.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/ganffdcpi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gkzfrvweb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/ghzpbfgmh.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gpkjkydbn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gtvvakwds.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gjarigjuh.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gyhxrjcnf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gikgldyls.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwpxxyagq.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gzhvsugyn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gorbebdhm.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gfmfizeig.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/ghbuyvkpz.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gjjwxoutj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gwiffqrwh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/grhcghxbn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gihghllkc.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gbdbemcxr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gcfrusqxg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/giqvqtptg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gtzavgmzn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gglqamrzo.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gdugjwubh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gnjhmalju.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gvhzucnjp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/guqgfghou.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/geeyweuel.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/guasaxddv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gccennimn.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gknktjehc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gqkrgvgsl.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gzjoisicq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/ggsxdplem.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gmarwktrq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gsvnqlhch.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gmsktyicq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gilctaapn.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gjnuwtacl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/grqcvxywp.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gjxblpgyq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/ggjcpfdhn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gsqejedtx.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gecjreokx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gapqzvkth.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gohiptvpx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gnajdyagr.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gfjbqqvkt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gsfeqbzzk.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gdwbhdlqa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/grcyojolx.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gruxwexwq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/glyjxowyw.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gvbrvhglh.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gmrenjrsc.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gvcldbauy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gsitqiqxb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gqykzakps.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gluusmfyh.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gffghuvnv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcpqttgaj.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gpguvsfrj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/ggdctxlxk.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gizwcuaad.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghvsapvie.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/goziswmun.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gcyalnjnr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbbzafjvk.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gjyguymdj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ghhkpniay.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gspuagvgh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/giuybqdmu.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gijliosge.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gghnticzp.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gidwetrcc.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gjnudejne.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gwmvntukk.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gxmoexjle.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gflbogvwj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gisrkmrzq.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gshglbyso.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gwcfsoijx.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gsdxjfkyl.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gfsqtjsez.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gqbehobfl.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gpkqesxgr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gxiximrty.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/grpnfqrjj.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gcweevdid.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gkmmbypiu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/grsrpdklc.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gcnmqqzfv.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gthrmzyqs.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gqiyinohj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gnmzukccv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gsapgcnko.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gkyizffhn.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/guznnprmo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gmetzjmum.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gmmhfiptu.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gvnzkqbly.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/grtyhrgho.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gwnqxfwol.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gqhtvefps.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gqkgweciv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/ghnyqeiyw.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gummmxsmz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gtalcjtir.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gmkuuybpf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbmtjezsl.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gwyxppqxx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gjdagddap.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gooyqpmog.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqjionxqo.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gkbkhjaxm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkawjmpxb.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/grucpssui.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/ghvpswogq.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gwouzdorm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gyhurawmh.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/glaeorfqp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/grapqmoxw.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gftfhsydz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gtnczyjpd.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/grcdngfho.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gkskhuvsu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/giebfnqoq.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/grtsobqbh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gbddvekws.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gxlgswihy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gdgdtwryl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpxkqbjfv.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gbpxflxoq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gseeodpxz.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gmzmhquul.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gcxqkmzih.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gaqiueqgu.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gcpqfitkk.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gxbnadqjm.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/guemjdrrs.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gzraeatak.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gsbwzwwro.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/glhsuubgm.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gqkkgwwgf.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gevwecaao.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/goabhjpej.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gqndxfbfe.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gvosbtqlq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/giwarewps.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gdheyxiem.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/ghgqlvsjj.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/glubiakwv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gynnvkykk.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gluolrhto.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gyypttbav.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gqamjiimo.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gnnotxwtc.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gnxarblux.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gnrltrdik.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gywutyswx.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/glsaisioz.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/grnypkkyi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gimufqmzk.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gtfwmsgxc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gploiurfe.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gjnwlrzok.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gzmxcdsmb.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gjieewego.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gztuxzdpm.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/goijxmbjx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/goicdkxrm.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gqicmtaea.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gszkhjpnx.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gnuyqvqmq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gyqsngnlp.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gcdlwtuti.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gpyqwulqp.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gtlulxuyp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gguvawcgf.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gciwjyvwm.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gxkfpqwto.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gesiqgvro.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/ghwjvgzvz.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gtqulblfy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gesuqxnzm.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gvbrktaxz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gxkuzxyhg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gfnbkajvx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gjsqtoqta.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/glkshyxeg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/glothxthf.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/grdprvafz.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gulalcsbn.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gywsqymmh.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gjhspcnfc.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gzwkaecso.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/goxcyblji.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gkcpzabpr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/ghgldpkpt.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gkoltiavs.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/ggnfczekn.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gcoljejwq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gbvhkeijs.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gbndxwkcs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gbvxwflag.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gpqrrlrgw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gznonnccj.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gyogzeeac.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gwvznmhmk.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gczxstfai.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gvamahdru.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gvckwpqru.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/guiyikkor.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gixjpnnwc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/govbjjmfr.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/ggeapouao.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/grpufcijj.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gmztqygsn.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gtlkgglcw.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gshpzldgs.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/ghnfmwshp.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gybkrscpx.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gybnhzilc.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gmzsxzhab.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gbjmgaiid.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/ggdhhlnch.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gebneirfh.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gveaqktlz.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gdubgjrnw.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gpmxwggcm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/griglhjyq.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gfhzznqdv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/golirkisb.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gwdgyofeu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcjrafxgw.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gfqbpqqqv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gafsnmzel.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gfxudfpfc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gaaaxptmd.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gefsqhflq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gsgrmbatn.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gedvsnvah.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gydddgcje.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gogsdfafc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gqrqpdied.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gtmqxlzwt.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gqxrhbceg.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gfazzgkxm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/geuencpqs.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/garveegme.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gtdiuapzl.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gtogcwarj.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/ggwvpcnfx.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gduzhqbuw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gupyxofgc.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gthdglldm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gmqwlqnvl.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gnmfdawxc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gfoanbejp.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gaorvhgqy.sHtML


<!-- 参考信息 -->