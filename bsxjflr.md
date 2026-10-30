代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gqjpszeou.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggysyzwap.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndobjnff.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gzgykqkxx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gxkifmejr.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gyjkbpirb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmoyiokhb.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/ggmgknkit.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeknmceq.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtofasxz.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlatuvxl.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/guwavfnxq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviunlksa.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvdsjbfx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgdkrhzm.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznpkhrdb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glzcnmmrq.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnurugrk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gbdperznl.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gaweiuvso.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvdiickr.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gowzqeouq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gjyayrhez.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsaqlfuw.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gabcfdktg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gvylbqfvk.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/grifuftbq.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gcosdtnwy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpoxulzy.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glnxklijd.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gmlovagrw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsfkmdys.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyjaosbk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gluyydiwi.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gomxjqldo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gymcouhmn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveavnpxt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gtqqfzcrq.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjvedjno.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaczyebq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gmxsfdaox.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggocmzmoo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/glyoilrvl.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/glzyfpjpg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/grcnqtkho.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwagcozw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gzyotsfvg.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gwcjyezau.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmzkzqyt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjcsphkn.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/glvugyofg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gosumjjur.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gdwwvdgjs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gehhvzsre.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhknfzqv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gzbotsxan.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwigbvoy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gliihbprl.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/goyqtusfy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjcwhmpu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gtykdkevg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnrdcsdu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbscgfbat.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsceirns.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gpvldgwez.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gesxscicy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gphwywnjy.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gihvouuoo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwntgpbhq.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gqbsvesvr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gjzvoxwnt.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/goaqfccdq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gdlxavtyy.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxuzvock.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gfxuosjqe.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gasynbhyk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwjoxlri.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihfrrnlz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkdgskcm.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnrwmjkc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqlhalrli.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikgtzbbz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtbwheym.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gkbalswom.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrrsymdh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvoqpupo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjrwmnyh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmcqqflc.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsgmqcrc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/guepbnlwi.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/grcyiwgkk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gbqeexqsz.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gghazrovb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gywgtxhkr.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdczriaq.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gzsmclkpg.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhdmdvqc.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gzswesgow.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjowwxqrv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkokwlhym.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqeypebt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaohwlxui.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpjetrfj.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gnpffiksr.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfnbtbik.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gujqjscnm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gynwpfqnq.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gowgxoimd.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/grtamxezq.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwrxzltp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhwpjqsa.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrvcopkl.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcvxlzht.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/glyzxaqgy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gplqpopnb.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gsklhbqsc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaskodgl.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gjmfkjfxy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoitqcxz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfwlzgsp.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gklbdhghd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdggrwbi.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyfhzusu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gokvrzojb.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gblyzsyai.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gunrhvgyp.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gtszjjnhi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/guwkwrehq.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gkacioyvf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqltqnzu.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuxsklxi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gilkpbkkw.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/giynazjnt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvwbbhubp.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gzgqnrryq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfrlivbs.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuaivpbj.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdhfgdsud.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjqeipvy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfpujwec.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/glnmajsbs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxksuwjgf.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxuruonc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/geqpgvhmk.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/grepelcyz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuywardq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gskiodgka.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbnclmmx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqwsnswd.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gglzevbta.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gcytoexas.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgrshcti.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmnuzvel.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guyekldie.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhpeqmfw.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/ghojwjppy.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/guurbbmln.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybnmgikw.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxggsvits.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqvuddjs.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuofptes.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwsfoaojx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gswmbskna.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gewrotedp.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbwvrbcb.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqngndpy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggwugkvhd.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvptsgabt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfsxoayr.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gqyovzaot.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/getkqcxod.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/geelvufgf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxwsslaq.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gjrpqtyjh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gzvjnnmej.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnhznrzc.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqwnetrq.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/grbpbfbmi.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghprdzexl.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxbgzfvh.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gayhlisru.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gynsaitld.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvfgyxvkp.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gwdoswsco.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkszbphfc.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmbuyxsa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxikjoxco.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrfprmti.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzhbfvqfx.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gprcbhxcy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmjywnnz.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqdpjvaw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcqoenljp.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gudybtmwx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmyqcnyfb.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gfqpiegtw.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxihzvrrj.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/grvyrmjvy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gezxtbdim.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/goeoerxqw.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsigmzdel.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfddmbkfh.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/giqocnmei.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkawwzbhw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gealmdfou.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzlvuiyd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcmpdgodo.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gydbhdxte.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaihaqqqo.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmtiamxcg.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gwrbsmyvq.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcbvboap.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/ghsfipfms.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gwvcmdtqq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gudixtufy.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcetixnm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvhdqjenn.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/ghecebntd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnvdtiof.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluwhtskx.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gktombuch.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gixvgskif.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhxkeihz.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvjfwbza.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gaheqgqar.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gldstyubg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gszcethdw.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gzfjvhgvp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gucyvunyk.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gavmuefzn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gucmqfkbg.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvjmuinqs.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grabbhpom.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/grmmlodvo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gbzdtswof.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gchzipxoe.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gdvccjpwa.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gggqeonxd.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmefcihc.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmspewlnd.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gibzdsisc.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrsrgvwo.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfvrfoln.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhebuhkl.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdraxtjv.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyyiorcn.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/goctmtjbj.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaitdxcxk.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gnzpshfmn.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklrgqmqb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gaafisyfa.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gouxhgzau.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gedxjurjv.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gmscictvj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkmeonfa.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gaazkjefn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/ghhvryhxg.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gscklcbkt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gshxeexvk.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/guzpoelel.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbmoephs.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbzlkdql.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeccclfv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqopymky.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyunxqbv.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmftkakik.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxadpntx.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjjdoxfr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/glsufbfhd.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gzbsgzoeo.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gjajtdghx.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmeuppnn.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/grujfnnpi.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxwfvojf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gspsehanm.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gazyvoqnz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gsudbwvud.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gghtwompz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/ghbgipjab.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/guydcgjuo.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gblegojme.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbuelpnn.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gjpmwnfal.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gorwoyfty.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkybxochy.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/glmilerdm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpgvpttw.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gncwxcnht.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/goycsfuvl.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjifrnmyv.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gvntabtuo.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpnphwjo.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/grydgbhng.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxikpfyw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjmdwgiu.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvpgfvuk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrcziynr.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gxieqljez.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbziefua.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ghmrvyxuq.sHtML


<!-- 参考信息 -->