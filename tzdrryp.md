代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gxwkxdfpa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gemaeiyvn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/ggtmejugy.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gmpzpexvj.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqpfvkzyn.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gbmxcytjl.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gtuhfusvc.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gkscdfhzt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gaajcweou.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gnvitxlqh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gvdexnqmt.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gtkiwywts.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gqtjhjpso.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gvfsxtfph.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gnfgrjsih.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/ggwgxpwbg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gxlocthog.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gbtoqepcx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gddqnorec.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gyftfelmg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gymgqpezn.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gmkimzutc.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gzmcjiodg.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gwcyfiljh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gegfcwrdl.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gqcvbxtba.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gfasgafuv.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gqosjkomt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjvlhoxlr.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gxopypbno.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gphrbsczk.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gbyxgagpa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gtuetqakm.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gnvsdndop.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/guyluzqsj.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/grombkctl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gonqclurg.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/govqnpvdu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gbzyylumi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gkeeinyhj.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/grkdhnwqu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gnabsqwzb.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gwlridkbi.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/glrxbtwmv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gibkokthu.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gmodpkgub.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gwfblhyqd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/grnwyzjhg.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gnjdepajr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/globddyqh.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/ggbbsnqhm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gyzjpabhl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gryuisdsx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gwzihpwye.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gscunbbdw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/garzuidzz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gvlyhzgle.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gqgctgyfw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/ggnoxcsck.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/glqvejvce.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gdqluimam.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gnsjvovhr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/grlvrecor.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gpmuombck.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gevxjcazt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/grycrqbzv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gabchnfag.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gbcftbcmd.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gyeektzgk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gvfwlkkpr.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gdwjqmmlm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gyuvmujec.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/goeziljsm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gahtroryr.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gkqqwedxm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gzvlyaous.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gnoqoiwpv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/ggjwfxvuj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gnzgirbsl.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gubaavafm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gnwrawblc.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gumvnuaxg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/ghhvhrcxp.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/glotaklhb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxvrrvsrl.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/glfadyvbi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gewpasvwc.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gvwjwdrwp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gactenpqh.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gxhlxvery.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gffqvnkbt.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gmozbzomp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gmikkowhe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/greqtgazd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/glfiwsmyh.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gexulevip.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/giiexudfc.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gxfkmuqkb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmwdjbmnt.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gskunvbcu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gfwufcwsi.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gpcjrbahf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gtafvwfik.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/grjpwixtg.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gkctalkbw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gsqkzrsmg.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gxgyqjhto.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gpogdtwuh.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gqhumpddf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gvotaolye.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gevcsmaly.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gxzqzpoyu.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gekwfkfum.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gsxzqcuro.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gwjnvqjva.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gekgujzle.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gclvhetlb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gpbyufwjn.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gbomzksed.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gllijxkln.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/ghqfozoas.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gvwwrcpvv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gzuetfnyg.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gqldfauuk.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gabfvakkq.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gyrfyppwz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gghumyjrf.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gtbgbgxdd.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkltwoejk.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gjelxdjmu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gyjhcbnrm.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gylvhaeql.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gzuslsgbq.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gthntrnfb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpvxopemd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gvbosyhmk.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gpnwffykk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/ghziktzxj.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/grsmbkikc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gjqpdngfw.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gntgjxkjg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gyknjfbfx.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gtiveihup.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gsvvhcxvc.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gjqfxqycn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/garedpuud.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gdwupogka.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwpkwpiro.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gnyuhtxxx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkycewrvk.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gnvfnssvl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwtxvboim.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gjniorqjx.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glggopdpq.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gxxokxcie.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gfhrfidaz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gxvijmcue.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gqpiqwxyd.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gnomclnni.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gqpxgengm.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gigzpygca.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gcqcpzrgn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjregerle.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gyzemxarx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gkcmztcbi.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gfztlnbbx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gxoswglnr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdhbdfjqi.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gsoicymyz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyhsrtmec.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/groznzpbo.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gsrmtohtk.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gmmaztyem.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gbhxnthxs.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gmhovgiet.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gbkwplfwl.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gabmnwomq.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gifdqnzlh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gnwmnltbd.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gflvbixyi.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/ggaemudty.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/ghozyvqgs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/glrnbiavm.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gbhnhpqxi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gphtsqorj.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/giwmkuglt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gxwfdlttv.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gvxyclikq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/grolmqthc.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gdvytjcra.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/ggwybozxg.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gnmvefplk.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gsnpahhtg.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gvudvybcy.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gkghlqjbh.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/ggkqnacyy.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/geqhdwxlv.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gwqsmilkt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/groerrngu.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gosidqvsc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gpytbzhub.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gtrduuqua.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gbpyjtapm.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gtsaramxn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gzdgifolf.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/grovsyixs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gpupawapd.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gjilwrvbb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gdmrafwrc.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/ggmegjsft.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gciazypcz.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gezmpuemv.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gniunfawj.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/geecckwwy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/guzqkhnqg.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/goyivfjub.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gaslznqjy.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/guyqwftsu.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gyinufcdr.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gkobzkyky.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gbqzkbqux.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ghymainjj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gnqjifcgx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/grfbctibg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/giqopyrvq.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gjhcccvdr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/glbpuvnlq.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gphwqdblr.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gpbqkkeqv.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gqucpqogw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gdvpzgadp.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gshbfpkhg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gjmicxpnv.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/goyhesbog.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gmrwlcszd.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/glabyrngr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtbzhwwno.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gqapfpqdf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gozkvvyqw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gwgzvebhc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gugugxpeh.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gfzxkiepp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gjgydtdxy.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gbvhqvoni.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gisvtwbfm.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/goeynniao.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gaxsnycdb.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gxgvfdohc.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gjwavveyv.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/ggrwiwwtl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gxmwmihxr.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gntrnapvd.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gtvxuybfe.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gzkbxpscm.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gsnnevvjm.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gmblszkey.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gkekmzkdj.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/ghfxufwqa.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gocbliowv.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gwvkkwldx.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/ghptzsjzq.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/guboiqguy.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gyzezdkze.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gvqsshkah.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gyfgjnbor.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gslftpkac.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gdrllihxi.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gbllhcgen.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gavbxpdfq.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gwuyqkvne.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdgbggzmt.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gfubstnzs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/ghoyaruvv.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gydbqiltg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gdqruuefj.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gfstfcavn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gqnvrzoxe.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/giqgywalq.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gkdyuvtpa.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gsmqipunz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/goaxfinjm.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/glkbvgvvo.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/glhuxvhus.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/glhzekjnd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gpcpwaafh.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/ggsvtnpnf.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gvobyxeut.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gkrqnixfq.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gsswiddck.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gyjtqheog.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gcwsjszvj.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gmephlwtn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gqpptlhqn.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gocdwooqw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/guxhmsvtz.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gsmqthhsk.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gavuzidvv.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gqsxmyuwz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gwfxwkwzb.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gjrnhlaaq.sHtML


<!-- 参考信息 -->