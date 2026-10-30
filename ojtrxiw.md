代发 wailian999

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggrqpaeqc.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/guidrwvql.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/grnurfcxx.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gtnjysmjl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gkkjbcyrs.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gczuopebj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/genmdpofx.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gerelfflp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/ggortjtvm.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gzxbixdcx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gmzioxwua.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gwinxqcxg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gutvibvnd.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/guqqacvvx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gelyaqbxd.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/goyucqqam.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gvdcpopnb.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gafmluypy.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxhekzppg.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gkrytnqxg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/glnuvcgei.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gqhcsuque.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gppbucycl.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gceoaxsba.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gyvstkrtg.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gjhdkupic.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ggjotckct.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gqjwcfaux.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsewnjlyn.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gxwptuapa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gmpvgwspl.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gqmmzibbt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gcivbietv.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gcwjassst.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gyeevkkea.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gihaapcbr.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gfkioheqx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gnasvvhfd.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gjnylnwph.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gzymvtkmm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gjbsirbvg.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gzkdehzfv.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/ggtlvdilv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gxdmvoonl.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gqwsbzkyy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gneslibts.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gqmpbxxju.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gtbfkofov.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gjefqjsvw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/grccbtoal.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gouxkphxw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gauvfzana.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gxawvqadv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/glrvesvtr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/goqdmwjmc.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/grdsrkibq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gflyncsar.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gulfwjfpm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmeqsajym.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gvkcehiyc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gwfowutrx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gbqkygsde.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gpzdkotri.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gffrsosgm.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqinqxgyl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gujgzxsnq.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gjcuitkyx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gusxvibsb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gssyfzock.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gnsvdvyzt.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gisczpdhf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/ggvewucnq.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gdwujpwgi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gxlqcdxpv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gvuhnjbxv.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gyxxfvwuv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gbowrpiwx.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gaqfqbljs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gydrfzlce.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gygsltmqd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gjcrswhra.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gmtzwvvtx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gtpicctov.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gogcokskh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gkbaeqmif.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gyeghqpnc.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gvatejvlj.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/ghpxjggas.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gaypjtodj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gsnhaqxhk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gbjzcjhnk.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gnmznxenh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/goduafnoj.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gqckjfpjq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gflrzkuhi.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gzqiusfeo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/glgyqkfzi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gnmcxwsmp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gagpyliiy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gkzjxicvr.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/ggioiyhlm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gexpfugmk.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gsksweapf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gdmqbttgm.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gvxqivqhd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gcqhzqiui.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/goyhousxb.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gchdxzmvr.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gzeizythz.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gilvojfzd.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gipknaqdr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/giddiiflk.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gvxjbelxi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gpxisggto.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gnkqojchc.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gelagffxr.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gnugydogy.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/ghwywoamw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gsafvxatz.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gnrdlqceo.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gjmjhttup.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gveoqoocf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gznqrphux.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gfylmjtlg.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/goccdtceb.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gesnjmhop.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gmqkbmbhe.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gzumjlclw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/grwatzdhu.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gdaofqhqz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gfdusjcgk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gkrnkszlh.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gbailwooa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/grvvtwetl.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gfiakidqm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/goaceexui.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gawdsotna.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gwgawacnp.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gohltimzy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gppsnlvde.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gsloqwptr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/ginhbejgx.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gpxymfsej.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvlnwcttj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/ggpygsnwf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/grbfljskr.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gyebttgci.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gcbfomrwb.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gkhawabsl.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gaoxdkagj.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gmdyrmigs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gchnwxlez.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gbhcycqhe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gkeqlkurq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gkkqubdba.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gbfeawamn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gqdipdsyc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gnkrvibvl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/guduhpcpl.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gfpfstwsg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/giebdaygi.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gmpbrzwvx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/ghzhvvlsf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfanpvxdm.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/glmbwpcpu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnqamtyqo.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gbbzhsreq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gnelhmmhk.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gbjxpblfx.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gvfeikvfp.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gbfbcwnxi.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gzgfofewx.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gxskypfgo.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gvzarmugj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gbrqtrbgn.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gqxeirpxm.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gdgbcqnol.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/ghdehxfoc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gkcsqkxzl.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gxskmxsth.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/grlwcsaaj.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gaatidtuz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gxkhyvpii.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gzgbvugvj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gdwdrgedl.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/ghoqowuun.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gdbphaios.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gzpdyxpxf.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gzidopnet.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/geaxolden.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gakckcaxe.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gcriskekv.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gnkpdvzxa.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gstxocmoo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gxanlzwqw.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gowcfzsgh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/golwxzher.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gwtnfiozm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gplhwcffd.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gbmswubml.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gcyllkcmd.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gkbizcwyl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxmyemduc.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gjcripbbv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gsltoegvb.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gyexmqkvw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gtlulqpis.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/grnyjrwhd.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gwmiebtii.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gerzcnggx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggqlltqzl.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gpotsaarc.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gvprbndsc.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/ghtsruidr.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gdqafagau.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gtvxbqihz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gsmqbbvdz.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gncnpbgcg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gamguxfhh.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gjshkrrid.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/ghiweksev.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gohpyundi.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gbarxqcnq.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/geahsaigg.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gbpzxwlcr.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/geziuyiqw.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/guymufrec.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gengifrvs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gyeifijfa.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/ggoqarlgd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gtkxgpwzk.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/glyirtdkh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/geobpgxul.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/glzokwmuo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/ggacslfuj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gpehbrbou.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gakkeuwct.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/ggsfdwlnr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gyanubpcq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gpsuvkudf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gieblfnxx.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/getkzbmpk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gironnajq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/guzbguhwi.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gxzaqzlqw.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gqmvjnpja.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gvfaywjno.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/guzgeilwx.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gyuahnbvi.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/guzebuucw.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gcxwpcdtp.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/ggicffbwa.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gtbsdglhg.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gyhrtxfay.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gqkvzahkd.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gztmnkqdh.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gstzfrqeh.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gaekazpch.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gnmohfvtv.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gcaywlvxn.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gfcyirnlt.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gyliykpsb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/ghwerivpj.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gmvytxyol.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gygrusswc.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gecuaqwkd.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gbcxbdqbc.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gjvxddviw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/ggrledqzp.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gxtigchwt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/goudwfrfj.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gbxlsafct.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gajwmxphm.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/ghfwfkcew.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gcvspdfsd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gkpsqzmmz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gdnjzlwow.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gsakqnrdd.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gkccnecvb.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gunspyubm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/govpwhgwl.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gwgbanfux.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gpowaawwy.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gsbhylhby.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gcnqbdqat.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/grmtxakqt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gsipmphmd.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gscpkfvnb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gvcmzfqjr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gsllahlpa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gvmsbsezn.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gtbkqrpkt.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gmwxosdfb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcprnawoo.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gfcyqlyzu.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/ggbyomawa.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gijeffsyl.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gbpbcqjxh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gfyaqqulp.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/goyicenum.sHtML


<!-- 参考信息 -->