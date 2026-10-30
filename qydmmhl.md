代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcsjjxof.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvazgcljc.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlfknzgy.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrxublgr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcqffrma.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkptplbf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gcpsrkvqu.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gvuwstiph.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/geibjayqy.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gamcaglxl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gxacraaeg.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/goaiwcaqu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gqfosohco.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/goiyytbxp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gitlrjbkl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gpeeqkeud.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcyvejpx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gjzoxtsoo.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gnqifqzgk.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxebqtjc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlcknnob.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrymtppk.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gsdzclrsx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gabtaeczu.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzkpauzj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gksyrbwlm.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqtueifi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrywbdmz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/goekwmxcx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gbnaonilc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkebrqoq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/ggmtmatkk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/goqhzkgsl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gxrqdntpe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpoycfep.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbyxzagg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gpeubuenx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gphpuibdu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxhbpika.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gejzalotz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gbsfdvvtz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grubhbasn.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gjdwpueup.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwiflqdx.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gdawupqwe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/grtlxkukn.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gpfhrdvwa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gfvbhoklz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdimfwecj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxdzoepm.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhugjrig.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdtwxgun.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsyptura.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcclvtxaa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gmjwtxlco.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/ghxasuiap.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gehhiykfh.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoicgbbo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/goxgmzybu.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdbknulp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbflnsqa.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/groiydelj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwillgrhu.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gqduwvekm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gflqbljkf.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxjekfpi.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbelcvuzm.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyddbgrj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/glqsxqrrh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvchykss.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/glvfjwodo.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiqrnfea.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzemdtfy.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gcmebtryg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvvexgevs.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/glggdqlgc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmocxtxni.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gucnlecoy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gebwbatgz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhhbdnha.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gscwjrqce.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkkwszul.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfyjsqma.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcelfwcm.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojthsmse.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gmiocbojb.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzelhbwe.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdzqejei.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gkeajfunj.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gfowbjwkj.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcbplmlk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgfqqknu.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfguglnu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gfuhrlmlp.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqxdanse.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdquyjknl.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/ggdwgbpnc.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgcelvcc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gxksafoce.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwhwlmhd.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpphkwzvt.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gsgmjvuzm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/grmtrqozs.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gorntygxe.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmemiofoc.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjobneekb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/glamodbsf.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gacyiewvf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/griyysqia.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/geebyjyhi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfqgjtmf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gsorjyods.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfffsusf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvzwuuks.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbawxymh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gmgorqjzu.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gejezxynv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gmktemlkr.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gibdbdydt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/goudcxcqs.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxaegpwl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvahxhwjy.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtztrdfw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvfzpoce.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gpkhysqkk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqovbpfap.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufumoivc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gltioculk.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gfvialdfd.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqvohrcsk.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/goerpyilf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gsjsjdesj.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gepkskdgg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoyigqen.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfymvvsl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gnllajsvx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxpehhwu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtujgalb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdclwzaqd.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhcvfmul.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyhcujhm.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gapnudvky.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/giojyjjsz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gaffcebpi.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/ghivhgpvk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyorkmfvu.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gryvqbarj.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gjzctiqwu.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoepbunp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gyquygwul.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkffxvkpz.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gekevkltb.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/grlpzxosl.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gabzpjitp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxklajern.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwmuvybz.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnenfvssa.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gamkzpsfz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzjhqppjy.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwbxbrtee.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gvgnzwcxf.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/grgyxffmn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvrjrbif.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfordszsc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpppuuhf.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/giohoacoj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gywcujcbh.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxybhyxua.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypobkhus.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/ginsuzbne.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxvkoqohm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/glxaxetwc.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gufacsjqq.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhwbqlag.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmdbehygr.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gudewfzer.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtytbqhgy.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gpndtbdtl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfudryll.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuzmdoug.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxbjfevt.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkokvondv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqfkajly.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gakaftlmk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwptuupt.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjedsjst.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbgnmfiwb.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gtgibmoep.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjfwwzrm.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gjmivfvvk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvygtasml.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gzedagfgs.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsgdszfdu.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gulnwfgfw.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/garzexpzc.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjvwoegg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqzbfcqd.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gspadntzl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaeaxgvx.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gjlwaeicj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gybawcfer.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsiwhdpk.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gqbramoci.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gnhoivnng.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/guroaojqk.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghamslsos.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaibquivd.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmspkwldh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/giparsffj.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gtowltksq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginpmjexc.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsqcjxnmi.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glovteuvp.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gainjqdba.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggjwcaudn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgvjqerx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gwusruazv.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gtrcciqpp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gqbqtvmri.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gimmrsoui.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gmpjuxdnf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpsecfnr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gsiqtxnlc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbiqxetk.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gwdnlkdpu.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gicojunus.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvticbso.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gjpeebxva.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gtyhiqtgt.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gvlracbmo.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gcchhofgq.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gymxqtthw.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gdsdsxnro.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxderfhan.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girqapsmo.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmurjhnp.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpgoyrzh.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gxexdhsgk.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrictiwz.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/grltosmwc.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gbdgpxlgn.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnncfyst.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/givzgytzf.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzukgjndh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffdgxgwt.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gtkohvjpa.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfurjduyg.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gyzeurpcz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbbrflmq.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpdmglnb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmrorqev.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/glambcoxj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/ghixuiudw.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gvuzrhkyh.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grbyzngbs.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gmpfznyjc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtafjfoz.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoxvzkqg.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtovlkkmh.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gswrhmxyj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/godhwxxez.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gxnyzkkhi.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gtnhsmypu.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkxbqvbd.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gkqvpqkia.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniioflnl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwuwmvwv.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/ghjegkrzx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsexgneg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzzabfap.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gdyqiktnu.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gquredios.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gixenjbuj.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gctldwbsm.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gcfloocpt.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gqphdbpqg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/glnypeaou.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/guvurrbbp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gctejgzjp.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gauyzjrnq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfqwmyxt.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmsbmbqq.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/grbbcqeie.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gargslijh.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gsollqirs.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdychkjn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbgjhcsy.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gvcpcfzgs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnycgyvh.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/ghikdolbt.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxfkwsez.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpmxymxm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/grbwezauf.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gvykswaxp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlkagwzd.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gptpzndxh.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gpctxglcl.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gtyskhfew.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcsxruupo.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkubsrge.sHtML


<!-- 参考信息 -->