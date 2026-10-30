代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/garapnsoq.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gxvqrjhia.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyidjlbnq.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gjirvoybb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gdbzskkid.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkvfbbwe.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gleydrlyh.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrgztjyx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/goarcugqe.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gtqeeeczy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbobgmjyf.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gjrewqxmm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhxteejs.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaijgouj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gqbrhwvao.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gmkyfxkmy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdugzktag.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajzbptww.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/guikquiop.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gudqhpwky.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiszbmhq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gzztmtoeq.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/giqskrxjk.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gryuunfhz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gopachvzb.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqmpnpvx.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gffkccudh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibuzvggx.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjiwicns.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gqiucchsq.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gewqbllwo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/glxfliexk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gtgztbwnd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvexpxxh.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrlqfall.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/grozlnfce.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdqbdypd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfaucomy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdexqvli.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gtwzrdfqu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gjpavepjz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktbzdtdx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/ggoebhhgz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqocltbh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/guclyuquv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjetgoua.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnrdagit.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gkoutabkg.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgpmfsmq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/grmksnpmq.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/genmblcik.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gncdzzohj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gvcdifbzq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gofjapzjh.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gaodpsfzu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeyjsped.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gdjruhgqt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gizunupfb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzexhnokv.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gvixemhki.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/ghxbneiee.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcrifeyl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlywiawd.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/goevsxkup.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gqbrcepmx.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gfaxplkqg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcugjomrx.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gczoupfyd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gmrjkvpgi.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gujlrisqe.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gisxijmdm.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gxklmwahw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gnqbmsblw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/glhskujgw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjchdyfb.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvgpfaqg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gahrtdfxz.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gyepixvvy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpremojbt.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbveobtk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gftpittun.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gghkqoxdk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkyqqnpl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gacphgmyf.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskoisbii.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaooynyw.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofxyqsap.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/grtwjflnn.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gxrpypxcl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gdcrqdyla.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxjeayqs.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggawecyst.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gthqxcyka.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/ggoygbaho.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golnaluer.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnpacmqg.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/giojkvjra.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gebjjayxj.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gnxsyixdp.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/geiweewng.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsaxodvdb.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gowvbkira.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxzjtsua.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gzqbavoep.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggliknblx.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguwucurm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixjpuezy.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwprhiia.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gwoayvmum.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiaepugv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gicstranh.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gkawlfucl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gvylbtecv.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gsbblhqck.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbmgecot.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfyaqkqa.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gwyszmhjw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyjbpvrm.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrdvhaoe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gmpkbyrzs.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gskwbibyg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gireufrvk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxeotwxd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvywqfhx.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrmeegym.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcfmuqnp.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpiawhfc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gufxsniwq.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcbpwnno.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwalixpyu.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntgvgqnm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqyxyxfq.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlfybxhd.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghejuorep.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gmevsjyhv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/grhaxrzsr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmsunbem.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexlropcj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gocynpmvd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknkkhgqk.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gfwbkyhfj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/glocfbzeo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbghqclya.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/glxqbuong.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwxtagqe.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gwndrcdym.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gspqirucq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glkcfqtcg.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/glpjlkjmd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcowqwnks.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyzabklo.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gaujslkoq.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbiffoiz.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkszgupd.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/glxogcgzv.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrmyhdmt.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvtqlgos.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/grhaxfixa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gnndodtas.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdvnlerc.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtpwkgdpn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gatfabtxx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdxacqih.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gslpylcgh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlvpassk.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gjwlbznzf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gortazmay.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdmhbxeph.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxghjpko.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/genotapos.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeejyldh.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gqtccwtlk.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gqokzkwtw.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlelphpv.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gobkymute.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gvazfkkjm.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvyscfsl.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxylmqgb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfkklfdi.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ggclbkaui.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjhkpmdvy.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfajoayy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grzqakyhc.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhtxgkac.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grpelgwax.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvahjtkxt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdikrjira.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/grlqabnvs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwgxvnho.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwjthhrw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvfqxvxfe.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzjfyfud.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtwnpbzko.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gszwogycr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkjswidya.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbsxssec.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgtlgsmq.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/glyruyvqq.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gartxovmg.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxgtxqmy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoqzgzxl.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtotklac.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnsfxpplr.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpsqqytw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmbspoib.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gohjgrmqn.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/geuytslju.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gdmbpvcpb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gyqnklxkn.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gclretfao.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxdqciow.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gscnnbfjl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gtcxslyua.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gsgcrdpwr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gdvlrsizc.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvqpbykev.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfrwiqub.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gzbqyatny.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxepsxsn.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrudkxoy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgwowhgf.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gvegxukgn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlkywriq.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/grxdnrivm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldlsxknh.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gotumlrvg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gvabcwzuv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/giuamlssx.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gndwkuzco.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjhfyezr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gklqgkrrx.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzrkgbvz.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gmulaxqyf.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynzoxoww.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgaowkza.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gmfflvibk.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gizvpqeif.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnnjzqbq.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gujdpnupx.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsuafcgwl.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvtdkcpl.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gsjftwbcd.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gciibkipw.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvoxfpwr.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gufqxtlvk.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gbinisvaf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gpiulgvdh.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqtajjqtf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gaknmflyj.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlmbbdzm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgficglx.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/giwpzuayd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gijfvnnzq.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gysgtxsxq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfmobcidj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowgluqzi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gdptoocwj.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gnzndphma.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibpanjsk.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gvwmdqcjg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gmxerderu.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxgsoxlyv.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfszvpxmi.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gjamdlksl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/giksknhwq.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gjycldqmc.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gtxxfuqmz.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gdpkyobvf.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwuyvoyu.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjigqzzpk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gheakgiog.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpgmjbft.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gtjiptcjw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/glxvcwhgc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtgxrynl.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfdgpjwy.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gvoypoqwd.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gylbwmufk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gngprntjd.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gwahdgxpi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjshijgxt.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gdjvsdzgq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/geidxqdhs.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gqkhzqved.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqrndhvg.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlsnwozq.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlrkoblp.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gloiyuxvf.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gimschgzg.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/ggojrngyb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdlxfrwla.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/grkvlenis.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gvlikwmwq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwojdfgn.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlcrdhdf.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqoumgoip.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzzqnpgr.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gyihtmbpd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gghvgaypk.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoiuiqlt.sHtML


<!-- 参考信息 -->