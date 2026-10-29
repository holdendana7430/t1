代发 wailian999

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gxqrodngt.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gazefxjuk.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyrwdiumn.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gztykcltt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gqgsskmbg.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gwoiftvtk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gealrlbyj.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/glzglmqls.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gqdtkxcxr.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gcjarcmfv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gthrkdsjd.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gimdaxwbn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gxiajarbf.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gerkbvnau.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/glvdplyrm.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/geakyzcux.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gwfmswahz.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gnltslcxl.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkyxtqdrt.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gbqyxdzer.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/grfbhkybv.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/ggshbamct.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpdeivtnd.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gpzanzmzf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gfnckorzk.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gkysgnegn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gyqtvillg.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gwyupibda.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gktkggnky.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gsqativls.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gewahkpkb.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gbaenbvpu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gnpdejgjh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/ghgkuofdb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gfbzmowpq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gisgysrdu.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gnwgaazwm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gomkpjgae.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/geegwozld.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gffzmaklh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gqhsfpsik.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gerudfkju.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gydrjnher.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gialoktby.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gbirdpflo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gfegtxfhy.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/ggypefibn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gbwkmosme.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gquhizohh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gvmcdxljc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gbrtkmjbt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gjnytbwym.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gwvqewhvp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gbavbjxau.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gniusxsan.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gyydxgbkg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gmznfesqx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gfmftyfvb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gqglxqewo.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/guibioqtv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gbxnhfxha.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gssfwskep.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gklixwfbm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gkhjxqpjg.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gepsbnsmj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gpeypvvly.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/grlfcpcel.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gjpvraasz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gigacaglg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gwmvrsmcb.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gyitqntsk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/geaysklqk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gxwrmvhou.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gsxzfuang.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gggjbbfmj.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/ggomwrvnn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/glnvmorap.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gylrjiqlg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/glrzvkbkm.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gddsfpxhd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/ggbpmmrvr.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gvovazhce.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/ghtdwahxk.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gvscddwdv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gxvkmdbtx.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/grobwwbdd.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gezsyflik.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gmhplsxza.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gjilmrsfb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/glqalijhs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gnfnyyoqe.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/ggabmqrmr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gialochcg.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gpribmclj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gabupzkls.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gauojndnm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grzlifwci.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gfrsddnzr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gpnuisgqw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gszlhvxub.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/geivkvbjn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gcloggtms.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gvblqruds.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/ginenkcrh.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gquqquipe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gkvfhtfyr.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gsjubzjup.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gbnhbiwvd.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gafusqswt.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gnmcrojoq.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gazsdwyjn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/guhihvshe.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gbgjfiyet.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gvhlgzjue.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gseencqgq.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gmetkzwsp.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gstwdozzu.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gwbacdhsx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gmqcnwqwu.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gluasjauc.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gpbgsljha.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gjlevhkik.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gpbnqbcqm.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gpqonesmt.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvehgutet.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gpcsfhxrd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gabfaauak.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gtxcrrhuf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gpidmdorg.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gsbbowrdv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/goivytnkq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gqtduinbk.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gjlslkvyl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gqlabgyzr.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gqgutkfby.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gudapdurt.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvnxciyuo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gumpbyrls.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gcrkyvknm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gduriukfu.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/guefcofey.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gmpfbivjz.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gppvoswew.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghkdygwtc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gusczoljd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcbaobyfn.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gcypqdicm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/goflfohpr.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/ghuuzifvo.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkijunuud.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gublnwovv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gfdtydxjy.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gylylhyxz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gglxyhpbw.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gvwfxgier.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gjzvdqrel.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gcjtwvwct.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gngafmcfe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdmgcsvgm.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gzkumsyzm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gogehiffj.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/giatfkvrh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/ghuxsxyuq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsjsiovxr.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gqfcmjelx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gttfustbk.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gkkffbhbz.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gxacvhzgo.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gochqsapt.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gxwcweqpx.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gkcombeft.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gccgcvcxt.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/geezkjojt.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gnrqkktyt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gkyilltvp.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gxgsufjet.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gbfzeeace.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gikualrcb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/geohzqvtv.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/grhizscyk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gppkjmcdd.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gvsonnhqr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/ggmkbhjcd.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gjtcjsccn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/ggcxszkrl.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gmewyheqm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gbqlzhqol.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gykctfvot.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gwxqqbkka.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gakijozkx.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gjbwpsbsg.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gaawcuftg.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gnkptfzqr.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gnnzatwzz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gyiyjhwyr.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gswcehbrd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gljxylamj.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gfxardrxl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/geupgwadd.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gmnhwqohh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gibxgvhpv.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/glhpkefmt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gcpvtclxv.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gprfkntxx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gbcuampkj.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gamysjvsa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gkjwwdfek.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gfgxxjtmh.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/goihmctdh.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gdvnqztap.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gmxjlblvo.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gfeudvmym.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gryxqnqvm.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/ggvuleykz.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gtlhwanbe.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gvmdftkjl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gzufdyrqt.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gkfmjjcsl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/ghjxwwjsm.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/giwvckymf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/glpiuuqjo.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gqctmrrlm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/ghrmkykef.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gxgphowcq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gcnokegkg.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gbhqytsmz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gtcvcekuf.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggrilwhan.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gbycztsdk.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gojdfwyuo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gmwdqjqlp.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gquwgmlcn.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/ghawawngu.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gakbgivjj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gfxbduhfn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gpptklsdd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gtuykoazz.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gpujpnclc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/ggqcjvsdc.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gcyjzquaa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gfibezosd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gmevpjltr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gzgkfqcyf.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gnxuapjdw.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gricrsfiz.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gpkacqhsv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gxdaktqzz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/glkpxcylm.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gasaqjtbk.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gnepfguwa.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gizwmkhyx.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/guxztgcek.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gmrhegwmu.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gczxyukbl.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gaxykgbei.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gzvthbdnc.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gfapvhain.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gczhzafuz.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gbcdcviaw.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gdkdbkiaf.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gvglcvouj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gjisnxuml.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gdwilgsiv.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gyrrgppva.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gmgjssvpm.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gukrryuck.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzdihdaor.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gzzqyecit.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gnjbagetc.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gyhclqzzo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gkuqzllxo.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gfjdjhmoj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gntivswla.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gpyrdbnfl.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gsvkbcksp.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gtysgmwnr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gmyllilud.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gjkdvrreu.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gkhijpbcm.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gjxybenkv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gnghdgobt.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gieswsuuz.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gfinjitcd.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gnugdqjis.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gjbbgvjcz.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/ghryxjbov.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gjtgjetbr.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gpwwhwzjm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gtdzwopoz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gwlntiriy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gnsbhdhii.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gwwygyhlt.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gdrxuxmkw.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gexlfurrk.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gukxfwdrh.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gstwozezx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gaqzqwrxl.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gladjxkig.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/ggpjmmjsg.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gyaxlchvg.sHtML


<!-- 参考信息 -->