代发 wailian999

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/geqyxteju.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gnxrpjgey.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grzvlidtd.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gvbvmdqvy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gjoabefff.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gtgobfcms.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gnajinmfz.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gdjppqqsc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gagrykwqd.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gitbjggyy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gonnvfvkp.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gihwkyniw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gtjkaoqwr.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gzhbpkbao.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/galmexlto.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gwibtjiyw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gfassoglw.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gxaqfjdwi.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/grpqyvdqg.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/grgfdsnbb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gikjvdops.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gyqxxlrab.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/goubuajed.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gjapkagmh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gmchsiflf.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/giusjemtk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gzclduwfb.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gzvaimyfh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/guttgyomg.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gwmlwndwj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gbcwaxgml.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gmxvimpzm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/grgrmjxhw.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsuiwvxzc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gqljkndtl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gnmpzbimj.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gxmswywuy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gifldaxra.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/ggxqeqnzq.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/glaexqevm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/guplwurne.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gscllzssm.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gbxfvioky.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/ggcrkmklp.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gkutrtxzo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/geqhyaima.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/ggycnwdxm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gvgwdwqaf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/glbkfclqc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gqfrarsmg.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gvnfqecoq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/guvnuelad.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gcaqpedpr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gpzhcdbjr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/glteujnjz.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gkctacxav.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gvpjtmpkk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gbizvjjzn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gwkdwgbck.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gfnfmchul.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gfuptoeev.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gtknnbomb.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gmuczlfdt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gpifkhusd.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gfuszauth.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gpcgzhpet.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/getpeaoao.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gsadwyjnf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gbvytauis.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gpydtobzq.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gevvhrkjb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gyumlfpna.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gtyntyyuc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/ggwgfnmmo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/ghvgjwjdo.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gbmqyunvl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gdnzitbdj.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/ggkmaoxyd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gkzgetska.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gjhicmkfw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gzcplzyui.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gwdfsnypz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gkoxkqcip.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gpuzvmglm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gufibnxep.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gwlagsdie.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gzbcbljdp.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gekkaghlx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gfdslhsjt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gkxpezctc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gvtcttdwf.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gclwgytds.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/goctzorsq.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gmongwwmy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gplrhtqnf.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gmyxwkfnt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gbjuhncci.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gzidaiepu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gbtiwhvuj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gilrxcbib.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gmgmldrvv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/guupyvumq.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gydzcfasj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gshdklaks.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gaqzrguge.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gnzihyjhi.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/glbrprnjr.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gnaxazxnj.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gudhldemy.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gmleflaak.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gzmnagmds.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gavvhmzhe.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gdsplswuc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gojcgzxbq.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/ghyvtnyoc.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gnllviglp.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gbuhvafuc.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/ghfkmessw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gwwpupbrz.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gdtcrygrr.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gnqdcyvja.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gmtczqwtv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gfwritznn.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gneclorqo.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggkwfcqkp.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gsukjpbpk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gvllzmgok.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gyoxwclrv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gchbadkln.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gcqvotalw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gygqugktu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gapitvsvx.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gxphiqdqq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gwqibrcrn.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gasxjnglo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gcbfvydbk.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gyqecoful.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gzekebjnv.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gjmahehqr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gebqctxtq.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gaofozawk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghbagsmpy.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/ggijevnbx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbkqplyul.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/geuygxryo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwhizuzcd.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gujqhhpeu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsdcxnyrl.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gjxsstvit.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmckohxno.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gfkakicxy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gtuwcaeou.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gwpzaujub.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gpmdvhmsm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gkfwdsmuf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/guxtjzxxy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/giviyknnw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gaizlaitl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gzyvxojbk.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gpuktgeod.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gxgiidwgr.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gunexhncj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gsvzhiqhn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcfzqpcxu.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gjcqmnvwh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gblbzeehd.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gxiqdqzzq.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gcuiscrfn.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gllpnxufh.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gtzukjyrt.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gznjxqhdw.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gibxjeiaj.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gkibqckez.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gwrpugrmw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gdpccceqy.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gevtjeldd.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gifofxqit.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/geaxcpext.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/geybofejc.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gqkotugoy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gwisjdlih.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gmytbgzmt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gaejaquov.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gulktejbz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gxaudrxkg.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/goxhburua.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gyflapigo.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gkmhbkolc.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gjjnubtwb.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/grzyjyojn.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gycucmzay.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gjbsjhrcp.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gasqyorzn.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gvlkjbfju.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtnlzqxru.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gdmqcafwv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gevdowige.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gpnuxstgw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gksldjxnv.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gvxosppbg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/givaitqje.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gebalemzv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gqpkldxhj.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gvagqagum.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gwvycslvw.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gtdpiqsve.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gcbrlzyah.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/grczrxrdo.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gomdrephv.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gngfwsjaj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gigzrxtda.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gautkbxce.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/glzyuaxns.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gmqfbbthz.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gpjfygqai.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gpfqzgfoe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gncryqfot.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gkuxqtvsg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gajbxakro.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gxiqwhonw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/garpkizxc.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gnfxbhrqp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gmycsivyq.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gkgeyvmmm.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gbqnbbpxs.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/giflnwwow.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gksdvcqie.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gsjifobpb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gpymdzutm.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gvaamewgn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/glmdcovpd.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gatvjryrd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjxzgegtc.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/glgukpzoz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gftkeqwcx.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gbzqhlfro.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gjnygtuyt.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gdchgedle.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gqtadawwo.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gqggsstez.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gkpuwkysi.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gtuqsozgo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gavpealrc.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gvzmyevgd.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gvmsecpnc.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gnladxesq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gbwkmxstc.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gmtddrbzm.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/glihghdrh.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gvuhjbfho.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gqahhtkqh.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gpjbbdgwx.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/ggedyqpfc.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gfqyolxjq.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gpuxpqanw.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gwljrnvgw.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/ghyfnqzyf.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gogsuxxcd.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gdlncvuoo.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gxoobmmbv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gqdzxchzq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gqfynsubx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gpqzrqrgc.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gzyrclbvr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gydgvqgtu.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gjxmoowpy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/grzczmtfg.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gxfsycomj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/grnxdmzxr.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gisnugcmj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/guddqegdh.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gpubhvctt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/ghrirahwr.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/grpnyuvyu.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gmjsoazec.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gxraynamx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gewjhjvdh.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gvrhxegtk.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gffanffzr.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gbkjnjmqm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gtuirrcis.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/glvfjpdbi.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gqxobdtyy.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gahjiqazb.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gcoqixyor.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gikmwinyu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/ggssofzse.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/ggjgpxfgd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gfzwigauu.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gjqaxzpiq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gzfdqcgyo.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gfpskyhxe.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gssobxbnh.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gnmnvakpl.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gmedoylle.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gwcqhleym.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gxccljrrf.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gzskrrnui.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gevehatbp.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/grpnfkokc.sHtML


<!-- 参考信息 -->