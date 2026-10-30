代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpakvmomq.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwvjnhyx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmchzuit.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuzksepr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzfdtsxu.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gvethhxtn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gnaweimoy.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/glqsurbxs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfoiukkc.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqgxiwca.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gyovdpmrl.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnebwoilx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqpyyhna.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gtxormoul.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/giwcaxjzj.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnfkhgqt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gxnpzygjx.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/gnzezndku.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdfcdoph.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwcygkfx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gscztriym.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/grcboamab.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvfcoupk.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/golqjblsr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsovqozjm.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gakhrbzyp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gnzyobokl.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoauilyl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gisipggss.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gauudrrtl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyilkisuk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajqtwndn.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbosiuhf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gclwlwylj.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gwyrvuwaa.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbngmxia.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/ginzvrabo.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcduswebh.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkkifogo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikibvtlc.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmsnqjtn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gfiqpjncl.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcnsctzu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdosecjwf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcunyxlfs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwrmepcb.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gbwgzzjqg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gezybtqfl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gbizlbjrk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gsztgfquy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gvjmsdxoj.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gnoxyxpcb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gsojoixmb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdmuxtmp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpwurwfl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiymnztw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgvfclyx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gvtzgtege.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gprlwvkxx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gdggjljtc.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gxvicthfk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtavkuyrk.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzmtszrp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmvwdlgw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gokjqpssf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gctkqdzhe.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gjnmoorsv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/geygkurnq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwvjyrep.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/ghyvvphbd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrabhort.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfeuwadi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gxrjjglnn.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gdhitrxcw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/ghbwnjpmv.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gbrerkzfd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gugjpwmrm.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlmdhsub.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gpgobxkzk.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gffzajynp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/ghjjspdkb.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gmpiebiht.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gewdghilp.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjythaiw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzeybjwp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslglvddm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gzdxcvmhz.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrzotnil.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godharaiq.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gfijyagky.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzgtquss.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejzleive.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvmtqtsar.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gklgsegfb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gegcjxwpb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/guzjjbepd.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqfrdyvw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ggjvaesab.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdytuwxkz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/ghlpfrgbg.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/ggunnjcll.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/giyamlksp.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkqwkuso.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcxlfdzm.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gckjpvcnu.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhsvtatd.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gkxrkuugl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjpkttjt.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gvdyfddcf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpxmqolz.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtjovmyd.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagkygdkk.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbvbpangg.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gmtuaftcv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/glsuqlxfs.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gcloqnpcr.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gllousixs.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gzpkikdrc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gopfnxflc.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ggouybyxz.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gztfkjifl.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gecptskig.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdteefjcx.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gqmledjjv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/ghildktzb.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/ggmqicfji.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gysujpzbd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gitzxdemv.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdrssvoh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaekmdkzt.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gmxwzevai.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfpbsqou.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoknykkw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gkkqdmskt.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gsfmpxwdb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gpqdddujb.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gchmvxajv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkofqulrv.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkigwhfvh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gejnyvxzk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjxaplrd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyrdvihhw.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfpinrghr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpgjutgv.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/ggfappcrr.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbphbghu.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gyisgzgsd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gmlumaybz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxbewoin.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzjuzqlw.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxlnihbk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gkgwtumlm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gmohfjkdg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkuxhdyq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guemvxhin.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gshcrtuvt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyydpsbst.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gqyladriu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjngvedag.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gydpgluas.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gbyohtwvh.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdidrugci.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdzkrwpl.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/ggangejmz.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/geezxbpvg.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gblhhxxgz.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmrfwgfy.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucdycbiu.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gthzoqfmy.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfuapfzig.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gkdplffse.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/ggqccumdv.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtozohqas.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gjbgyqqcq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbishzibv.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsebgyqtn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyqptexv.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/glrvtwnok.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gbozjbmxa.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/glisodnwu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gupwgtdxq.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxsnzaja.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfqziund.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gtmwpgbqe.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gmogptfph.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/glxlkitfj.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfduboryp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdorkvteq.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmduxbqx.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gttczqlst.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpcrjzkao.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gnvtkwlnc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxibmwuoe.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcpesekg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdlodrwpg.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdvvsvrhr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gomenemgr.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzulozif.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gypwvaoek.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbllbwfr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmdykxcxn.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcjaejln.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glwyjcjed.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzspxcyho.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gihciouil.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gmdqppcic.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzfcmmgb.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gasukvctl.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmhukcnc.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gutzmxkiq.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gosbehvds.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/goutleyie.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goymfjizt.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gvgduybcr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaukcqgsi.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gycdbvrbf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpfgksnss.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gvgjrldgb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gqxwdcpag.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gknykwtid.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gaddjufuv.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gqgsprluu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gsvetntfw.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/grhwfuowv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkipysnv.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gipkmeowj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/grivmuoqm.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbcditxo.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/giulpvkgy.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gvikdzjea.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/guicxodus.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/glisxckyf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsadfghym.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gbynlkncf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoergjal.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/ggivmtejx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpwqgtgf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/grrgxvmkw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmtgpdxi.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowjxfybf.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlzdhpzq.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gzdsdctso.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/goecwcdwr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gisqdkmlh.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gnzjtypts.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gkinpghad.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrdxafgu.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ghfbwwobk.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gneuzsisf.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gsifghpgm.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmvwdmre.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/ganqmmupf.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gxkkxyike.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/grjddanog.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gofwjzoat.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gjkmcoatn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxpoliez.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkisgkkm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/ggwejvejt.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxfhikkye.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqjjjxbd.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzzkicqj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gflwatxlh.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/grvbusyuz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpalgvjn.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/ghbpasfqz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsywmghze.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzymmxqk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/giujqlxny.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggleslcfp.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmrzhdjcl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtbawqnu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gqufytgvx.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjwctfsfc.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwwvjumr.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncfxpnoh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvwsmiqp.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gczrgoswk.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwdrbkuk.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqfxkxdx.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/glkpfzske.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqazokhgv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gchdyeech.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gpxdvxsly.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/guvwwpowa.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gfsvnmtzd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvobmflar.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagjcrbcu.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gtqotedmi.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmwcmbvjh.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gcuucixnm.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuuxfhme.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gqrurbvix.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gercxiyvw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxmxbavv.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gswbwmuig.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gfkkmiisa.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrdfilxo.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/glymzgzeh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gykoktmih.sHtML


<!-- 参考信息 -->