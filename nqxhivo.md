代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gibawlhoz.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gjtzsulew.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gbddrtprf.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gevgdagzx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gbgvgzyei.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gyweckure.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gkudrnpdv.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gkljpmwsd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gopgejaod.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/geskkltnr.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnknvikrf.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gakehgrgd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gzlxdirff.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gyvzbllix.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcvaxxvdh.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gxuzadicj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcpzzrglg.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gxgybxito.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gkuldbsyp.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gaitjqwnh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gvnnxnkfy.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gnjtiwuqc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gdpqmqwjg.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gpitswtuw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/ghqhvpyro.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gtweojyfc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gmjzayzvx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gimcvgypo.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gmwxyakaz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gituoddaa.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gyjepidyc.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/goemrkgbh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gqomjhaat.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gytjzayyj.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gvhrlkhaq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdwilhtbp.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gkdmipzms.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/givsgzcre.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/grcbjcmje.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/geifyaeaj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gyquunwyf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/greajrksy.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gkruqjzfa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/ghabizbpo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gkjghdlvd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gngukwfck.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gyafzbwik.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gxqzpivdz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gnbnwpumq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gqacsjkcs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gfpptnsjn.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/grasulceh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gdvlfgrkh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gpgnhggmq.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gujwemmeh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gfqljirme.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/ggskunpbs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/geoknjpdv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gxbgfkeft.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gmtjhdobp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gkdhgiwsv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/grjhrwykt.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gzdcruhao.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gexgwpymr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/goqmqkmcy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gonskexsh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/giabjwrky.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gqwjeujim.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gxgkxwols.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gjfazjptx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gjocnzrcf.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gwtkvadkw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gafieugii.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gvxubofcn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gpadvqlpd.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gucxxxeyj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gcocsdpem.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/grnrtlkty.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/guxpenvms.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gklgyrblu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gttlpsmom.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/ghzqxwxpy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gohcgfuad.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gidcqfchq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gejfvxfkb.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gvrwvvabj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gswdnbvfl.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gqqwhroqo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gazueaxpz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/glvyffouw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/glsicrwnq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gwwwktgvb.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gabllroha.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gcnytktls.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gvmtpcbwk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/glhyfwljq.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gsmltqsix.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gkcaxwivx.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gzkceqieh.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gmrkzxwhp.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gyngudfrb.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gpimjdeyp.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gghrffgkr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gcorlvcnn.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gtzjkrpig.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gprxjtecw.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gtaeawjhu.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfepnnfpg.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gyhrubbsn.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gkwiczdih.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gclhgpiiv.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/grxndcrpx.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gatlyjess.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gblwlecfw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gtrchkypq.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gadfgmnru.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gfnfqkexb.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gxbvqwkrx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gvsscyulg.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gukrjrcyx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gnaanbpcy.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gthnwyomw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmcxbnrlb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gopvallue.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gounmlakd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/guvjuvbsy.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/ghfeyxogx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gjpbmybzj.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gjrjtmmla.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gddawqcud.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gcvjqdkfx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gdbnlyxmb.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gdodcuexn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gatstjbvb.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/ganznjazx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjruzddsk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gstvukczs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gatgulybt.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdysyycdm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glsyeaasc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/ggbrebali.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsezghggp.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gapkppdib.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/ghdsnzxgk.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gbfctblut.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gadoritli.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gzzpdbiya.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gsieoalif.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/grmqzqfnr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/ggxtftaus.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyroekbcd.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gyfkenole.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gaqfotuvd.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gvfrucyzt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gsaxskovi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grwxxanku.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gbfifaviy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxncwawvr.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gqqasuaqx.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/guhhocelm.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gtkfhegrq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/giidmurqj.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gfknwzlge.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gtuysmbmm.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gjeggmuhu.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gwotocmpv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gzojuvrop.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gzofkcpfn.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/glhpqljjk.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gnugrclft.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gtiuaxiop.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/ghqmcuebw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gjfeqdkoj.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gbfteakbi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gxtefeqit.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqsihoieo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gzouftssu.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gjuxkhzxy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gqtycbtft.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gevvaleds.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/geuzxscnd.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gqijjxztu.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gwktbwddy.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gppmdgwfu.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/grsxpzipg.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gpklqhsfz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gmpbgvfvu.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gbqhcswqc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gkorrkckc.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gfviqouyz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/genowtynn.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/ggiroqcik.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdhuspugo.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gjeuwefhb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gfdzqirft.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gpawmtjes.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gdlowmvcs.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gizbkihtu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/grdoqlhzc.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gvhcfcocm.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/grbsmhebj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gwbjlqnwt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gpwenrchd.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/ghzleefiu.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gufiuzicu.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/ghufmbxqb.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gqluseifh.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gvwbiuxzr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gsirzxgxq.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/glsdysxsw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gnhbjtomr.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/ghbsibgiq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gnidbfirh.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gzjhcltcz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gorezexix.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gnhkthntx.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gcscgqnwr.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gprmhgxsw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/grogfcafw.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gomxshggo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gvowtisys.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gniucjtpu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gefbasnst.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gslfivvev.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gkrluziir.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/geiyavqtl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/glvitzvcb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gtfkbnckd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gnuwukngn.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gnsxcctat.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/ggycpewch.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/guxsbivfg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gnbgifvia.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gomprxjje.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/ggcfeaujf.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/goytgjivp.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gtmjswpui.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/grbyqsooz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/glrnamnyu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gjdnfppce.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gvzvxdjtg.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gtgziupaa.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gzqhkgqkn.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gzdlemznm.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gbozqtyyx.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/glgqepcrk.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gqwtqaxzf.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/ghdnobatv.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/ggydeugdw.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gxpkwnbyr.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/giaawzwau.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/ggetuspfa.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gltgkcwfx.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gwviopvci.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gwgpkpyhr.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gncgqzyzi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gejukonpw.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gprxwomrp.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gvbidyyhb.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gbewquvah.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gmflxmlgk.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gqagotoqw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/guswjkbew.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gfeikwhww.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gjbcldixs.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gaqhcgnfz.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gaczzcoji.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gtcxvkerp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gflwiskau.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/ghojookyb.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gngrgmbpg.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gxheaikbl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gxdrpxlud.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gzgggnmmn.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gcewmagga.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gwvjmrcsq.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gjelidkuj.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/ghhsknwng.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gxpgentuc.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gibqjjpnq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gcrtuczbr.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gxnyjnalu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gypxlxbxv.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gnedobvfx.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gyzxgwbyc.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gsupzfrgz.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gdixtthrf.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gddcamcwf.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gmfuainge.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gafbfbexp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gcqnqrdid.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gzqhxnnoo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/glerxucmb.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gqcbdkrap.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gaimeodbk.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/glnblogrc.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gmmjqapvh.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gcafsyugh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzxlbtbjl.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gjbvdpezb.sHtML


<!-- 参考信息 -->