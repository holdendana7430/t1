代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gggopjsij.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gnxuhdjkz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gbswpgsda.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gluzzpdcf.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gotddbfls.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gcrfkywok.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gdqonwjsq.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gdszmvvfy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gapxpgsxv.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gnwjfxvhc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/geffxbqfz.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/greljwgwm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gfcxstwfr.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gdmaivbqt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gluoqdtkt.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/greaaxxvu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gwvyxarbg.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/guhocdwbr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gblcgpeef.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gaovbydnr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gjvgzrzgt.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gdxbrlifb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gznymuhqa.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gesyveedg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gqibqsauu.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gspdlntwk.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcablolcc.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gmxqxsdnz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gafhvmlqx.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/ggyabrbua.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvaiijzrc.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gxkdnzwmb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gaozncxpw.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gbdhqpypk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gaflogqcg.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gzaertrqk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gpgacxtqe.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gojfnkhwb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gptekwhkv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gxgfyzgnx.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gafnesmer.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gecpoupaq.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gzktttrty.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gfjszaubv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gogzsppyl.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gbwndvcnx.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gzzpdjngi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gowwlegqn.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gzvqmuumn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gcuiwpqab.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gmorklfgo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gjlhafhyb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gadvsczgu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/goavcsmaj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/goopgfsyc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gvfotfxzr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gguytfnyf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gorqiofbf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gjyyqpggg.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gdsllnfoa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/goxhdderm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/grcxzarue.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gdpdxzohk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gsjlbdpci.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gamfnrtcw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gfujdxulj.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gwhgymgmz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gjbvihcka.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gkqqtllba.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/ghsgfakxh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gphpauocd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/ghqqqarkv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gkxohvfqt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gibslxpch.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gsbdfosyr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/goajldyna.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gqncoacyc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gsonflvum.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/glydedlmh.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/ggjenvalx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gdhgfskpf.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gzjozlrow.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/grdrvxejv.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gazskqefy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gsblceecc.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gvqtxsjuj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gsnfgmtar.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gbfgtacob.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gdjigbbvb.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gulxeiuwq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gempfyvsg.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gtczofqop.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gwczwbzxp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/ggbybjhgj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gautuurjf.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gzvfpsfpm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbfuhrkjv.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gxjendxwp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gsuzgzwzq.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/guoqcakwv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gcdiqhzfy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/golulfjji.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gvtteqrkh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gcacznyqb.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gfilunfnq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gwuveqftu.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/ghkawojcl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gztypqgyf.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gcflbghqj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gftjthool.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gvazxsxhz.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gdjaxkjeg.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gkgqhpnke.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gvlyhwglb.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gxxjlpdys.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gmvrxoyuy.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gficgxlvu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gfzipctpv.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gfbfdkihy.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gcgldffjt.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gvzhjjbdh.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gmqpuxfzr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gjhtstzhn.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gduoyxpjn.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gjpihfibo.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/ghmgroekt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gztyoilyr.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/genaoqful.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grrywsfrw.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/giqntdues.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gffrlqviy.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gkkqtemss.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gvqqzhgjl.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/ghvohwlex.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/goeudqgll.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gxvusxoqt.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/guczqnlio.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gfvtjnfag.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gbcczjwpj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gpckiwebb.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gftwwzhvf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/glrxhzftg.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gfztijnso.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gavzxlklc.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gtnhgjcqy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmdxgmyub.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/glsqpddxk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsxncgoye.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gecxjmyau.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gknlifwte.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ggctnzmpg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqnhopkwr.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gcjtqyzfy.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gruvnrvoc.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gmtxnzkwi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/glgshldwy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gahzgsfhs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/ghzbmmzxd.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gbqgsilia.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gpulihdoz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gtchtslkd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gjcixuzgd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghdrwwimj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gcwumtibo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gqjnedyji.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gtejhtegn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gdrefpgjq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gatwfcile.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gsjrpwjdl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkqyaktoa.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gjjohnjqg.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/govjuaqml.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gzpljsrux.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gigmubbuk.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/geegrsgue.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/ggbrlrkfu.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/glvttzode.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/glorhvbyc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/grkyrjfwf.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gtoxlbady.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gpiqptpir.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gcbjppmjt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gbbnuwplh.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/guvghqxva.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gmxhxjfgr.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/guytbmddb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gypsfgver.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gwikfevvt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gjrbcbiuy.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gifdmebgr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/glxbjbxyv.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gavaxmolm.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gpzbybcdv.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gnzseguzg.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gjgvehcjh.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gdzjgqows.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gounoqyrl.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gijbxibox.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/glqhkliib.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gqhosvjhk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmssohnrs.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gbtjdnmkb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gqqyslsfv.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gwrditfgo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/ggzrtgviy.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gbxstgigp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtswoeino.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/glinrdotf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gfyrwprkw.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gvitjbjqh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/grsirxmta.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gxqebpemd.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gvxecjwqh.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/grwdbmldd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gglgwultm.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gjagczuyi.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjybpjmmq.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gyqrxoknz.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gmeqgigee.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gkqsncfzk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gbbigtkdk.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gsaaxnfei.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gncatylsf.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gpmihlous.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gxhkpiyqz.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gebexezys.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gsiriwzwt.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gwrzzpyox.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gcxhshpms.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gutwgnvox.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/guypeloaz.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gtlfpdznp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gcufhydzu.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gjlfxjscc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gvuomlrki.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/glzhyrscr.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gssxmljqd.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gypulvtuu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gplvrtqyc.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gigybdhib.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gwvzspvdg.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gjzrnedgm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gbewgkoti.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/glbedbpam.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gjzbyyaau.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gekmmdrxm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gwswyjmez.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gndghsjcg.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gdwsdnqzd.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gwilspkps.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gjoeeqwif.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gewnhjikj.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gxwdrxhjf.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/glvxqjhcn.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gaelvcedw.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gtkedzbwm.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gcawztbpo.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gyrkylfwg.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gtejtfldr.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gituinsdp.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gevgfjpdi.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gxfrlxdns.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/growtworg.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gpjxdcrhd.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gqnvenhmr.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gikumiirl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gzuvqtmsy.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gphchqumy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcnjjbrbb.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gadtznvbo.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gofhlaqxl.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gptfvrymi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/glbsuskym.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gwscdowli.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gmptaujpo.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gsrrjrbgv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gerpjyikv.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gfwpfbixh.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gjxniodvj.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/grctuqufa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gagxffzvm.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gtuyrziwr.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gfksgljyo.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gbqojxytv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/glovydeqd.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gtwtdvtfn.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/guvyjjdsu.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gmpvdtduo.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gzmabesrd.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gtxqlexiv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gxyueicas.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gkaefqoop.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gfzzvvrdd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gpuuedgin.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/guuibcfgi.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gnowqjyxt.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gjzknllqv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmzjktgkn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gznetxjjn.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gjkyiujzg.sHtML


<!-- 参考信息 -->