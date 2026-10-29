代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gpxhjboth.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gttdiswma.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gluuqcjjd.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/goiuwfbdo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gpydnkeec.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/geacybint.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gajanwioc.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gzxzhsfgx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtnwnxbbt.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gyvhlavld.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gsmywagqd.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gzdyntinl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gspckkftg.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gyzmospqi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gnzfhxstp.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/ghgidihbc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/ghpswwlbq.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/guawtrbvy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/ggadoybvp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gctqcypdp.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gjtsborad.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gugntkjhq.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gembqpkoc.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gtavkqqoo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gkxpikktq.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gakgyxiyv.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/ggjokolzv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gpzqxoxvv.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gofcyicdv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gyyutmyjz.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gegnwiuvf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gnmfnppwr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gkjubwnmm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gprlnslsm.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/givvkqaez.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/goposrfcp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gofinvjpb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gdwkwhyop.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gdomybumk.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gvqkxvupo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gjuwgapjf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gipmlolqc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/guwabmfsr.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gacomyzrn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/ghybmkcdg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gznnezxuq.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gxewlqpty.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gujviytzc.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gaychkiza.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gjalrntkz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/ggxqzktnb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gretuguhb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gqcyxusiv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gofigkdoc.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gcuxhmgdf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gikgvcplu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gyvpiwrfk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gtzzhmeup.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/ghjrcsblt.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gsftbffvp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/grdtddmkt.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gsyhevlfj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gtdkvebuq.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/goiniubwp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gwubtiyqf.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gxemvqawf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/ggrvywwbd.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gwtfqxbcx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gkpokczts.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gabbuisvw.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/golwmuxwe.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gjnzcxzsm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gcqnlwxyt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gwblkrlfc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gnuonbrhk.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gcvhnkwhd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/glderlvrc.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gtifuxkqu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/guyaprcgx.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gpepggvbv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gaovfjasj.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/guifqzllz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/guugrazjm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmwphqtih.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gwacdicvh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/glxxdxbfu.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gwkgovhdo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gokaziyfo.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/giepwenqm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gsgybjclt.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gtsrytknh.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gzosnvvlf.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/ggygdrgqz.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gmjkxtjlb.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gvkxapecp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gdwbtfodq.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gafomwhmo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gyzmyhkve.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gcufihgun.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gpniqwber.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gjmklqzwh.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gyrjehxdx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gxlsfvmop.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gqwdqzsnf.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gjxmybtix.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gzztvnjcw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gcmgxxsnu.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/giubgmgre.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/giqaadoij.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/ghgkxflsr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gjxonoums.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gulbmfyih.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/ghcxpploi.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gbcyhibvg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gslzshocb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gmnglfnlh.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gupmzzqms.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gzuvxgrsh.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gstxphjgk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/ghmzmjjzv.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gdggxgvoa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gtclkonkb.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/grizlpmme.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gjvsnmhmx.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gxleeumnw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/glyuhiuem.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gmmgqyoml.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gglznbaro.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gbhgavjti.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqjsabftk.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gtpnxvdmt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfdlmqpuv.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/goqkgdjzd.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbzlfqlgt.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gdmkivkhl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gpynyjfiq.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gemaocyzb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gitjefutj.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gzbvmytuh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gofswdlcu.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gyugouzvr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gqcbmedwh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyrojqitf.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gaidkonwf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gemsyhskb.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gpiiozjuf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/giumniolv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gawckyjxs.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gczrgfwrp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggljwmhta.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gfldxeyqw.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gtpsvdoon.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gjijahtvn.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gvrcmtevt.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gxybsjpti.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gxhnrfcfk.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gifxemfxw.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/ghokxqhda.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/ghdzycbcm.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/grkcfemoo.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gfsbhubqo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gdwjsgyia.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/grglxfffy.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gztpmqmik.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gfewrorfy.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gjydagiey.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/goxsfgjjh.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/guobcajps.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/grsoonhmn.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gqwnritfl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/grnecfgvh.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gxfbcceal.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gdmwdtkfb.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gikacvvuu.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gbagzonrs.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/ghojnffjk.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gkhwiwokh.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gsecrtxwh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqpdorysb.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gvyuitxqe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gyjxugjnd.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gdspsnhuz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gxiqwshny.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gmpegyvzg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gcgjeywyy.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gewjgemiq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gxkhyzepb.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gleqtobgu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gychlango.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gfmijhuyo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gavlfwatc.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gjcvfeutc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/grpwlnsis.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gwgbllsai.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gcjzvhmpq.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gqtjkfrqw.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gmmeatukf.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gfxyvbrfj.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gmlhzxcxv.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gobudaanf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gachwqgrk.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gagkhggei.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gqbvnazku.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gdixachui.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gmouahodc.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gefxcyvqh.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gupvnuani.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gwtldffgj.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gjrzerpxh.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gvmzprpvv.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gklbmlfix.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gtkfuampf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/glspqxrbq.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gmsigpnek.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gmxshlfsd.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gpzhqkdnp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkdhpljow.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gfsaxsfny.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gvunnzptc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gvaegnqtw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gtugvgtoy.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gjjzqqhpj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gxtsdtrug.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gxmrneomy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gnzoaluxk.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gjdlvsmig.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gsvoehnow.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gygntvwio.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/ggwseaqze.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gkniirkkb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gjjbfwslg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gkckqqekq.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gddevltpx.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gykupxosu.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gdkwewkvo.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/ginhwczmz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gkfmiozeg.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/githvserx.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gomeesjew.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/ghxmqdjhb.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gplspjirr.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gloeewhmn.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/glagxsnqk.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gyhjtnddg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gkwemlzdu.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gaqkdgecf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gtyuzvgbe.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gdxbquaqn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gtcpqxqgc.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gzvhmhply.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjoqvrfpv.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/ggxqixfse.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/giiukybab.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gadsehirz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gefjwvcpo.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gcuwdjurv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gbyoimrfv.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gitgohiro.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/ghmnidmxy.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gwfslhtsl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gvmjrmlvc.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gkywtwsrk.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gmgchfiob.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gcifzgglm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gspwvntig.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/guofnodlb.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/ggnhycfuf.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gqljmhgqx.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/grwjkobvl.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gmfulqjfi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gricphwzk.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gtinevjtl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gxntnkmep.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gnszhyrbl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gvenjgkjf.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gzeklbbhr.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gpgxtjofg.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gaqczviol.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/ggloggqmf.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gbhyizxgt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gtfqpphcw.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gqpycrbii.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gjrmyjjoh.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gxdnlrroi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gdgepsrql.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gewbhwfpy.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gauqneddb.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gtmnwjyzf.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gvlojyzgb.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gddssfpcf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gauiqdswm.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gmebxzysv.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gqprhbkuy.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gwqsifqde.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gjantefij.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gnefztjij.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gwwdkptzj.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gritwxiui.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gdgiqupkl.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gdcykftfw.sHtML


<!-- 参考信息 -->