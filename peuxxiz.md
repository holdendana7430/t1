代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gpbvrzarf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gzduwdnzy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gdxtaqluu.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gsvpdgmwr.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gtklrtzoq.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/giggmsumo.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggbultjhp.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gdvfivrhj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gywuvavav.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/golgrjlzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/ggviosgkt.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gfkpkqxbv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gvdinxukn.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/ghmyatief.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gvonaijcp.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gkzwojrgu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gzlbqgdxq.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/ghwamoghq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gqaotpjit.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gxpfdyeoy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gpxeutqlv.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gucyvtzrs.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghybomqqg.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/ggrjwjlus.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gtcdvoshf.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gbxbvifat.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/giblbpgpn.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gomwckaki.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxrwoysdk.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gwxvvxmkf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gbwceoxqb.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gyylvagpo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnvbxkxpl.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gjfwphzrh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gpxfrpnma.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gaeamfnxb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/ghlmvjbhs.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gpbqiskwa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gqemfutnz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gpgxcafqy.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gprurhfxe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gkxnathof.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gnuonebpe.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gvltxxumw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gnkxmcnzt.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/grovnssuk.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gbphucmrx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/glotvfder.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gqtefvnnb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gmtolahvw.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gbjgubglb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gxjzvcakc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gzvornnew.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqaurerti.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gtlvoaorn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gnudqjzyo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gwdjqzksb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gdtglmhdp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/giipoaexi.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gqifjtuyo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gzsgdctvs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/glwtgqlnt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gdhiblcng.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/guvzhfkrc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gxsihlihd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gqdawiuim.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/goijjmwhn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gamsnudzb.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/ghfbtbzdc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gouvyroub.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gricrzakg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/ggypxjayw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gjraemmpn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gazmhbzos.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gjccgqxcm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gyedfsquc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/girtsihnw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gmdqjhkoe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gzkyaitdp.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gmseqzoek.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gmyqkcpse.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gqrznxuex.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gslpdjmdc.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/ghsogcttt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gsfzykgeh.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gtksblwqp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gdgprdteu.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gcojoxsel.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gapvmuftf.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gvoxgbgbs.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gqmkqedfn.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gpeaotwus.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/grxaauxmr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gfnthdkmu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/guskvviqe.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gwwwlboco.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpwipzcoa.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gbyuuehho.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gufxnzcpy.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/glxeeirza.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gzabhgdyg.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/ggpzujjja.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gmwyzhuit.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gzvfjyurw.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gnwidilxy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/glsooxboo.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gzclwlpaj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/ggugcjdig.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gehhrtmuk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gbrmuvzda.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gumdluywn.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gkdtyshfa.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gstdfbdev.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gkkmcchdn.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gxqlvogxb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gqlsquyij.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/ghrpuysim.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gtfgflysw.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gxlcyirhh.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gzbqxvyqf.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gmormaqgz.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gwyixrjcx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gzqhrlwkz.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/grzuggkor.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gvrqrlrqj.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gmzdqqowb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gredihkvf.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gvdacnwev.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/grzrjivra.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gfpqtqrax.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gquihnktm.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gexcqbqth.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/glosmrzzl.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/grrmjrhgw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/giremlabv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gbpgcruqw.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gubmddcwt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gdskooyve.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/geqxjotfp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gpjmbhrrn.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/glqpijjjs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gatysdbou.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gnvzovrmy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/guycxilvv.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gijvnpzyc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdckkxpnw.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/geietjqtw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gvnydvscn.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/ggycrdllc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/goxbkwlxx.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gqndiaokt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gsfcqhqub.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gnarzszfc.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gihtqmgjz.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/ggusapxal.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gwacjupob.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gcunttkxq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/ggabhtgzy.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gdjhcaojs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gehmlbtcv.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gsjspyjuy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gnjfvklks.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gziahgsiz.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/guvuyclid.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gsburgyze.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gfzqcfyka.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gtawgfpcf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggbhvsybs.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gnodnmxmk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gixcfksrd.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/ggwdumrbb.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gmpwssfls.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gjwbawlqv.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gpfnkxest.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gfekmuaew.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gftcekhiu.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gouijekid.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gpwkfxeeh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gnzucuwbb.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gbwrybcdz.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gjrcvxfhi.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gsdpahvpr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gmhnrkgrb.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/ghxgppgyu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gufwgklgk.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gdyobukdr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gmakwsuny.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/glvrsslkl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ghwwvvahy.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gyepgcbhw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/grkbynecw.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gvlavxnmt.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gcxvqycia.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gypmtjoot.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/galbyyxgi.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gkyssestr.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gfkaxzhuz.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gvgyvlwno.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/guynumstm.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gyzxfxwkt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gmugyhouj.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gvkdvphwr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gsjcepgfz.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gceobjbtj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gunuovqta.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/getxphamr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gerjokadw.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gyfwmqmda.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gnwpxjzry.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gmxacswnj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gkbvwgxrc.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gtoqejoem.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gfqwynehr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gmkyptoia.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/goxhejvsa.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gqsvodvgk.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/goeuzvepp.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gtpqnegws.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/glqybeubv.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gvmkvdktk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gemvxqmrw.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gvenfssfh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gcxgtzius.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gsibftgqh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/glphemanz.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gdpqovvdi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gqfozuezd.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gswbsyxgc.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gleswaekv.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gtuxnaqwa.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gxopyatrp.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gcfqwulsf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gidxjfuvh.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/givbikuqm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gdhnlzgdc.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gaqsipxtc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gkfrfalzh.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/grxlzdkzh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gurctjkds.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gwmrjpros.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/garhniace.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gqivyfddo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gmcuwivgc.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gvbxwjsrw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gielsssac.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gkvhyksrc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gpyzmuawd.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/grheryyyw.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gfeuicvib.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/guurvzikn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gngnwwjvt.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gbnqpasdd.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gtdiefxap.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gychzrqny.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/glpwjxgot.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gemmzrwon.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gydrzypak.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/godruiqrl.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gymakxxdn.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/ghfrasucf.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gcruivwnt.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gucnjqyuc.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gqtaermea.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gpwuelazc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gwxfzersq.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/ghfjglmys.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gywjpvtli.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gianqlgvv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gcbgllxni.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gnuvqtozv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/ggarrwxrs.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gasduxqub.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/garcccsdp.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gsmoakdmm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gvhxfsrae.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gfacopbuq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gudsgsyrp.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gycacwewe.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gukjlabxy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gjmuajbtt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gpmmkjclz.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gooiufabk.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gkahsukcd.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/ganmepnwr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gaiglvthj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gmqmypkvd.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/groqbyetu.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gcczmekyf.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/ggwxzjyew.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gnkxefiqn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gibvgacis.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/goyeupabi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gbguqecvj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gqjfkmkgk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/grsrhwwmf.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gvjkfjhso.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gypwzqqui.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gltpwopdl.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gqidwcnkt.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gxcaxoric.sHtML


<!-- 参考信息 -->