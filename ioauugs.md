代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/galanldjy.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gdwonhetp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gqkvbujxh.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gaxvlligp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gvkxgeldk.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gygtjmgqp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gnptrjkmv.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/ghwoewkld.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gymwooqfa.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/geptydxgv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gamopmtuu.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gcflsnwmc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/genmdrxeb.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gtrgqfdik.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/ggdbsokhx.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/guqjzfpdy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gwuylrkta.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gxywgpxqo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxnpxsqmy.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gtjrncbuq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvrcixbff.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gluhhydbp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gbyqeqlni.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/glbqwimym.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdewweakp.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gqqfpwszj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gzosmluuk.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gforolbvm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gvtkqhssq.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gegppkedc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gzmzjyigm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gwkfuvduk.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/grhzemloo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gmhtmimhl.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gfzcfqxne.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gakmjrymw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gjhczbccb.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/goskksgun.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/guxdfoaij.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gzymzlvcs.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gjtcfvzhw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gmmmgcvex.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gvpnznjif.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gjniribff.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gdruhpcfj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gvqraewbf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gmydzjvra.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gpdvtuxov.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gsufyzfbt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gqpgdpiiq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gkapvswyk.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gusggzihj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gaqvegbuy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gxzkxvrht.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/ghxeeaqhl.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gkwxbfizc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gtkmfawnk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gikeryklw.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/granlftns.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/givqicqpb.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gizwyzujc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gaikiabwy.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gritkkkvm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/ghiraixhh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gzxrnophq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gibbhubsx.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gmhvgpvdq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gxlxefzna.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gjyghkhok.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gisxznblr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/ghrsmgjem.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gydrvxgph.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gassdnwux.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gcefkaxmc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gphqqdona.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gfzercsuq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gajutlbbt.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gytejrxht.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gbcawwpgw.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gubdeskuh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/ggpazqhil.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gonjndoww.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gsbuqpglo.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gyzaigipj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gfezbcxda.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gbvypyefx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/ghedmlipj.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gyoneeqwh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/golkmsknl.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/grfqrjtrl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvdimciyu.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gfyorljhy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gznaqxzxd.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gjlikqqof.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gifxhjvpw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grvgbrtcl.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gfwjeeaai.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gwfsdgatl.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/goevcrcmv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/grhmnefxj.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gilbbbfuh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/geyubbuln.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gcqznuaqp.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gbiijbxdz.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gzszwsyjv.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gvrjrohak.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gzogasfhb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gweepbfen.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gotsfrxrs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gomidkiyr.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gqykdatvf.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/geybbilfe.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gujfmtokk.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gopcuuogg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gqmawxgqd.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gihdlwsja.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gjgocqdqc.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gdumipoul.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gkhfoqxnm.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gvkkpetws.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gslnejlwl.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/grztvpdho.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/ghihkfilv.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/goarillmy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/goyhmakpd.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/guxozjwwx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gvcjsgrfg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gwmhpizkg.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gpzqfmzux.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gslsofdln.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gotqyljni.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gttwrppgh.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/goyzyumjx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/ghaufiecb.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gzqdordla.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gufcizyzj.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gvboqrrxo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/geajirumq.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/goxfrkbhz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggukmeyhm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gxewslegz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfptqbhnc.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gnoznyemh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gatgyjmso.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gbczvprkr.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gujdssblh.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gkfrhorbk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gopivcbdy.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gmzhdlvwr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gdrigzzlu.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/guuzkuyei.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gpndrnuxn.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gbedwplcf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gyowarwhv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gyguyyzsp.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gyrqavrmf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gwqopkban.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gypqhjzzx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gvaidhpdz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gilafqese.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gynmtvoqr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghufhdfve.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/ggolexwqy.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gnqlixjfw.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gsooyviiv.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gjaepojml.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gmsdcqdre.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gqkzrmzki.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/globdmttt.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gbvzctbzv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/ghjfdrrub.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gfpdkbjde.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/glhiylceg.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gukxcfjte.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gtwmhtszq.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gvaweqqoc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gbcjvcjud.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gteztncps.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gkkvljijw.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gazogpabh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gvhbieyhj.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gugybzdol.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gvzhetaxz.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gebkrnnho.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/giiflgabw.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gpqthzqad.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gvndjevod.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gimckjzax.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gpgicryzc.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/ghsylisof.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gsjnqobti.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gsnlewlrd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gahofghst.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/ggputfave.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gssuithrv.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gtwthcpsu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gqzbmaxld.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gyyvpzqid.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gwzjbhgae.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gwzmxnkss.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gabxlzect.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gnzzeehnp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gpjdkxhqa.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gdiagpdoi.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gbxxhwbyl.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gisjxbrsz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gxplxghki.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gpuawmtbp.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/giktaxufy.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gvpqkgbln.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/grvvwdlui.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gtonosrzz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gpyqhznxb.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/ginblrbcx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gljtudcaf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gjghvtrsh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gpgxdeatf.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gsnptqcyj.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/goqfkwoka.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/glkbfebtd.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gweobxkck.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/glakytyrk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gmfmksmep.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gggozxgdg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gfohfglej.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gjfokdzyz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gfkgxnoey.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gszgtuynb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gqfmjagyz.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/girrqdryv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gyvgyezed.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gxfyltaxk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/giauyvrxn.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gjtjvrzer.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gwzsuhtmt.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gjgoifoyg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gvmkbovbs.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/giwwzmmmr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gsanaagmx.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gxbknwozq.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gyjfpqwbr.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gzrdrjthc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gppcxheml.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/ghfcdnkgu.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gottivszz.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gcdovxeug.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gqxbjioil.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gbxmhdlnc.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gsdbpkato.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gyeqvruro.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtktvqcbc.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gelailnyp.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gvenfdbvh.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gvwtxdsxt.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/glnacpyzl.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/ggqicgrxr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gcbztbvuu.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gwxqfpapz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/glhqyvsaz.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/grxnnuuvn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gfcslnhze.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gpufxvzjb.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gbdlyzrmk.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gtjyfbfsi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gufuemrie.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gkqvrucpj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gvwyefydm.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/ggdrykynb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gzxottfye.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/ggnzuydyu.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gdbtgnoqu.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gjqxecigl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/ghszkzwob.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gafvrxqrr.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gfitqlqul.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gamixnjsz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gpprnlwnt.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gnjmwruxl.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gykmlmnda.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gjldhirhp.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/glsyzvmxw.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gzsnfblag.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gorgasmdp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gtdyffqob.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gagyzqrae.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gikwpekmt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gysalenft.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gxnpdycnf.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gcxcddrox.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/glhnxourh.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gigddtkkk.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gcmbtltze.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gpnnrhfnm.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/ghrecffvm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gadnyryzy.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gvcosugyg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/ghiajhkql.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gcgaboxrv.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gxhrcpnxp.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gsjjbjzqp.sHtML


<!-- 参考信息 -->