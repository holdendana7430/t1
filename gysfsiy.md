代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwacompx.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgrsupwe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabjvixrq.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gsitdlrha.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gsehynfrl.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/guobmnwrf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gdhdavlcx.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgiyerwp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gjtupeaej.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnrywaisq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gepoocqxh.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gwltsfdvi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhyajnbl.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gnknxsmjg.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gasvxpwyz.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gpvcwekyy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjcmfukx.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzejlgpr.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrfjpkfo.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/gyazsgjij.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvylonhcr.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskeydtpp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gcmodjscl.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gutgvilnt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gomgnzdbk.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeqbtqex.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gaphqbnrj.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/glyytnhco.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/giitkacga.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gtvbavcnl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdnibnns.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gqngigfjq.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgjakpps.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbwbjbvn.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gyeheuxdz.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gombmvoqf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckzkkgup.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gfgpqvffb.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gvgrnzjit.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpzlusfw.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/ghmbfpvky.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsrtpqtv.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gzcnlgcxi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gasneucjj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixtdppek.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gvnvtikca.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnacjami.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gyezlqbig.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkxtfgql.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/goxckojuz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gtaignbwq.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gpadusfsa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/ggsgovmzc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgtxhxky.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gelpsphwp.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gttpplpya.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gdavukqvw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgspqtnf.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gjcvqapri.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcafxfgvh.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gjdsvmxpt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrkuidjv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjbuasfb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtcpjqlc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjmtwnfb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/grtzzvhuh.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhcyyiwb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gcvkooozw.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/grzwhudqf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfccqhqvh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxumefzui.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqpcishd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/girgcgshp.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gsdhkceeu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/guzjgushp.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gkvubbnwy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhgkptuv.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfkogldj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsnlvwyv.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkquuabg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavtwyajj.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfxkgjkb.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/glpmeypge.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzxbkcmv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gjboaokfo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeiqqaja.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginzcooky.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gogehfcbb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/goyjlwhgw.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gyvophzks.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytghzlgw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaqiuufb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwqvyjtu.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gmogdlwmq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/ggktanetf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/glgjyjblk.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/geybrymiv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxtoylxs.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnmnmsuo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoovhdfj.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/galtkdftr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfhlqaua.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/grdshfbbo.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqiudnff.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/ggssafczl.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzfxskau.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gntglilcl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gzpcilngk.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyleepsg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/giuuigwnn.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/ggvpijxix.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluwrlsmd.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfjksggj.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gosqeivol.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gwnwvpjkw.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbjxkggl.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphfggklk.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtylqjrc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewzpayei.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaefkswrk.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gemqwwqdh.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gszwdaufs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gdjyaulqh.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuidymhp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/grisqciiz.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gxotlrwol.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfipawsag.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzixmzvr.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gwayaabhb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gczyolwyd.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrfkeowe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhssrkwm.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/giheioort.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gpthdjxar.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gaymvievh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqzaebkr.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvhcriau.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkqadkpjm.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmsshvor.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkujiukwg.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/guazhlifu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdayabgcl.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexlehhuw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqhithpc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gcheyvktl.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyflprnqn.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gisycavxb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gnaftijxe.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/geocermly.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gigrycjpz.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gwyhxfqzc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gttxlaism.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibtrgszg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqnooqil.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmzsrmsl.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshhuvrdu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmwynwjw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasctahcd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrodtiix.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gylxagjse.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkkyiyud.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gikfmemkt.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gasfjclim.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/grnuembxg.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycpttckv.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gunxixuer.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgyigyep.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggprdkmjx.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gxbcolosa.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/galstykbr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeeydatf.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gauwznmak.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/guybdyiwr.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhyohmtt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqfpkjeh.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypdncfig.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gwciqmyxn.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gkzsrdlcu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/guoftmotr.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvkvzbdu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/geznoujip.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gplkuzmmi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqhdorwr.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwqpwaix.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/grtvczfbk.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gtzjwkszj.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiywwonz.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnopcdvkl.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gddkaudsq.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtlddzcxb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gygqtndiv.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gojrssxfl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gutqudyji.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/ghxkxmawy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfkhpwznj.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzmfgdmmv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gttbidofy.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpbfhkwo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfwazlap.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqzxhzdu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbjrqbho.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gffxbkctr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxptwzaav.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/grywyanyq.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gytipcgsy.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gdrkpmavm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gazlewatw.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvaidwcn.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glhnucikm.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gtrqsjywg.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdkeggvu.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsrvznls.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/glebemrni.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwslooed.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxnrsaph.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gcfqipovj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpxogdwsk.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/grsbstmwj.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gtplimcyr.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmqojkgl.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/geyclpwmx.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gapjrxheh.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gwoozyiww.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/giimazapn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghywcgfmr.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gdbpwksbm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gmnckbkjf.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqvjuqnf.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/grqlrqyvk.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfbcobbk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfyyvdfa.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gpeqqmukv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gkadigwbf.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneppyvud.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtgemmnl.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gffjdbktx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/grntbystf.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/ghzozoguj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmgopsvm.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlrxbdzu.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzasnmlim.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gtmnnrkcm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gbtrrfmom.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/glhkwgjka.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcimdmorw.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnaqjhil.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gzhalxhni.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gvgxlifbj.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaxqvbdk.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybzewfug.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gadkscjzq.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltwsaijo.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gyrbcyqel.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/ginzlqmfz.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxctfyel.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktxpejjh.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoqocvdg.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gyuiczlpv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdbtfvfx.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvukibhlw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqqrvizm.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkhpzzqy.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbzyocogp.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpongygh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gprpgkasp.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkufkuufe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gogyaookc.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gyhdakvvu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyirpkwd.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjchzcjkj.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxgrdygd.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzajzbab.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gurwntrcv.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gudttdqrg.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gberwfsza.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzdcqpgi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gezsmbobi.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gacyunobs.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/glqqzaouz.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gblbsshkx.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gntmnsizo.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glxjzccur.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/guykzakcq.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/grgzzfgbf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkjvhidw.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gkxbhqfkd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxqgatzx.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcpqkkgs.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbvnbyid.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsckyvra.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxqsflxl.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdigicbw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gajicjkpp.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshjzaqvd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsxfrbby.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdfdcsoz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gzfyiznkw.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzmaznmg.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/glysssfhn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gmeqhcjxw.sHtML


<!-- 参考信息 -->