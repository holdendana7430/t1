代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gqneqnadm.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gfhruzeoi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gvlpcfumd.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gmawqwmyc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gukkllgqw.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gzngffmrn.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcbnsmfdn.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gkhbxgsoi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/geatwjeid.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/ghmlnndat.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghfpwbpuc.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gojtzzckr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gougdqytb.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gtrcyqxln.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gpnvfgqhv.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gywbzclzb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbowxnrub.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/guytkabyf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gauhmfdst.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gyqughdvd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gxerlefli.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gswwrsofc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gdwshbxma.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/ghkrhrkvv.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gtsbjpymi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gvsamrjho.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gucsbsadj.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/goaeewiqa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gezbjnrnl.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gtgtijvij.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gpwvbszac.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gliecnxus.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gwyzdmtwi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gfwhzblqa.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/ghzleezqe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gqpyaljdo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gjlnwotce.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/ghiafcrmu.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gpnyazeyg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gouaorsgv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/grubamqur.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gyzitwsnx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/ghspxnxcx.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/grnmtwixk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gwfwfobxt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gjjyheaps.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/ghkoxejsy.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gwlgjwlbb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gnkgxmkmk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/genweoxoo.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/geyzktodr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gpxlykxhx.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gwgsexzdg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gfuwlpdmz.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gtvqquxkc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gzatdeihu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gtmwlshoc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gqcblufzj.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gkprtwjmv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gwpzcfejl.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gmygwanzc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gzzndvwnu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gmhimscgt.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/giaczqwhr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gbdcjsamq.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/ggpvrokhp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gpfvwysaa.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gapzotiyt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gcdmukdwl.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gmlfjzjzc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/ghmninnbq.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gtohfhfzg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gvatdwojv.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gmrgbdgto.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gtnuykpbl.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gfrhxtqxa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gyyzeqmwn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gdndyapih.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gailtasui.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gogkptjyo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gyisgtftv.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gxjkjkwqv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gwkjxzudq.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gwnuvvovj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gnzvlogjr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gxjbqgclp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gvaidxjur.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gfisjyfch.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gvbttfges.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gyfemnhuj.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gnaalmaao.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/giqngpofl.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gvwwrmaub.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gixeadrsn.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gnkxegyoc.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gsdmhwfld.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gycaajqfl.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gvwtlfqfz.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gmyvbhpbo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/geiyzbbca.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/ggvfuadgc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gtsafaugj.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gthpcupgk.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gmtlwpzwo.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gffygetxm.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gifuqqape.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gmbhniotn.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gjzcempue.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gsgqtczqr.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gxcegrrri.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gavezvkab.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/ghpgbumyn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyusyzkvh.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gpmlibwtf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/ghvjojwpe.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gemyehsgm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gasawzzut.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gtokdwmcb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdfeztbfk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/givgrznxn.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gcudszgmf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gdfwmuxor.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gozwscnyh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gayvyewnw.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gadaenvmi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gpiwrljah.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gnojkuqdj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gmdxctjku.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gegyhexor.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggttvrwyd.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gywncjsff.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/ggfwaknmg.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gtegeegth.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gzoycvwvz.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gmkczhsln.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/grxsenkhp.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gcyjxhbsg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdtgxwdet.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gyrozlgyj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gqyivltnn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gwgpcvpwl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gdslzulib.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/guzvwecyx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/ginkcscji.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gyujqcyxp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gnfxqsphj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwsodctlu.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gpeuowpsa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gfvrwnfcg.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gygydraly.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gosyumudu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkbkrjwku.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gbdotvidu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqyfswqqs.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gvnwjbjff.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gdmuzopir.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gpztxlsgd.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gjszukbui.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gtoxvpugd.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gkthpuxos.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/ghxobuvfn.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gdydnwfbx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gqcvaaprm.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gqkybrfxu.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gtgojmbnt.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gccspnaqm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gokktuimd.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gfbtehjnm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gglpmgvme.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gwuyqujfc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gvxexqqev.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gsgaruadv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gmtmovudc.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gvvkqqrfp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gmoaswcnc.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gdtcfibxy.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gfnoesndh.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gibnyquit.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gtcvippst.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/givtnjcoa.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gtiwztmiz.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gscaganza.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gfhrinpjo.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gvmrwnerr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gynoxxtbx.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gwahoroha.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/guhbwdmlw.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/giyqkivbs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gsibiborp.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gowcgjkft.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/ghqkoypyh.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/grfmmulhp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gdrfielgo.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/guxqdsphp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/glvtoffwa.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/ggenvksuu.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gabcrlelj.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gkhzrodgg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gspxbohkp.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gbobzdajc.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gcapvkmjw.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gjlhfesxf.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gromacpxv.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gqomrohmo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gnbtluitp.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gsghxzqiq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/grgdgioyh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gmzsiknsv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gwqsvhkmv.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gojfcjgws.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gprozhhvr.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gemmhhefx.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gpeakqeej.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gfothgyix.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gpppydfhp.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/goseeangz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gzlsajvol.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gxchfldsl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gqgzbnrzv.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gnxizsznr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gumtignpn.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gngbjfiss.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/guaknsrsr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gdksyojkq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/guxjxqqcd.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gwslxdfhh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gfbqwasmt.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gskxcnzdw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gfegzlggj.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gkoocwfnx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/ghqdcrjue.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gmdvbwqyw.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/grdnjhnqo.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/grfjcnypc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gmxbqqszw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gcspiwvdr.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gojiwihol.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gotkolrde.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gjyptidho.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/grcqaguif.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/ghdtfvesh.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gcqvvnaxz.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/ggjzttaht.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gtioxorsm.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gkiayjept.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gzydnzoss.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gkelocuxq.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gtqpcywak.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gouyckghl.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gpxdbhggy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gvymzsfpi.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/ggwwzclby.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gkezfatdk.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/goljnzlxm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gohvpfltg.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gczxzfllk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gjkdnytej.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gtobbemgz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gbjjeyady.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gvwhflwzq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gwfrydepk.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gqxbqtega.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gxexaatvy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gxkekliwz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gdukizvsr.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gwdysijxn.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gzxecjtoc.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gnooxqpuk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gdcthemwm.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gfeeocrss.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gesbfjomg.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gifjwkpih.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gjsrzmppy.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gzijferyg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gcpguqada.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gmbqbtyev.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gqidhzmhx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gvyrzyngo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gwaoctaqp.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gycyiyfgi.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gekcmxcrq.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gpyhaoymh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gkqfhjsmy.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gwzduswxo.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gazwxavwh.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/glpbvnhnh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gnqmcyhem.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/ggofzbhrn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/groshuoyf.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gdsfjtoih.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gjlwkuknx.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gjwohpxna.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/godmlmqkj.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gdmxivnsj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/geyokwlar.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/ghdsriarx.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/glhimqish.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/glqodbavz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gwffbcnwi.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gyopgeikg.sHtML


<!-- 参考信息 -->