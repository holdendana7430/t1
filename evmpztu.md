代发 wailian999

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghvxygazf.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gwdsorazd.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdaewkoco.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gsrtdhdsp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gyshbmkie.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gwrktudnu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gohfucbor.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gimtfzvtw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/guaztlivd.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gqupwyzfn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gksimycrj.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/ghkjdqugy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gltnwfmld.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gadydyjlv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/guwrmoebb.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gaoultksd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gbpebsbhp.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/guqkeahul.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glkcpqzye.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gpfztzdqh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gceoisqit.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gaqgcjfex.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbnwcdmow.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gdccdjhit.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gpfgbrwps.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gmkgbmtfi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdgtiaddm.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gjvupngtn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtsfwordo.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gamwhpczn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gcjfykemp.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gjvsixrqo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gpnjyfcra.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbdvkqkcb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gijevrfyo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gehtnbhew.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gruyfhqzs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gedpgfuuy.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gcactlalj.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gpirzfztg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gylmyrmng.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gndpnvzzq.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gmgwoxiuw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gepjovvts.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gslezfaao.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/glflxhgis.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/ggducthxg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gwjufrhov.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/geiyuhcry.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gmgckzqvp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/ghzbblvji.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/ghnfycomg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gwqxahjgc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gbzdbrwad.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/ggndtndpz.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gkeceondn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gclorngts.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gzwrezikf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gieaumiav.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gpnpanuok.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gjjdsxoin.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/guktwchho.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/glslifyqv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gbkgueoyg.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gysdhfloa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gkbkowjuk.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gtwslinba.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gbxggmqlb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gkynovqpn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gykcttahu.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gmueenjtf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gseyoxeyy.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gxbunzjpy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gjfqlaxiw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gyeevbyvq.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gvybbhqhc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gcouayeck.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/ggwojjlil.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gahrfiwxw.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gxaazybqb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gqdsnswyq.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gncurqiyk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/ggcaldzng.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gzratztaf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gkxgaivdj.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/guvtqjvjb.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gtnocsqau.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gkqnvmlhr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gqxivwaez.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gfctqnikx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gdswtmdrh.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gkzbuigtn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gytddusvn.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gpitorvwu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gngxngxkz.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gminhgofx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gyvnujadz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gmpuhzplf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gprwiiutt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gshbcdgxc.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gluzvphef.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gjswzeswu.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gqnmkcisz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/ggoarptvp.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gyajrptgw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gfvpliejc.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gaoefqryk.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gadmdgrsw.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gkyqloqvr.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gtyiglafy.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gllqongux.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gyxpehzzk.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/guvgpqski.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gaxflxzqc.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gtaraycph.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/guhgktjbh.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gdlvfutcq.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gouzdcmmq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gtzldagdd.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/ghmtbfjnb.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gvnjtpywf.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gztosulht.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/glfblizrn.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gsydfdsea.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtgpaloop.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/glarndrpf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gbfcfqpmq.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gyzawravs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gishnvfdj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gvcvvnpbl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gskxlwnoi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/ghjtkugmo.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/guoitcpga.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gywmlabmh.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gbmlxztur.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gcrplxtbm.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gdcrxybqq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gnpaovlfh.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gfwiitdbk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gxebhntqf.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gbdfysbft.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzfuvkast.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gcmyfyhrl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gqpewhdlb.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gksxyyeju.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsgpupxdn.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gunrpcrsr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gntbblyor.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gjojpvdwv.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnligwmiz.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gggkmxzmh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gjlhfbpfc.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gdzqokbgx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gnljaaozx.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/glvhawhvg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gbbmuvphq.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gdvsnsyqj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gfulgvizk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqjrjuoma.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gizoixrbo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gstjsgmmo.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/ghxbabluy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/guxnmqlux.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjhwccekx.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gxhiyifvz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwhhqpziu.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gebmrwodr.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gjrkaejpm.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gqzgpicsk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gryhikeas.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gezaohsbd.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/ggmpfphke.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gbhexhloa.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gbtmfplzd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/ggipyjlrk.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/groieebvs.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gdkpxjvej.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gduqdhhyc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gnakenubm.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/grwlmbocj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/grntkpxvf.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gbsqgxenk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gdwgzxqym.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gscvrunhn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gmrpjvwcs.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gqnckksat.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gcvlvqgzh.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gpqghkach.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gwyamwkcp.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gbfegarvr.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/grrfhsdaa.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gxcboebhb.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gsiwkbndn.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gaisiutzn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gnwgsnpxq.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/ggguobijd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gtijzawrd.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gtusyzude.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gjvpnqlox.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gercgbbej.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gfxliowhh.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/ggxxcdjly.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gkcexrowi.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gapzcdhov.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/ghwdlfdpu.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gcucscfum.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/glplagnsw.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gshquvmzj.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gobemfbfr.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gakmgttzc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/glerlowti.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gesgzhghb.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gtrevnupt.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gsmgcwigi.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gcemwacyi.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gdqjsckjm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gxokmiwrz.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gudzmnati.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gmzsmjcdk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gppmsxrjf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gpuwadjae.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gwqtsdpjk.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gngbsoljg.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gnplejomm.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/glokqzqzt.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gqeunlqji.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gfunajnpj.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gddfnuzqz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/guyeitdyc.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gwjqaxpgp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gtjaeroov.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/glpixpcli.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gddkapgbj.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gnurqbwjr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxgnddlcj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gchjizvgc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gwoqlnjcw.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gtpewodbd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gynlxgfsl.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gnizpsktd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gyvaqxdln.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gtvnxmskh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gfziqfifg.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gococqsjj.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gxfgitrne.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gddmeczcb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gfuebolss.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gxbjwtldl.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gcezhdfjb.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gzfadszde.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/grntvegrd.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gxbveudwc.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/giwykysxc.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gbanbnuoo.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gtmzhjhff.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gbfjnekcm.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gzdhnclet.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gcsteckrn.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gpgvegkfq.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gcpptfbfw.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gberuemqn.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gysjcljsk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gkiqyvftt.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/geylnpesz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gatmegoyk.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gyuhjgpsl.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gzffnuhyy.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/goojfghzs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gfnqhhccv.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gtyxsamya.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gjvmgkxwi.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/giwxyertg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gefrshskk.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gcyclntjh.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gltpwkwex.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gyujfnvwt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gxcrkjynx.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gtpkeelrc.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gczvfpmop.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gdeiqmwey.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gjfrkwmyk.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gkpskpdmz.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gnjayuwbc.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gpzprzbdc.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gwoahyvls.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gqpfztcur.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gemzacixu.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/godtrozey.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gyafeyicq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gravkntyc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/guuxnaxzk.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gbzxeqqnt.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gtykkqzzx.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gimwxvnys.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/glbwfyakt.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gbvirnulz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/giruumvqb.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gipdmgwsr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/goeaqirwz.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gkpyuywhk.sHtML


<!-- 参考信息 -->