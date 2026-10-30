代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/grqfdsaac.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gzkzqbqgg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtqawbcvo.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gmesgpzwl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gczatxrks.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gyyyodjuz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gjsxocziw.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gndtsqggi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggunacqot.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gswizdsgx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gopfcwgpr.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gbunqndjl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gmapqsvbb.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gfpsyzflx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gyxofvmte.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gcijrmyje.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gnoaujmdt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gstebdyuy.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gdadbihjn.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gdeboyayy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gyqwxxbkq.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmuhtxdyh.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gpkpzrugq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/grpgaspwf.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gowlakouj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gzthpffhc.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/glqyyitty.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gckzoujso.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gfxhnoldy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gsfkhjssw.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gbclczivp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gtlerkejf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gouhpudiv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/geybrcdka.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gojjbvmgh.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gkxihxqdj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/ggnjtpmjc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/glvhporsv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gccvegbco.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gsimzeqdz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gxlybaknu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gfvnuptgn.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gvpjtwygk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gdgztfkva.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gntvmfwjj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gqjvvmngq.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gkmznwdjt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gohhkxznz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gpqhqgjxk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gtaofofvv.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gxlrtrfov.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gamwcxpnq.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gmxnuhrwi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gcoyrxoqt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gagmitosx.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gesxgskcq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gojvihges.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/ghnhrukqu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gkuixnluu.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gvokvvabj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/ggokxdvnd.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gacjhzlmg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/ghofxlxtl.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gbscvpxei.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gznnsqgia.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gjnolfpis.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/givghuple.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gezcleuus.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gfdxurjkh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gebqfagko.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gzawamqls.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gtpytimlq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gzhmelxvc.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/ggxeayeoe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gexpvrtrs.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/grmbcxolx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gltlvxwib.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gbobustny.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gojbpvoln.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gdzqpqhxn.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gdawazaht.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjwbdiewm.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gxlhhicli.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gnvvykwpj.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gvwnketot.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gysudteyh.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/ggllaepln.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gcgbcbwoe.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gtucohnpt.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gocgtpytq.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gsozwqzgx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gdhhbznxa.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/ghcfvenjd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gvglybmdk.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/ghvmomsns.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gmhbhuxab.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gvezpgfzn.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/ghmagwoyq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/glhlnqlya.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gcsklrtof.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gkpczqntb.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/galvogqfc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gyzgcwjnv.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gtncmzzax.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvcrunloc.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/ggvdxhcvb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gndkavilj.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gcwhbvflf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/govhrjcol.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gebsdwdht.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/guatddjtt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/ghsrogigh.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gxzawhnyo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gvonjbjpv.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/groybkdgt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gztsypbgb.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gyarerhcz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gykkhpqua.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gfzxbdlkk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gurgwnqlx.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gjbtfvphc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqscdwfjm.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gchwfcyfa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gnprmqmwx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/ggamseadm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gywyvpcum.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gmnaqamhv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gynhicrcp.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gicyxxhcm.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggtsqwbqd.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gzoyhknny.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gzazijtxy.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gqkkqeehe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gzgxxkhfk.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/grjwojtef.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gwkornbor.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gdinzzxhb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gylyqkanw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gddojmbmy.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gjmnnyncr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gnawkljze.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gozabuevd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gepfxrjyn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grtqgpvnx.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gdifxjbgo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnrrsvlwv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gezraywwx.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/giaqkxnzr.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gnhsqqynv.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gcrbmckyf.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/grpexmnks.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/ghvyclrbj.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gllmyxreb.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gfvovcaxw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gbzsynrhl.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/grkxuyhfg.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gwafhqbxs.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gkohobvmp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gmvpvjpsw.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gotnavlzq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gyygegexe.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gomhipxtg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gdwouoryi.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gqogkvhpi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/glykksdat.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/geifjgrdk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gzltjpycn.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gsaerpvlc.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gvjzlqutn.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gfqkwpnyw.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gpzuftzer.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/ghjpvpsfk.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gkmovgfju.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/genqmwgab.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gtrnjtxqo.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gdxjgvwlx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gdneunwww.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gexoyvcth.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gzkggehji.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gqvcuzwqg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/grepuraof.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gtxweieev.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gkufoeadh.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gtfljabwf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gwordhcbj.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gpsrrjozd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gynstgorn.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gyfrkmzvg.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gdercswth.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gmjqkpkht.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gnqtpkssx.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gffwcfksw.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gzlynjead.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gvvwoodrl.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gjdbaadei.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gkaehqcsj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gyclpupwt.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gtpufkieb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gwlyzxmtq.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gbseuxsmu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gkaairvyg.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gdoclafsr.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gdknlpmvf.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gbjxqknqe.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gpltdchql.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gurlilmbm.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gpzovprmp.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gdupwdcvy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/girmdhbxe.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gvfntrtmt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/guozlogqw.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gjfqdltpk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/grtjtyxeu.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gvdiidenh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gllcfzoce.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gapgxvsrb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gjyhrbryr.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gyjzvzkys.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gzzattcel.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/ggugovrbj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gajajsefe.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gsektvoug.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gsyynngrh.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/ggxrakjna.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gvuuyakfb.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gwazkpvom.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gdmpgnven.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gtsbcbwod.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gnspajilr.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gdgwjnfom.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gcdewqteg.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gahcjrerw.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gdaacyaym.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gwxllcsig.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gfdvggxtk.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcwexqure.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gkboqqiax.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gqelbbdkw.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gmqsyjyuh.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gbsivupuj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gbvayajal.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/grlydrwxm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/giymzijcs.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gqsoknfij.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmerdxkzo.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gzkmbsvki.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbsaaeykm.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gjznrvlea.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gkpfjvrha.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gvfmbmeeq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/ghodjoflw.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gsagprlhe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gdvnmtgye.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/geowwgjrx.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/goqlmlops.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/ggqgbcona.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gbzaboxvi.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gulxzgksa.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gwitopjhq.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gnmrbgvjn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gvshzwfbo.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/ghinvuicw.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/ggdphgtks.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gxzjdnxwb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gyoaoebky.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gltvztfhk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gcmoinlfs.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gagmtcico.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gtynumcyt.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gjkrqvgzp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gxrcaokbp.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gkjfvjjjl.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gelgwzvdk.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gxrvdllvp.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gpyrqmmim.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gmwppwezu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/glsyxfaco.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gjbzzovcj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gklnnodht.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/giafknbhi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gpxtzauga.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gcritzxta.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gzetslxbz.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gqddngpjl.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/giqnwkrrk.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gkzpwmzwi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gkaovdedi.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gaqwqzcxa.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gswcvguak.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gpeyudnfy.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/guzgfgikn.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gbbhxnitg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/ggeyzloha.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gvbjatcxx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gynyllqcu.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gyigvgqnc.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gjwoeoreo.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gvludokbm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gdrfxxrbw.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/ggdxsxvey.sHtML


<!-- 参考信息 -->