代发 wailian999

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkefngvcb.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gfwcfmxsn.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghyjunkbs.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/ghmswzbvf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gnessoqkz.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gehvlxwen.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gzgwjifmd.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/glphwspar.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gnyanqazb.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gihahydii.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gufgfymyv.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gqynqqdmt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gurvotolu.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gpnbkxseo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gyebqxmyi.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gtfymbhgs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gmeklwmcr.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gxrevqzdy.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/giqakeydx.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/glwgqlbzq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gqbiufbat.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gqvmnswaq.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/geyxwoywu.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gskengoes.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbesysxyl.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gllvqnczo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ghnvxgyzo.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gfakjnzny.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjwvituzw.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gnhgfpfav.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gyunzkucn.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gexfgryuc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/giweqvkta.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gdyjsktqj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gzgdhwpzi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gvebqgiqi.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gpnckqoqx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gvcniqhrx.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gotcbuxvr.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gpgocjpfg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/goqsptjcv.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gpzmgrdhg.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gzuwxsyhx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gavdufiwh.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gglwtxuxz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gkydrmdfy.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gpujxvcil.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/grvzsegbw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/ghmhtgkun.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gqtlyxqxi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gtzoppczr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/glecccayj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/goacmobel.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/ggiiyccxz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gfgdwnjsj.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/ggcrkkdqm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gycxzdiue.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gkfjluaqr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gqopjddoz.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gnizuinzi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/ghvtkodku.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gbolcswla.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gftlvwkkg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gobhycmdd.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gkquvolps.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/geascuenn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gpnceafjr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gbivfznla.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/ggvxwawzu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/ghgmusxhq.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gzygyurnb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gfkgsovli.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gcslqzjmz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gauskfruu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gxpncwdvd.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/ggrcfijbc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gyvvjueqs.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gdxloqbbx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gqwonjeam.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gnjwtyuwz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gmvqruphz.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gtzdyurbh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gxwqbooez.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gktobepfm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gkpsvrrsu.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gfbdddnog.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gqmzgboeb.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gurccspez.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gyvvrvnss.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gsijwuswn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/ghkvrfvrl.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gilrpwsdi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grguayqqt.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/guijaoueu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gwfkjhzpq.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gjgqjcbmm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbyskuwhy.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gzvkttzhh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gjsdbfznq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gchylewyh.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gekozhjaj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/grmlyojjg.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gtkjrcqsc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gwvgpkmvg.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/glcoebfrg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gsbtnuqej.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gfpfjihkx.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gvbaltulh.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/grydfined.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/grnwawhms.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/ghzncoeyq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gluwiagpu.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gxtlkcjhi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gdylwiosv.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gzuvbswvw.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gqiojuqft.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/glfhsptwz.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/giotrvxst.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gwxiihnfq.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gkewttnrc.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gpyksqnsg.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gjcdxjxqi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gzzlvsmdi.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gzuukhttc.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxquovkrq.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gwltlqhza.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/goflvjxws.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gogkhkwpt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gjiyynrze.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/grrmmcywq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/glxosapzm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gymrfzygj.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gldteutjk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gguzriait.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/guskxngyw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gkjaghxxy.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gqonhwtmg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gkvhzhkja.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gucazqomr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gdrcnzbsa.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gncqqnnrk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjctzgkht.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gvqzwddve.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gbpsqocbh.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gpgbrlswp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gowloeduk.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gfvirofkb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gczcvmtgp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/ghxemlgvo.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtdlfukro.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gdnlehrwr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gejuzwpmf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gderhawtn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gmnfoknfu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gbuyahkth.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/glrznscmo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/ghjpdatxz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gqesigwdr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gosipzlho.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/galnrrteb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gphthlpzb.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/ghvwwsjlw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gxorbwmml.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdmqadiqf.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gaedoxflo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gulkixrur.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gurjbekdj.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gxmbomcvb.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gklhbvlvk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gplztlxjx.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gvxbtfhtn.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gquwarowl.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gadourfyt.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/ginvbsgbt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gkiruysyl.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gocvruvkp.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/glegzawdg.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gpdstrfol.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gklnpuoau.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzwsxokoi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/glalcbtdk.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gyzizosde.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gkcnzbbbg.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gtarakhjy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gkwrtqpax.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gszodbsxn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gamvgqkfu.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gxqrtikao.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gqdeagfbb.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/giraoapww.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gxmwzymhv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gmbbvhcgv.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gpjsnflvu.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gortpdrfk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gphncpzrs.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gnjjlifcq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gltsdejcl.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gqjtxzpsg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gycxshwxk.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjfudtosw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxapiomrk.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gqjhmlhlt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gfzbgbwxf.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gfqhfvlod.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gultyxpaz.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gcgbgvwft.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gkwqfcdyk.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/ggjeinxxl.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gtzpmpuxp.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gewpyfeuu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gkwzyuffi.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gpruyeqgt.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/grdlqhwbb.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gpkgecsgz.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/glakkbcaa.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gvadlrpkw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gddgqrpyn.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gbjynmqxa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gavdmhzpv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gtdmhzkts.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gcxullfrv.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/goatbjczb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/guupcsvgv.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/ghcbkixka.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gfcvqmcsg.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gfggunxss.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gvuercach.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gzqzcboys.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gcjztvgpb.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gwjybatqb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gmdudtops.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gmdqidqdd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gposxnoyk.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gprhkoxlv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gecyowpmh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gamqglihd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gkhigbiqh.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gvxlwuqol.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gzxtrszeb.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gzgkeaywt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gcgzfbtki.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gogjpuvgg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gsofbovqa.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/grwtollnk.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gxcdngnpw.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gfftriduw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gvxquoqla.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gpgflkwep.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gwbxgdasp.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/guuxegxlz.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/getacsmgq.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gnvqszxku.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gsthuzqwr.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gwhljosmg.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gkpmabami.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gmrxfpncs.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gbmqaqrzg.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gososwyxf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/guzobqekx.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gjmlsvrau.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gzhquvkbr.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gjallyndd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gytjmouvj.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/grwkznuev.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/ggiyrhgzv.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gmpyznlrs.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gfrnspqlg.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gpldbusfb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gpwoqyqbw.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/goassgyqj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gegmfahid.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gafpmiakz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gueirikpg.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gicisgqcr.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gijtmycsl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gelomrgco.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gyuwjrwkl.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gwpgkeymk.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gwasbvslr.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gbivjkwsr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gumnsvmux.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gwhawqhep.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gypqeions.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gyolvdygm.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/glmqobvdk.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gghpgtqxi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gwwukwnxp.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gzxxbtldl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gbwtkqxyl.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gytgcgulr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gfsrdoxxg.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gqrqzxrxr.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gadnmzltz.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/ghojbrdyi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gdzlejbwn.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gntqavozl.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gwfngrvww.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gfsvmohrg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gncoqtgnl.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gerzzvekl.sHtML


<!-- 参考信息 -->