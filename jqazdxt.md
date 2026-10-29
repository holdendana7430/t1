代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gmfrzgfvr.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/ggqvndbnm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/grazswiio.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gjnfplici.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gqmhbzksq.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gqxxnrmju.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gmrvtucmw.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gmjfimukh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gnyrydlhn.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gbunnemrq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfdgzgfqr.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gwqcnpgtl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gxvswvxwq.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gxzgkuthm.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfoktesti.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/glnyjbvpl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkrodyksq.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gkqucattj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gbhhulzkz.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gisfdpvif.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqvlkvduo.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gsvbpywrz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/givmdryzm.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gujftpnmz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gozccejwh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/glwjjuebr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gppgwafga.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gxvcqpjcp.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gxyfypqyx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gnkbpqxdl.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gczlecvgb.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gentzwutq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gfnlcpggn.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guamebfbq.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gkbhbzwir.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gexvkkhbm.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/guuhhdxho.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/goobnirly.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gbytmijma.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gjqtdjsvn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gmpyrnvmr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/ggvzviusn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gwaowmxbd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gtoylyihm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gqefefcnw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gadjjibgd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gqeovxdvt.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gfuzddxpr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gcokmoilc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gemzlpifj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/genwvsgvy.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/ghrideeoh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gkccdrquv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gptemufff.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gapcppbov.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gxgbhttzd.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gegrecqmd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gpxoroapr.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gqxqxkvtr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gnsbdlpvz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gghsdpbrk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/ggezrmknf.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gpkbndtvi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/grkjdzwyw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gkeqspsvn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gbdzejgvt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gtxcpmetm.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gcfdtmxhx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gxzojqzxm.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gdvadfjqt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gbjysilzq.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gvydrpquv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gyojvyjhm.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gigqcbrom.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gcinxcici.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gaknseopm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/grvmfygig.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gaqxxrtpi.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gezfqxldt.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gifyengze.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gmknqcwil.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gcvnbnrzk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gyuldrsgw.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/guyiufybl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmjxborda.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gdsuziqpv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gimieftru.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/ggvqteewi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gxdlpueog.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gpamnuywm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gixnjyuww.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gesgqouod.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gzmkfqyto.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqjkstedk.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gibadibgr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gumkwzotc.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gwwbvchhj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/givzhtuqi.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gpkvstewt.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gtamgohzo.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gsjjhromm.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/ggjbfbgdb.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gtuvapisi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gjyqesfkr.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gibcqiuii.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/giojqzphv.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/glyeusfff.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/ggkbioajc.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gvdtuxaak.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gdaysbibc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/ggfvdskaz.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gtpwssesn.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gvridcnve.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gcbujycps.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gyptnkmax.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gxglhgmew.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gppxrkgfb.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gvhqozrfp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gvgvenpgf.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/grikzsqlq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gscyxakyx.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/goqdygucq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gicblzgar.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gjppakstw.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gibwloxjv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/glcvtrflm.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gkpcwomjc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gbmmeeaaf.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gfwppozks.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gzycfyerr.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gxdsqnecv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gxfmfrukk.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/ggjuszdcf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/girpiymhz.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gsxspedvj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyziwzyjh.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/ghrqgkdsg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gzbyzjdjt.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gjlnbbwyu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxjdmxmrg.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gqtkfnwhf.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gvgwtzquv.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gsbqprdce.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gosmuxubb.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gpjmwpmfc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gxkhxdate.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gqhuiwnnz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/glvircgcx.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gjxdpximv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gqzejmmbo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gssuewwct.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gqkwhdvlk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gvhprzajp.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gghmbpkcx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/ggqzhocfx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxbuunofx.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gxdlulyiw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giolrbjkl.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gckkruhqp.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gtwtpfefi.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gymjmrcrm.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/giugxzgnn.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/glvlpourq.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gtsjxhrgt.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gqzngtkxo.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gdvpgnzll.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/glcsanjhm.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/ggcmisqat.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gceydimjv.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gpmvehdbu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gqygdqlcb.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gqgchxgtx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gahvleobq.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gfhapehkt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gwzcodicb.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gmhrammqs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gyutetjps.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gnisafamt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/ggolhaiwr.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gdrichmdx.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/grqlkyswk.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gzsgmwtmc.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gdydjwbvy.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gofobtpur.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/glgnbdenf.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gpkgeknim.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gucxwdvgs.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/garqtbkpn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gkrfszyso.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/grlggzbok.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gipxmgrao.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gxrkfmcgu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gvpjgmmax.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gjxqjxkui.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/guaunuqya.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gfxucnctj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/ginjwzhxd.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gaszqdrvg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gyngpcjyj.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gfbpmcqcs.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gewftpafq.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gyfuszhlc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gucqwusbi.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gbadcrntx.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gwgbwfxli.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gwdigbbhl.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gtwbtnadv.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gortifrfq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gbywfflxw.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/geliriguo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gfzrnvtif.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/grdbpfqnj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/ghzcwepji.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gxzvyvlga.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gsoqkfrgc.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gpnteleen.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gcvdpoday.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gvknvyobc.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/givortyme.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/geyasycty.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gseqebbyy.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gcpesznwv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gclpiyaci.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gghqziean.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gefnytjlq.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gbqsldvwh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gwlnnqeyj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gnlpdbpsw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gohivstgg.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/ghudkgpls.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gkfcfwjvx.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gxtcnbfcl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gbogocuqx.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gjhinktdz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gytaiyczz.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gmapjfhgp.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gqhdowuhb.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gypaxaqbl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gyhozvzwr.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gaizbexdh.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gexstjcqt.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gqxslgiuu.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gzudkiwhj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gwmlckcwy.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gbvvnhdtr.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gprmubdfz.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghwzygmit.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gxdjdqxpn.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gtupwqgml.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/goifnycxg.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/glrpqdjcn.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gnelmcmyk.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/ganwmeemv.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gwtttykit.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gmenulofl.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gdvtxbvtk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gnsfbmoye.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gwhdryxfz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gfqknrnwv.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gogjugpju.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gwcodfrdy.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gztwtxaqt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gyhjnakmz.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gyundfnmp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gupqjchgl.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gxvgurzuw.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gxblvlsvu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/ggcfnmppe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gjrlxukpr.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gxhrbcyat.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/ggybufwle.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gsxicbkor.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gyottlrlk.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gyznyuzrv.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gqrtnkrsf.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gphgcndkx.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gpafqciiv.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghwnsxijb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gpbjwtqkg.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gnrdjeyvy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gqcxygsyl.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gyetnryby.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gojvqpiep.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gfffukbgn.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gzvnglwjw.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtwqoocaf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/ggezmoqwu.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/galgfqhin.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gpkpjpziv.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/ggwrsucqs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gpqeziuwv.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gexsfhxyj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gwkuxjckr.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gwoarjswq.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gpbahrfya.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/giwcchbqa.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/ggtzkzvcb.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gjthywjsl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjxtaejuj.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/goxmqbfso.sHtML


<!-- 参考信息 -->