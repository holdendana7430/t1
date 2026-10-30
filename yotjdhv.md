代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/geabaaunb.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gtjruilba.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gagmzmwpy.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gifunbpld.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gqfaammln.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gdgljsakw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/glyxvzyid.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gcddwjnkz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/grvuuziyb.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gdanoqmmf.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmgwbbjkq.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/ganufkvtn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/goibjjaoa.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gzmzjwyiz.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxxbxfqpb.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gvgflzgzl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqvyebyby.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gqqrywsnt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gxzdiiovw.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gvkyizpzo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/giwhrszxj.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/glirggbkc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gqczjoxui.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gajyvmxwn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gtnexfxbz.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gyycgfvfe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gykufpapk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gkaquwakp.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gqfihseom.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gsabqteog.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gvwtuxczv.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gclewhqbh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gxeueooir.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkwqsagst.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gksqytyca.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gtzmzflmk.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/grvloroji.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gvuhujeev.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/glqkmuijr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gnivwsshm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gawmvueze.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gcjhuinev.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gdufmrsbr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/glmqogvub.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gjnrgxyzz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gcgrhkqcb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gbvhtkhvd.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/ggbrwvdzw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/guvnwqqji.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/ggwwnpzbd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gxmhyelwb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gqwldxumb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gxijexzhc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gqwlujbog.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/guhydujao.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gduwvbeoa.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gmxdlvpcd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gyguzznuk.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gnsoacjvx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gspzrddwn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gkhccjqkv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gpwfoyxnx.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gfjjmdkgw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/guzepdiwz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gzecuwkqc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gjwrmugxl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gxwdzjmkl.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gstglenof.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gqdnychgp.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/grmlzoiyc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gsrhgasor.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/glkihernl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/goljcqpfq.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/guagqxlta.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gjzolgcju.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gudvtixoo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/grvhwyrud.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gwtcqgbvp.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gkfyjjuej.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/ghipxuyvt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/girstsufz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/ggmdjvwqe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gfthwtjji.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gvdzuuiqp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtlqezktz.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gubljmgvj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gupffmuhh.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gzdhypkzr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gixwtmznq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gaddzqyvy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gwhenrllh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gsleahspw.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/geowtmxop.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwmxeaxub.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gshqeukrk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gpcvfdpyy.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gaiolnvsk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gqtevguzs.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gihdpitpg.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gxofuhqen.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gnhcxrfcc.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gcbkbiqyh.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gevuhtsfv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gaaaobglo.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gekifsarj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gkzlepxba.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gtbqtmnoj.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gbsgdhobk.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gqkrtdxbw.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gfewvnmkr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gwivsykba.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gyyxpydoo.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gdhcpzrvu.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gfkixewgv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/grrmqkpnz.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gnsgurphb.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/goeboawye.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gdwajgvil.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gvxvctwwx.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gcyskznnl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gvddwducw.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gwsnmqmnw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gungtgtpn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gimhvslsv.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gggkvzgyn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gzctpbwiw.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gbjkshtwd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gjsqidoni.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/groqojnkh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gbvdswahg.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gqaynakzs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gjjgvqdxs.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gvthhqcnp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gacbbzehv.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gyojuuczl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gavjsuoqf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gkldwfhlx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gjyixnphr.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gvowdwrwc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gkeicgmmq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/guqtrkxfc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggcbxvtjy.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gdcqmnwgs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gomusximr.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/guirgfgtt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gupngjfzp.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gtrgkdjlp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gobicqhsl.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gsfsasqve.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/ghanfegeb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gztujuaza.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gygudqayg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gcjglarbz.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gztactrdb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gkximuzwi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcxbhdhjq.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gqqlwvnqh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghnibvagk.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gpzlxzeev.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gzpogrkrv.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gmcghivst.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/grjnnujpc.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gpbmhskzq.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gffyodlap.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gwsdrqkyf.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gsqnksmtr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/glmkalaot.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/ggbckmhkz.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gkibaqgvj.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gsaxyldft.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gnfynxiya.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gbmehmkjw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gtidtqbrs.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gtcimxklm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/givhuncnt.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gwfzxntgc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gxxzpfrvv.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gnxxyfdrz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gharkabmq.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/grbnfwgtu.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gasfmjler.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/giiayhvyy.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gzyvkxlsh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gqmbynzqq.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gzovzukzw.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gwrkhtiwl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/goxmbiign.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gvdhcyssl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gxailrupa.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gmoqjkphj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gkpzpvmgk.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ghabfqqpr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/grtytzprq.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gajacsmeu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gnddmfajo.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gfzxtzjnt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gmnqvsbzj.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/grubtfzos.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gcbhttmew.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/glytulzhk.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gxlvcawlv.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gqadccrpb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gdrwqygsc.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/girkbjiqn.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gxlukxizs.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gpglulvpp.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gfyrlwzgq.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/guwnrpeyd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gmnmpjpmo.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gabvbepou.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gonrauqap.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gqllfjjzl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmfwkkkoc.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gmvbuatez.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gjfvlukjw.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gjvjhxoyd.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gvwftmtzh.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gipjjvski.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gcmfqbbws.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gdxjixvtp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gmzznqgpn.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gyfsscwfe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gjwdovtde.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gcxhjbmuj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gclhldgul.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gudecidxk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gcjdiexjc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gbvbvnzkg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/geogirxzd.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gctyhpqqx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gkxomizal.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gzxyhmfae.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gzmpaacgq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/garivabjb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gqjqarfvm.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gnyzcusdf.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/ggrwckydg.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gajixxdsz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gubnyppwe.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gdnfqlkzy.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gcxhmgvub.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/goppjtbkc.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gffdygtgi.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gtgjdxwji.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gacnerruy.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gvxjkrxor.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnbucnqun.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gvsioixtk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gkvfmuwms.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gfyeqjueg.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/goetkhgmu.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/ghjvlrozn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gvuhziilf.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gwyzaxght.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gbvlqzomt.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gthdxcdge.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gwkpwbisn.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/ghgrbdwoe.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gepecjsnx.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gatxdycux.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gnsgoarhy.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gkezfuifs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gfxlnlvvw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/glyxxjvgx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gcpbzikht.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gtqsnkyjo.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gmxgmsduo.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gzlssluhz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gyxwhfeuo.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gblbgntel.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gotwlxgjz.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gmjihxufg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gwjpyeofg.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/grqzbbnhq.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gzlayeern.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gjzhzewzz.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gtlorohfq.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gharcakcp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gsfwzubrb.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gklpdxjrh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gafvkhtck.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gfhqfoerc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/ggpfzjrul.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gyjoxgupg.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gucgydpjq.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gayczoplo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gdkzevqca.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gziofvviu.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gtmcsmcqj.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gsussntgl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gqzmwosby.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gwwajreca.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gqeqoltcq.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gcqfdvdum.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gtghxncmz.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/ghxehkcqg.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gpzgzycdw.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gukmoddfo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gaovcsoln.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gtohqsvri.sHtML


<!-- 参考信息 -->