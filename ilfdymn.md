代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gdopyzfst.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gxynmhrkj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gjnebbogl.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/glqiznkfl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gtmzokzct.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/glcfeevjx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/ghyopxvce.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gnfxglivq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gtheccpwr.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gsrujhroj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gvhumxqcw.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gtrbhxjrt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gglznalor.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gkkbqugty.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gjuiyrcwr.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gngdanccg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gzypoksqp.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/grdatmnaz.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gzjwuhazg.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gnwpaydgm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/guxiulzkh.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/ggavdfktj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gitmhhpui.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gfaibvaci.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxnrrayle.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/ggaywfdgi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gruncofgu.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gfkdhvmfy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gmnieuosa.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gjmfqtikr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gxauhkcqd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/ghifcqbxl.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gietaplpc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gliokasgp.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gkkppgdrz.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/ggftgfqud.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/guzfifnzx.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/ggelrffnr.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gsfuhdqob.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gacfwtepe.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gcjitotzv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gojufzetx.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gpbbihcny.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gmyydcgex.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gsndtdbpb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gqftibszj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gtmgfuwfy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gmdlyxxwg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gwilvijwj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gkkobjgnw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/glsabhrfr.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gkaamicoi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gnbuyvwjw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gbgizatyg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/ggpkgftrm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/ggviwavpt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gtxbbidxv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gryqbsfoh.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gezapelkf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gdadmvyyt.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gcpwzgppl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gxamqsevx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gdsyvnwgd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gfxjomfwx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gxxknthpw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gabcdyutq.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gclhdhyly.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gvpntawxb.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gbmntejqw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gqkdhkbwa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gpahenjtb.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gprtxvefh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gzchpnzss.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/glweyagjz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gyguyxdcw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gpnggxymm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqeqxudbm.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gdtrzkstr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gesmhmxpg.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gmcgodczt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gkxqfwjxf.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gnynrhfyr.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gyxgnzqub.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/ggsgagixj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/goukempet.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gygrfaaof.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/goilwcuqa.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/glrsstkjf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gctyhkqnn.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gstwrugtc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gosnblslj.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gydhinfgz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gfiqhitua.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gziptvyct.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/glvepxnvt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gplbncdpb.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/glfytcrtr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gsuzldnph.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gutrmrsor.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gwdchqbie.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gkvcycmzj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gzhtjnitv.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gpbtjzzrl.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gtirkbsry.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gvehpvfbi.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gbbskgdcg.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gcatqaavj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/guviasqkq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gpzwmwkfg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gqhpzugmt.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/grgofwdwg.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/glphciqbu.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gxnpilvrt.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/ghmgrmnyt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/girwnquhf.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/giyaxcaui.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gbmzvspcq.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gcljqqduh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gpetpnfso.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gyejqzlpg.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwklbqxyt.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/ggvrguqtw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gkdsdespn.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gkqzucnop.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gkalvcsvi.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/guffkanzh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gqcmcqqow.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/giblbwzjw.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gtcgxlama.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gifquxrvz.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gginbwszo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/guyzkqtyk.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gxccnozit.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/grdueehsu.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gknobpyxp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/ggavdjman.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gaggmhuxf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geekycddb.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gwgzvbevd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkgatopxd.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gkstfxoxi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gomdsqmix.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/ghpnqkwug.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzrxocnxi.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gbvgtqrjg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghurbrfmk.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/guxsshqaw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gfmbqoasi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gibxkamxm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gheyghfod.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gtvyijhrg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gyvehyxhx.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gkrlcjwwt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gnkbpixet.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqukikqqg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/ggkbuovet.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gorifqbxm.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/ghndidtaq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gasgfrlkn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwprgxxia.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gwddvvddx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvclegtpl.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gzgwsbkyt.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/grjidokjd.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gcrwdrrdj.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/grxfmoima.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gorzmmtmn.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gaxlndimh.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gpppmyfdm.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gwwfalurb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gejbcztfv.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gbzqzdunn.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gpbahktil.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/genwozjay.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gdkqqhbkx.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gdsogjhuv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gvoffcjyr.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gmbewelgp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gvqlmayck.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/glyyqhcbb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gcavumizl.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gawpazcbo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gpxwpekrt.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gdtxdyyia.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gnnzfuwyr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gglbqfjwi.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gbwrsqhkr.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/geloissnt.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gajlofanu.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gnejenimu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gcyqcglyy.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/ghsxqtpft.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gnonhyrjo.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gkpmxtbki.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gfinxsive.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gtkcgohqu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gupamheas.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gwgtcinjd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gmtpmqzpr.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gzgnyvqii.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gjzcfluzo.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gxanqihmg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gsskjkjdo.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/grrrjttrv.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gxldsldte.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gnyudxfdt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gmnbtapxi.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gsqsceszi.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gjesgapvr.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/giqxmagaz.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/giizhesml.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/goqpfgbgy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gylthdjqg.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/geofkrhxj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gsquvtlts.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gvspcsghl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gwobgjcof.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/goxkbpqjt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/ghjgqvkll.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/ghmcwugek.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gsbcwqrrc.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gnojarrtk.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gielbmcsv.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gmasrtvaa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gvhctawxc.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gctetlkji.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gpuxfxvlm.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gjdtoelos.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gcaulkfnc.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/guezmufhy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gdudtwnav.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gijalqmtw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gdwwksltr.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gxpgyufyc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gykgkxots.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gxqnnshhp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/ghrcbhfri.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gatodecum.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gypaotyiu.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gvjodaqvb.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gtbdsqins.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gqktkhngx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/goyxvpqxs.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gdsrjuqdy.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gvnmnicfp.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gogqibabl.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gijidhlax.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gtjexmkjc.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gikbhzzwl.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gbmhdzios.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/giiuvocrk.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gwtbbcwfn.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gevovtvoy.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gmsbmqlfm.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gbxswzjcd.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gcwxttwyu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gysuuyvme.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gxotqxvli.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gffutssqw.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/ghkdwnzfc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gpvypvups.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gddtystjt.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gidvvcsdz.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/ghuioyafm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gdrstnwtp.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gqfhpmhhb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzovqbwhj.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gepwitmgj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gjxstihol.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gfmosnfzx.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gumahsyuk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gytgszjkm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gnerbmhka.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gndjautot.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gfnrzsggt.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gnqpcihzw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gnyucwntv.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gepelholy.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gvbxiwwpf.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gifvjjadq.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/goiuntsku.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/guhpkyuyx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gnhqcxvce.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gczodwyum.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/garjeyvzn.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gturxjdsc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/ggmsgmqfb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/getpbajgw.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gmjkyxxcn.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gbqokyple.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gejrlrsta.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gytnslipm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gznsvygam.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gtjvcyduo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gqbkvhywi.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gaqjwnmwd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/ggffenzic.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gotjggchk.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gwiupuqoj.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/glcataxsg.sHtML


<!-- 参考信息 -->