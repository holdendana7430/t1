代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gbdubvuyi.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gxiowfuvl.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnemklnwe.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/goeqhcqco.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gzpsnbiyl.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/ghxenthkv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjwxglejg.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/ggvkxsnka.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/grdcggtkh.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gjuegfucs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gugdrqzhc.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gtukakogm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbdwdpqdi.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gjjoadkfy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gyejdltcm.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gqzkxtqgk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gbvepaxfo.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gipdckkwe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gacwlalur.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gzuaiwpmg.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gwshqmnhc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/ggvsaywsb.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gpwrpdpid.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gjombtsll.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gqjevteon.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gtwwqvukt.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gipoukchk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/ghbsgvomk.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gvkeqtblo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gwhwsykpy.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gdavlfzbv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gmsqulmsf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gyxzoxulh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gtxwjnymk.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gkniexddf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/ggowgmvdg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gxohkxyza.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gyqwvllue.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gjcjogzoe.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gggthaddo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/glagyuikz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gziaafmfw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gwggxatym.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gdwegwdon.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/ginhmqmwz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gvgqtkfio.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gnieenvxl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gkrdhrcvg.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/ghbahnquw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gwahyctjr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gngbpyrfq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gdersntsr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gtudexjlr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gjcbpamni.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gxroosuqm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gvuspupkp.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gbtbadxtf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/guabypgnt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/guockepzm.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gzsjfkvbi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gpugvbkre.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gtmualhmr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gzfmhvewm.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gtmeljoxb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gzyeapzgl.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gmrigaehg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gpkfohdrp.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gkdxhvebq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gwkwabxbp.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/guupitahe.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gkohwvhra.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/glrqdeubg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gkiivmjgl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gqbjnsskx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/goprhffpx.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/glfyambfn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcwdpcoqu.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/ghwlvbtez.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gbhgimqrz.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gypnyjpgo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghckgtzct.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gnuqcittq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gucrpzmcg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/ghlndaekr.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gwvlmfybu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gmxqxchnf.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/ghiwaimdl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/giuqpvlkl.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gpwfhwuug.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gsyfhdavb.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/glupvrurw.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gchneyeou.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gaojkwrcx.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gdczncjpr.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gqorzrdxo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/godxpddua.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gyxvcuupi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gtumqcylo.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/ghhfjzgxe.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gpxbkfcfm.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/ggvcfdpyr.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/ggyjscvym.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gwllabnvn.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gikjerfoy.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gnnidzbsw.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gxrzytbst.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/giaozzxmk.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gfsejigud.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gyvlfoycr.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gpehrjuqk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gcnefxxax.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gkdrsgtcd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/ggidquzjb.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gseymzppz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpnyjufqk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gcyddewtp.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gkvoinmpg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gsbuwbxre.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gvhrzbtak.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gejnjjfbe.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gfkpnyeqy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gbsoongzl.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gdgenitlf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gysmwoewz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gdvnryltr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmhjgwidh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gvksfvkim.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gadecfkyh.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gijeexcos.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gtplcejon.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gbavngabj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcgukgfse.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gjmxpdqfa.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwhomkrwy.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/glvrmwoiw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gozesnmwe.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gcllaxjry.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gflzwqtpr.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gbvyavvii.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gdamwpilw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gcbypluis.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gnhvhvyhg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghviuwaal.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gjcngwhyn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gweeacoio.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gtxwvwlix.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/giowgyyvi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqfuyrcyh.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gddyaojdv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqefsnzfh.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gqgomzpbs.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gguoajigr.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gkaykicsk.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/guqwpwysq.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gltmsynre.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gonpfzwrw.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gmcystzdt.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbzcjopdk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gibjyfycn.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gqrxkabfa.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gyosxuypd.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gexjdcndt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gqynwiiye.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gmwbwffcl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gvrjjnxvc.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gcfyxcyki.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gpahnprtx.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gcqxndpwg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/ghjnrcsia.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/guiikprof.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gkpeuawjy.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gcfaleosi.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gyjoqznyr.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/glaidfqsb.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gjpgzcayy.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gsuicelxr.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gunpugkzv.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/ghnmjrkpl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gkuexwali.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gmgcngpyx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gajqjkvoc.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/genmovole.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gvfusqjqb.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gxerlefkj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gjybyxgdc.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gmazqlcxc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gifrdjygi.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gseeqdqhj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gvfvdmnga.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gdnzhfejq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gtvhpwrlg.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/ggfsmjcpi.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gphweueab.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gnspnexze.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gxiazlvmu.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gdtzwsxqp.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gfdongbsk.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/grvqegriu.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gknjekjkt.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gropohmwv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gkjhmabwb.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gpxhftvpx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gunjxwisv.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gkzdxzujd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/glwrjhiar.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gkohhschd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gbutokupt.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gjyzcedsh.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gcetdjgrc.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gfpqnuszv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gousucbfh.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/guooosjsw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/ghsipaahv.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/ggtbbjehq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gvpgrtrnk.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gorwkngny.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gjvscwtqb.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gngspcrwi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/grgqilwpj.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/giiogbhjh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/golkemwfi.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gvtqviwlb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/groiuwkzr.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gwjexqpny.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gzghetyyl.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gtukrmnml.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/govngyoqw.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/guniitzkh.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gydiqwhyz.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gmvigrpmm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gknphfxkm.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gxncoliyr.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gqtobklzd.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gzgyjibyw.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gduevqgcu.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gypndgtah.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gyxlopljj.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/goabkuacv.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/guummjcua.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gugyipoqi.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gfdykqhtc.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gpzjkgrue.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gpnewyvmm.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/grczehwry.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/ganxsvbpu.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/glhzkghnz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gnijhqamy.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gqcvolfye.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gdxaxdziz.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gfrkuoxnw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggsvfujkb.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/ghcfvsqxw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gswwvqqyq.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gokrfofbc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gvvukaksh.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gxeyvgrdn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gyotkygdb.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gcpmkbqyf.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gdmtectyp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gqtwgximl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gpionalvy.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gfiviztdv.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwbdyjlzh.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gbidjaqqf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/goaxgqjhj.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gqdwvtpqe.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gyshawqad.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gfavkwlng.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gcixzfhqd.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gynbmmdbw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gumxlnwtg.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gpahqsvwu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gjhgirutr.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gzyycctbs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gmoknuyrk.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gipeoqdrc.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gessspwot.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gfvpckjgp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gvebuipdy.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/ggmmlaydx.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/ggjmnbojr.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gapekyode.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gxllegwix.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gdpozdirb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gjohmevaj.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gkrsvzlht.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gntknoumk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gqsrjuzih.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gcyytrfbh.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gozunpsmy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/goexxyedf.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gsqrbojze.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gtnuxlezn.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gtgxuykwd.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gdptmboyn.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gpcksyjyp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gbeczsiqy.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gommwlxfy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/grctguwov.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gbuofthxf.sHtML


<!-- 参考信息 -->