代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjkeyzis.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/grljdnojc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuoljhea.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjwtfqtg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgwgsjvf.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gglpxjkwu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwdiazea.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gknhichgi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlhzrvbx.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/goeueylpj.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbuazqlub.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gmunuktin.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghwhhxwlu.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvleuyfo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/giiwgpiwl.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqeulxow.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrptuwvx.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gcznmrulc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gkbzwhdyh.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gcwkwfudv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gxevintoz.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gugwltxkf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlcwkzsg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/georxocdg.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gyruitsjj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmlqwzxt.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpgalgpb.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gzigkcnrz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gpytxthvp.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gyvzunesm.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/ghssnwkzl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gjvotjnli.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzczsbdi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gnncxetzv.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/grermxqhq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/grlonhsmr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gxoentnqx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gjjzdxgnt.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gqguvpgmm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gnweivuog.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gscxfkcuh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqkviyig.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyucpnndu.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gawhkddnp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgkwnjgb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhjfimvx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaehkceg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzfkwsqk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gvtaehpkf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpplymcmn.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gsxqvxeiv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gplxhzxbp.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gezreythr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gckqxnnng.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdmmdxeo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gnitzhhya.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrehjapr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxbqypbg.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnmnfphc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcswzgibo.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gtnvwvgys.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdpniuya.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gygjlydng.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gpqaqptlt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfdexiqh.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkoomlej.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumzemicu.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/guizahvwd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grfsiklfb.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gakghhwja.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gknkufmgm.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvewddpi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcbbkdrd.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/galjbewyz.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/grjcgzkhk.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdwpatsw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpudtwlh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gmcagveen.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gtdduljtt.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gsnffdpnf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gywdhereu.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqreyppj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvecveyku.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgqbhshm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gzzvxohsp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusutxrpg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpeucwjc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfeetuulb.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gmahiaaiw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgayypbr.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslvbhnmt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geimatlex.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpftdqkx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gocglvtow.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnxcifax.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbvddbfm.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/guhwhgltk.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gixyzeqig.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gkruukltx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpkejnyx.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gurpwuupp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gwqlzhmjq.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gemkkgloy.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/grabxtusz.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gevorkyjh.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gffuklnub.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmviygmn.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gajbxhurj.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gobzdnsde.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gpscrdvru.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhlelwhr.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gqmthgnsc.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeoisemq.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpefsxnkg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmntbgxl.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gylhiykev.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvorionsp.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuukoksu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvlxqoiol.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gmsxjrild.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gctlynumy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmklzkzti.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvayoqin.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gotkkjthk.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gxrvoskdu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/geqlazutl.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/glxzckwjg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gchiepwvt.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypjmdwlu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/giteiidfc.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuqtgzcr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqfjxogq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwubwwysd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdhgkaix.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/glnmjnwqx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goguobmez.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/giqirmitg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtitvjkm.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gjjfbikav.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guspucevf.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gprbnoigf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/ghfnczlym.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdfspiob.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuczilpw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnakdfmad.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/grtccaqjl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdaylaqd.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gupiygled.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzipprbp.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/garriwpto.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/guvbsngbf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzpkdkng.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gmrokiily.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvzkckjwy.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduhcunfc.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeebpphp.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gyovyenqz.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gvnnfukqw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlbkjavq.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/guevgbbmh.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsyxkumt.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gdoiafcnt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gkzduztci.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeyxwzlq.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkzggure.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gseswfkge.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqpgycpwq.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gusrtzgmi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gngdgdwcz.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/giexeokrj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygumkksm.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gdgiozoda.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpfrmltu.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gayjpamet.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gzlyctzen.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/glvilwsgz.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/glibsvcxg.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzegrjecs.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsismlde.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grvlagscu.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgpbibtg.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwjcrzefi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkyuravh.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gaygtuywu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggffzqalg.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbqzdjza.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcllxqqjk.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuhhazey.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glnkoaimj.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwnihujp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/glxvguahn.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gmeabqdeg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnxsfzkv.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gixsvmija.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gybovrozi.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gqavftvdi.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gctpqxavw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpfddzbi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvtaloqle.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwnlzjbfy.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnafidcc.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/grixcbahv.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtgsysosk.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtluirwrg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gndjnmejo.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerkpasoc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoqppfsj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gefizisea.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwpfosinc.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxpooxgi.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwpbkpfe.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeaoeoqa.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gepoyibcn.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtusnqytg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gttqmyifb.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkhkutxvo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gocafvvwv.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkrixqxc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giehvckwc.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmiexvfg.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdttfwrdc.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmkplimx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gapeiwklg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gzityyslh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gaetuuimm.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyfivzyj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gyukinceb.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gdohlgwos.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gysefhfjb.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepixwerr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/geldbpmub.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghexmtozk.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtvulcfu.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckvzaquw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gxkamoszm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcfxyrcu.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqokmcfc.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrqgnrnk.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gbzmozzqc.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/glqlschnz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbidjuil.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtunoxqz.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdctsjfz.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvpungbw.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxljwkikb.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcwnmtuv.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gdnzxwqvg.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gabeocbru.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtejxizqy.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gtrhlzvpe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gplyrfuky.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjjpqjjx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gukylhbos.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gxoputaju.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gocsiuhmd.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxtueduai.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gcgwcweie.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/glkfbyftz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkfteaba.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gpibzabub.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gxalxuwfa.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/ggiyseair.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcadijaxg.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gbggijeto.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbfsgemm.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxdszcdh.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/giwdbzqzj.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtwuddal.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gozifwvqr.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gdlpygtjc.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gtremyqmh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxzvmljf.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gbzdybxrn.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/goqdxbicr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabjmvtkp.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gbizivrdt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gjprremnh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynksetnc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsirrmcj.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqxihadm.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgpqazjj.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjjozdle.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gloxexbbe.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gaqlhejqc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzaxmvwo.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxfidint.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqthgzwc.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/geaemxxmu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkjqsizd.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gciniyzxd.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/ghcffkoey.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkdnhwom.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giohnrtis.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gorfmfkti.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacaoywjo.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gyiwdgsaz.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gptclsvka.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gilmkykvw.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/grqwldvfl.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwqrpkvd.sHtML


<!-- 参考信息 -->