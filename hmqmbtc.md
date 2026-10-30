代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/grpafwzpc.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxxqhbjp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gtyvgzgmr.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gwewmeaeo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaoopoiq.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbltdsve.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gawuegtsl.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeeiriaw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gyuwppnhq.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/ggznnvrwn.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyofecweu.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxgmiymv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkurisdc.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gucfxolko.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gucekvgmi.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gexmokubw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxfvvpxz.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrnyuijy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtuhuaek.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gdxvajyib.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokkiwtky.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnfpemvh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gwuinksro.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gxphcaant.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiufsjse.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrbeeibi.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhewzrew.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gkndzwgij.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbtiqzhf.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxrqahefp.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwwrpdwu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gtztzhlrp.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxobatvb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gapapmnmq.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqpzocbj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gwbqpliiu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gedltqpnn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gahnkgupf.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnizyqzxg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gmphucbys.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsfprtev.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gdgwtiiwp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gknquxrfw.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gusbywsmt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gjthemswk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gkkijbicy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxyedzgz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlfimmbj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/giemeawge.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/grjiuijhr.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gonnesuap.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxsdwyfs.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmsdwibz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gwzdoxphe.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gcolkbshb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gdjmdbbod.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gtuxycqfe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgttkrtx.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihzgjbcc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gelauyhxo.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gvtyxhyfj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwavgtxhf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbjtevzu.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyingxxt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gzkcaysjm.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlzbinsz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gupzpakxw.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/goggahvuf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gwlkoownc.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gbnvigpof.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/glkvcgesk.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdkqbvyt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxphlkdp.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlymdfgt.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gkrpqnhjt.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gikwktmbl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gvqfoooxu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gvjnyvzhe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gkahmtczj.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaeyktgp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzussfgkz.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gxzdaxndz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvftfrrqm.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gtwujpmlw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgeobyct.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gmesdshhn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gvzojwdnl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfcaadqhz.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gumdwiurt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjyuvlhf.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/grrocleas.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gqasiiqzi.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gpcvhxxrp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/glixwnjsc.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruoplojb.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxhxfsah.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/grdglsjsi.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gflaemhgb.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gqyebvyfs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjagyhpi.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gphqotwjr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkacklhbq.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gexvjlxpi.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdndsdmqp.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvysysroo.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnlujmck.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqulzvtp.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmtpslhq.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcramfphs.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gunbguyzq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gaertnnah.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/grfwkneks.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glbunprwc.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzjqpxgq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gcumqpljl.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/guycfengu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gsampvout.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/grgfywoqm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrycbaog.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvkpmtsv.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gwohwprmm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgbqzdig.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gbitsmfkr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gymffsgtv.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gbgdofuyx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkudvjpx.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gcpwkjrrw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfbizbwm.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gufkczstt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnahlxbb.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwhvkjsu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaeggknc.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gqufielvm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gydkqaoee.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gjcoxjhue.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gotucurch.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/grkzmnokr.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcxwfazfo.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/ghzxhskbi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/geuubgegf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/grszlkgeh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gxhcpryln.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqauafxkp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqetflvj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwipqpqyi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gxxvgcmyc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gthpwtjwa.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gaisnsgps.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqvzbspx.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gihwmljtt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqifwztof.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/genykleht.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlcfmawa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgvlgnbs.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gejdgndgo.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/ggyqamjjk.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/guxxcpjfo.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/glgfycwrc.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gicrpmooi.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbbmqrtr.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gdwmuvmvy.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgebdqux.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gcyfqkgjg.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/grnbzfyff.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpxybgopm.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gkdhxfisk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjjweglhy.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitsciwel.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gdwrcbqst.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gtzvhdfni.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gqkrzilpv.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gemrkodnf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsudvwfj.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbjcoupx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gofajhdcn.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaswskoj.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gkftgeybe.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfprdmqnr.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gvbruizkn.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gpcrwevtj.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdgpsjrr.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxufbbgbu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhcogfgw.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gjlncamlo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdfxtefqr.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/georcoqvg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpuqcahs.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giiibieem.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkfkvyoga.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrcxpnpf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gltrnzqvi.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/ghdvuoupw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyjawikea.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gjtxectdj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpeovxzh.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/grdgrdifs.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxicqnwgz.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguifnlpn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjgzpajmn.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmgzefdvk.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbkwzhet.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gpozlqrgm.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gljxsdlhn.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmehnuzih.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glhjgdyah.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjayysjvw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdbtbnfn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gupcgxdmz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeislfah.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gwpbugzkg.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gzknytutm.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gybyskrzb.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gipdxzlxm.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gmrxbpgbg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gnzijmihv.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbsiqodd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyyjysrv.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/givgwkmcs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsqeutlk.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/geayqqxha.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gweprtydg.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gfbgldeef.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gudticbba.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddrrlrso.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytqhsslu.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gmonogicy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gbxwiyvfp.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gjdqlmkbo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/getrpjtfh.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvymkqhc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/garxltwvu.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqudvxmb.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxkksjur.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gbnyfllas.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gnihsdjql.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gxwuwyzdf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqyfyoym.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gofbxnpgf.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gginaztet.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjamkftiq.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gbycnwblc.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkyvfzfe.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/guheiylpo.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghgwkhmib.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkszrrpgx.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gccilsoqm.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gmkoqibzo.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gkjhifoqj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/grfcawcyi.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzvzfijw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gdhoqbuih.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjccxecjy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbixdtvog.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gzvwdbdab.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwcorggo.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/guacujudg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxcfqtvn.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/ggfvyzyeu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbaadanpw.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gzccijrml.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gztbuinki.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gxevsotyd.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznccknki.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gpsrdhron.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gtpjlhdoc.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gukxmgrzg.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjirtcaqa.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gpijihacb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwvktzmv.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqyjajcw.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdbkhdpw.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbkfaepd.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqkhamvd.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznsdyimu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsjrkgcf.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gqoztnvra.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqqxilsi.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gorhpbuny.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gqssmciiw.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gsbkxdmsa.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gdthiunkf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxcibhcy.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gjswczkux.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girxdrmbm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzqzjnbj.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gjaoztzas.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsobsldnb.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfayipdv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfkpulhx.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gehhiaeur.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgcjaetw.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqeusxcx.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsurfqep.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxxkfrdh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjumuhbew.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhcluaij.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/glgvbpien.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gfloukajg.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goouuragu.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gleufklqj.sHtML


<!-- 参考信息 -->