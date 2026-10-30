代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gukksrorj.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gimzzvbys.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gqudauurg.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiflqrru.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvhxopsg.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwcehzph.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbmqtswp.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/giageckpx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gtbhqlswr.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgawujkz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaqoxxvo.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/ghugqilke.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/ggoyhxscl.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gaozqcfwn.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gszylkgyw.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gemdegebb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gxltbvjwt.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gyzcyqewi.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcialjptk.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givzrppqm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/giktidqdd.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gldfgoswd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjbfdnhcr.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gakdmxebe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gliihiaea.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/geywpsyec.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcjoalaj.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjyobcns.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/grhvkioru.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/girmwjxlw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerkixcrj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gjixjrumv.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqcqcbyn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqmpbtca.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gyrryoknv.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxfzhpie.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gcprsespr.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghgtiaofv.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gyggrmrlo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/goeicrckw.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gwdkeavmw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gpanvzkxa.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/ghpspabbx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gxceqwnzp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmwewkzd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/glesziuyz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbgvrnth.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkmsocfr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/grrecaxmh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhkegpjd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/glsjzglku.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gugjqhrxu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqyklpva.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gvytnfdbl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gqhwkochk.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmsddeeu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcxkacfi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gynqrwzmm.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gkjmwomwm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gufiwypqb.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/goiyqtgyw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwkqcwbb.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gtndimbim.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gplumkhjx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gbenwamiu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdjvtmnc.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzrrsozq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gfnxkmbew.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gspuxvyav.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gqtvlcjgk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrhcacfx.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/glbothtvr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzugophxl.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gxwzbfikf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gbabwdthv.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgmvaplq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvzzqnqo.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvsxvusk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gapbtajpe.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gxvcsgnrm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxsmpivf.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gqsugkhxk.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpqtkmwy.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpgfosrb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtegvlmkt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gpfuttyrg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzdckfld.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gcuvwouie.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixtxapxb.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyplqiwj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giimlmxaz.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgswptuj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaozfnjl.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gqhacfcqn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gkuvlpthx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gpoibeyph.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/ghosdoahx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gzqcnsrtm.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjhxoynd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyyzdmfg.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gtnexjals.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcicwlhfj.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkndbtlv.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtctpspox.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbjvcubx.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gifnqhgkh.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxvkuhhu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gyahjnelq.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gzcysvstk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gxovnmljq.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gihkpmxzn.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrtuqdoj.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqfrbxvx.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gnybcmhky.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/geupbutae.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gfrrvfvve.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyzwqbbbe.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/goojyccpn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrubudin.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/grniroiui.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwewkxxix.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gavfruiyw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/giyhsmdva.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmirjjla.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gohjvzfho.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gzmcspleo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrubqwsv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxorwinww.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gigtdlahk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gwhkmpmxa.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gzrtqtdfh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaktapail.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrfjbeqc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfestdnrq.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gaajtchtw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gphbgqvtv.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gfepmqnpt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwskizhiw.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmbzrixhr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gysesylkx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmldmkose.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuueagrc.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeafjwkl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhcjygzp.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjxamxdr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfwiotmk.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/giliwvrxq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gfwwppblc.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/girugjcwg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkylpxuri.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gawlzuvtn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/ggxjfpuxc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gpfhmgzma.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gfurvpjyb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gecysstqu.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gpysozbrf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspksjaza.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqsgwfcz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqeswucm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbionbkjl.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gydftenzt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guwmxfxts.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/goknsqfgd.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmobedjf.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnzduqno.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gochwbjnb.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzjvrhwp.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbibmvku.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfxpwfii.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gclencxex.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/guwwlxflv.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gpvixmtku.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoawnggk.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gggryursi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdnnmzmdd.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqenrrarz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvppfwnf.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwtrneew.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gydoajjac.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grkfonufh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxkpevlz.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaesdsga.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxmxgfnj.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxazxdfrd.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/guarzbcry.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoflazuu.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnxwrzsw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvueoczih.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkqtwlip.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewdctcly.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gizrqdlwj.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrfytfzm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvdqgjuf.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gghpfhgyc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gepaazxjb.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gahupcgjm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gupyumwrq.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijbtawlh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtjemywb.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpalfdigy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbxymkbh.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gnflrfgjy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gesvgbdws.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnlzkrht.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzisnudmh.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gsjytjwrv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcwniggo.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gbfunespf.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtwzfgrbs.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gazjlvmis.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyozkwpg.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujhjycln.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gueqngpso.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyujjmka.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/giyyfpwht.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnqogkhg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwazkbzwr.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoabeyxm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/giywclqzz.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbabourct.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/guqjxlgxp.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gmwlbywal.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjatwsmt.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfdfwajqs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/ginlsnico.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gdutxnbpg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/golwzaxyg.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcebdqpls.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewkrexau.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gbgpjkzys.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqakyqlal.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/grgivflpo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gnpkdgweh.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gpnrsshlf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtyqyzah.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtjrsriq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gcdncehpz.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gryysivki.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/guqafoadd.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoulxywi.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjyeytmm.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeauwwvl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gmzmiosyy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglycqwtw.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gtpaxdsom.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoebilca.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuindkud.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrshibjj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gsditpybm.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gkzuabuus.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhfqgyle.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geuayioye.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/geittaiyt.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/ggrjvuhzw.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gftpnqqag.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gloeoauxl.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgifcewd.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywnjhjku.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfpicciw.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvehywdo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrirzbhd.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/grxosdmec.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsqbraji.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gceelbznw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/ghxrrbzrd.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/getgiagky.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpzqtxiq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaruxrag.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlxdcjem.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gbqtewvbz.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqzrywpp.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gxegjqdyz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/glhbzybum.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtvsuvzpa.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjuldykl.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/guhlamuby.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdphgjcv.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/guhahnxco.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcnpesvd.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnnxrzbs.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwnzqijc.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggmdycrxc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlhokpgn.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnrmlsro.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gahaibfqt.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsxbyplc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyemdavli.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvszjywp.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/grnzcqfid.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwtclahe.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhnosmht.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtxcarxv.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrduermh.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gruybiwyu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxlgysrp.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfnetdgi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgchvmzr.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gipvkejxs.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gheflvkgt.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/glloimylw.sHtML


<!-- 参考信息 -->