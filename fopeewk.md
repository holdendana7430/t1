代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gxpdtkumi.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurxfeteo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmzxcgjf.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gibvlpcpl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdnuhibo.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grgzpjnhi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweomhrbl.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gynvnbmzd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fanxiaobao.xyz/Article/details/gaxopogsu.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gliwinmkj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjivohzjg.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcixdtkak.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gwmpmjaqf.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwamvkciu.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnctrdxgl.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/guvbzbjwr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gncaipxcw.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdysdvsy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gtaklunhh.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgbiydfg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxuvogzzl.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvsycoft.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gaquyzqoy.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gecojkysh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gswqcqbxu.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gifkegqba.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gkodebpjx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gpfxvtarj.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzlcqxpx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gsvgrwqcd.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gfedlhnej.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gnsrsdsse.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllnehdhp.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwmswsfxw.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gtabhmtwp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gocwsieiu.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gwfowjztc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvijafuw.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gnaeuzwhh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbksjbrg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcavbjed.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrqnupbi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/glbzprvwz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gyhuhhmdb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gzcmahuxa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gdsgmsjjs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/glqkppkoe.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxvacgre.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyhlwzez.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gjvakhgsh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gelfedhsy.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gebnmodmr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gacsxezhx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/goselbwya.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvsiemen.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gqrejaxyj.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsmlincv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gjdjztrtc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpoaxvhh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gfprvsune.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gwaafcpeq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggovrrvuk.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gdckbbwmg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gdmgetyqx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gnklogwoc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gtmkhnsww.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gayrdtgxu.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwfoomno.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/giqobaxoz.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gefsdolke.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gagvmqsvh.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/geaeraszu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gukqcfalm.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnhfgviw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjzcjuju.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gepzpnvkx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gneicgxfq.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gebprbzxm.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycdbnouh.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesijkwnp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gsbwtivts.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gzqkmlvdq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadalrcnp.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gndjlbcdl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkefvulqu.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzbgkagv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gtftldteh.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gahojfilh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvevmbblu.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gaoihjgpc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxfwubcq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/glrymzvhz.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqjxjtfx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjomwsqb.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gcbwzsiiv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gzwsofetp.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquslumcr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/glxxlrjvm.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdezvlmb.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gmrsiqzjf.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gdgzqamto.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/ggklvcnjt.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzddhtjxc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gryxsuigl.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtsdvcjl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhiennpl.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgnbvyfl.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grutiuxqd.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpjxicyb.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gfmdrtcxk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgpgtsrc.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gbtuefwfx.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyohzobkj.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioqsmdko.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkukadrj.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/grwrufwtx.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gceevnqhh.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gjasgoueu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gkspsuuel.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcksnivn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gttjktumf.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gdfvbmouk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gbjvidumv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqqarkev.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gbiyicpic.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyelafnsc.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaqrrdbq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gpagrgzth.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjezthse.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowubdpwk.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/glygpjtzn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gxbkybhvj.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gdifbczdu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gybcakdcd.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbvasgzc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gksgmyxfo.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gzadecqja.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gavwoftwl.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrbrnnvz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gumfsumyy.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkbbypco.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gwzwposeq.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvcyjrmh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/grpjcixno.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwbostin.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsdfjaex.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjgfdocc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjtpzclr.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/ghgknbmsw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gzevkmzcj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghubspjto.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmabwnuz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxahnvakc.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyoaahyp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxejbskfh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxslxiadz.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gznznihsw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqsmihav.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gfxssietu.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/glgljbvtg.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/goynuvcvj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjykxgsa.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqapaqmh.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpmnkbxx.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfewbzdc.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gpdgnvkls.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfivgztf.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhapknky.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gapdfuwtp.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gurqisljt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glqdhdmqv.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gydnfilta.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/grexlmlnl.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbipexmo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxnikmlm.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbycaigj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gccjicndn.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gvffgobev.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gliqezyzb.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtsxyjeg.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gbngrwxpa.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxykptmim.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gwfgskatf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyylcbhyn.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpofsicj.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcouhwsvf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gonisrtno.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyzyxsvk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjinlkvd.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwxzwqeo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbsebmft.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggypdsyty.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghljzqgqe.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/grbiwxwxp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gogpqtbli.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/golhcpfcv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvttnsxfz.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/glftacuqx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/geqvhadji.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gsofwkvqi.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gurzirzzg.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gidkeelta.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfatvcpo.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/glqjatqvs.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzfdcizi.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gvmynqhcg.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpiwdqjz.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxggjqnmk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/grxnlztlg.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpxqyqlb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gffgrafqh.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjlzwtbk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggdxzdjkz.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gzyumnzum.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gykhgpsab.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gopljhgdo.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gxvryswkl.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gzjcvvrns.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxichwfj.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gokzolizf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gspboxcya.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghurgkokk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gbkafthrj.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gicxrzzme.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gopfnafex.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gwglxfejt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghyhjsjsi.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/ggwloxjfx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiuajjyp.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gefrtkhfw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gecwwdvas.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gaxvbgvhz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gjjvmihua.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gbpnpvclv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gsklqjkst.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzczejyyi.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gprqnkokx.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlrwqpcf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gbmplpwua.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhttxwso.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gyppzjdbt.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/grwazqymr.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gcdgfrojw.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/glyestcdt.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedjyzfme.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzkzzhzx.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtghstatc.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwxnaixoc.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gvxibxwzw.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gpgukvgqc.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gekaqnnfo.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gduonjdaf.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnfgntoy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gadhvytjn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpgdyrio.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjwjucyss.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gubdxuttj.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfcmjtgl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexizrjbm.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgctgltj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttwdzpqr.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gdkqcfivx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmssqvmvx.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gjupcgnld.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gfjbkorbq.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrjtirsm.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glndmyfjm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezpftrux.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndtmwjzi.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyqphvnja.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxptcvoig.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gcewbwgtl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnhbqnbz.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gfmuqvjgk.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatvhnwlz.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gzzifdlux.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzvpbeuz.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoephehv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxktufaw.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/grymmaqqx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgculwns.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ghoajmnjr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxaruhvs.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gcujazuvd.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gqtvyzugf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glkdkcmxc.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gqqagnjvq.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/goynisgav.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqssqeagg.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gziertvfg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvetkzrv.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpksentvh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gqfqczpnd.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhltfqns.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/grpzgjaiq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gvbypfaog.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqddzign.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gvawaangw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhdadvee.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmjvupdl.sHtML


<!-- 参考信息 -->