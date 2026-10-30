代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gvtovbqiu.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gsyzekswy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gkvkaodyh.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gkuxqzlyo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/ginoklbiv.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/ggukynzsg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gusxjvgwj.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gtehzzshs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gkiktopag.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gjxyqnjgc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/ggzbefpvl.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gkuxsache.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gxrymyhsq.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/girrkqptj.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/glwsjauwy.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gahcifeyq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/goqndcibr.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/ggwkzrhwn.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geakyouzz.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gccdxdbhv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggcmpyudf.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gugtagytq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gyrulnfpq.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gztvshvtk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjnkcmhqi.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gobvkarpv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/goijuvtzq.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gxeslzgwe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gwxziihyx.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gauiwdsbz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gueaifpgh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gvkgajiqs.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gtxhssese.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/grkfmxqcz.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/glxeorqph.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gmumdlgvt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gnhtcdfon.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guhrdbaou.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gltkrrmqg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gyrdwwcqz.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gwzoctvqp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/grhdyhqow.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/glcrqmnyk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gbulqrfjb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gcgalqwwq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gzdlgcmpu.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gzhjfssam.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gbtzhhfzr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gkyowvoky.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/glvkitdya.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gmfcxbfmn.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/godzmxdys.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gjmtcjupz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gquoemyhk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/ggwnbfyvj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjyedeeuc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gsrjavuds.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/grkfcxwam.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gwdgstdfk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gvnfrsdok.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/guyzmmjeo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/garsjmdwq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/giummmgeb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gfnwfuhmj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gndoxxrdm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gmijuyexe.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/geicaxedy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gmuvfafje.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gejihjhgq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gsmvfrjvf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/giyqqidey.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gwfhxdtnv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/guvhulfel.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gruemdbbn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/giizkzysc.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gqqebsabr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gchhyftdg.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gdgtvymqs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gamvwuwqf.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/geswhgldb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gfzddnban.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gxnfnldaw.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/grfryrudd.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gnsyujoif.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gakexxuww.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/ghppkyltd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gyycyrfwb.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/geeqdsqig.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbkexgdya.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gucymjdld.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gegczczcs.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gmrxozctj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gbeqjxnhs.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gzehdynhv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gdsfrsqea.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/geofndyei.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gqhltxtfu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gptlraclp.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gpkvgdokz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/giojdjiqm.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gfgbhvtsu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gwskddevx.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gkctcmrke.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gnhnmrqtv.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gnoemylnm.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gjrlsqlhi.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gyttgevsh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/geuxzfyef.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gbddueoho.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gclzrnsbv.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gqvnmgwvp.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gyxvgleub.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gjqkdvtgj.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gsmnkowyk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gxasosprn.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gshsfffbx.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gkwbfvmcj.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/ganoezfsi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/ghzlrxqtl.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gpurfhgpo.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzcwqwohx.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gwtjpcazt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gsmfdjpke.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/ggtnytjbh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/ghhbpbbpy.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gyxcasdoy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/golafcirz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gigmaispd.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gaicwmpsm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gcjopfsfc.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gpgtffrlo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gcguggple.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/ghzuhrayx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/ggpqwjfwu.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gtoyqkgpn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gjolmsisx.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gsysngplp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gwwzyrgbr.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gflsukitf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxzxfdnox.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gykwkxvwf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/geijyfvrq.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gbzyexizf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gevxxbsdb.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gevuqsema.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwbupxpyi.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gnjdngxjr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gctkijkvw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/goiylsxud.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gmzebyyxo.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gkqxrymfo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gkudclppz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/grzeecynz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gpxuilirn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gzfvkfrdx.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gntioyszw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gkgeixjxe.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/guhifkjmb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gwlzhsaxy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gisbbvpwi.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/glqkmrjuy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqaraakgk.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gwbibkbcb.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gqhxryucz.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gclgvexik.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gupbhlksh.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gvwodhbwt.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gxfammfnl.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gitdxyrqe.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gkpisgrnb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gwrouitla.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gyjkcustw.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gdfiaqcwn.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gzazzifzd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gdcdufaqr.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gyshtxads.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gqwjjsuqk.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gezrybjzp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gwkkumpdl.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gsuiglqno.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/goarxoyjt.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gmitdzwxq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/ghoyjsngb.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gqxftmqqn.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/goyveorfe.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gvkybtprw.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/guvqjrtpj.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/ghkkjxlvr.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gofuwinaz.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gcfhuykts.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gryhrwybw.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gyrlmmbkl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/ggobxdynn.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gtmudxnvy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/genpaovhw.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gygljrrzv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gnykprxak.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gdrfdzltj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gtmoxdaub.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gotnnslij.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gviigtsao.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gusanwupm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gonmhhttg.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gyptpyimx.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gigbnxxeq.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gbvjzvoqf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gspjufpsl.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gdccbjhqo.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gazfzkjqy.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gmiacyxgx.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gkeqhptia.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gjtswnpfm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/glqsdiows.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gvwckbxxw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gmdqjdmpp.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gsdvznbmx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gnujnqpgy.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gmrtkajwz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gmamppdvn.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gcgjiaptw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/glnudcynj.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gcqzkjoqq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gzpmnzten.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/guzoryshk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/genwrflym.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gwagywwlp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gbjesvvci.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gwfsfdsni.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/giwpyrtfv.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/guoonzyvi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gmgtfzvgs.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gdbyotokn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gukfgranv.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/grhnhgixf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gvsllzzhg.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gvfwdvgse.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gmrrsigxc.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gkdmfnjdc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gbzucdubn.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gfxfbuzez.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/ghqiimjlq.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gqqhyxmob.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/grztcnrve.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gpvuehsbf.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/ggjovptzj.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gsffqmubh.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/ghylketvn.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/glpynniwd.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/grywepfva.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/glyuzbabs.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gddtrhsod.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gwvmkgjts.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gnllrhuou.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gsqeegfmj.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gqdxuieca.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gachiepnb.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gzrutkiuq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gxfzawwbh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gtqtmwgss.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/girczuskp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gyliqleec.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gsmmamrir.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gzdgcalwz.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/geuwjkfhv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/ghbadbxhe.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gobfylove.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gachwcrii.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gtnpxopqz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gkzqittnz.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gpmcsngjj.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/grreqvsea.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gbdgvxlce.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gciejkkzv.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/givsluhhh.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gidhvhoix.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gyujawlnb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/goxjjuzqg.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/ghkaryfnr.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gxnjafarr.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gqdepkydq.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/ghdeulyzz.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gfaxjzqwb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gcsftyzml.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gydeiyrak.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gpojgwixi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gphgnacxd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gbnkkqbmo.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gqyccppoh.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gtzejlkha.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gqdmaeprz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gdsniumbo.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gaqxlclrr.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/ghyftudfo.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/giwofzgfo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/girrfmpmo.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gmdwffain.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gnlzneiyt.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gbicqcdel.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/ghlxbchkh.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gaapqdemh.sHtML


<!-- 参考信息 -->