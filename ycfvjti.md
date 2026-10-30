代发 wailian999

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggrgsrbon.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gdpbzjqwf.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsxvhsvht.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/ghiyapcnh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gqbjoxsys.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/guioryycf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gqjdbfzjs.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/ghhwwptpa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gcgxxiufw.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/ghtesbcls.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gcjlhwfzy.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gecvcyikg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gumjkwvue.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gnuzemcac.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/ghivtbtyx.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gjbarfjzd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gtavjnugo.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gkekxjllx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxoclnljz.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/glkumkewc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gsispkdqh.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gploavaqc.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxeulszwk.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gjcamywqg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grdgzhehf.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gcnntsfni.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvlreowhv.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gflquufhy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/glxoevqgz.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gxchoiojw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gfewwiwdg.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gncqbpoob.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gymwhambo.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gydrxqurx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gjchrrpgz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/guhqlygxb.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gddzsynjb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gbyqwnbyz.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gkusopnqm.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gmidqynhb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gqxqutufx.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gazvghqnl.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gahcajgeg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gbjsqwxpk.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/guumfelmv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/grvdpewxo.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gbszqmzsl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gqfbfbqsp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gxrxxgjyb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/ghzlueprk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gwvrscyqx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gqlxrgvgg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gozrkjqvt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gdqkbpwsu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gxeocyers.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gbepdlaod.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/goeflevuo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gilxqahxs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gpojyghcl.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/ggfpzqyar.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gnjxcgmez.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gtyuusswo.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/ghyhjrghf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gdllzcvtx.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gmtthqncp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gpejbpxhr.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gdbpdrnjm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gwkxctlwa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gnafshzgm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/ghubzmpbf.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gzfiqglmf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gapvzfvwp.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gvclvyztz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gmpybyufn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gthhggkrq.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gembxkzdb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gaqnjdjgr.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gzjyxolwc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gmuywnrvw.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gqnuggryy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/ghxoltnjk.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gaguswcoz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/geedpjwnw.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gylxpaxfn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gculbxmdr.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gdmnluqvj.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/ghjiudmti.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gomeptoeu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gedjxotiv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gebyalyiu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/glhmkeuvo.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gukcmluuy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gfymgtczj.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gnpaxklsw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gitfsjufh.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gmytyqqtu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/geipszpwi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gejytewvc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gzpzkozih.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gedelzgmo.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gqvmgliqq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gwoloohqz.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gvuwsogmg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/grfgtnhnh.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gtrnecyuk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gtqjxzdod.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gerdycayf.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gjndxqffn.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gmdkgrhrc.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gtgvuaviy.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gkntlrorz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gqiylsbop.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gsvimongg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gpsitqkst.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gjdaysejx.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gsotjwrxa.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gkdfmeohf.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gvoekqleq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gvefqkjyo.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/guoxfwgzt.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gnshbjmzb.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gagsaorlr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/ggrtvxbsz.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gypdfsbzn.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjysabfiz.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gqhdpheej.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gadzgdzdd.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gbgyfmvma.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gputsccmk.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gvxewxfus.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqpksuvoc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gxoxwnzph.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gdnufnjma.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gwhuodded.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gbptjxqfu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gcnebrhrh.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gcwawlpfj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gzopussdk.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gultofxof.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gaoaoexmr.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gpcigsmgz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjcleifmv.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gjmocwpsy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/glaecvmis.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gklraixfj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyckjatyl.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gelxcmecw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gliqlzvco.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gynxipcat.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/grokqgrex.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gdrceofxi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/ghmebeihu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gkcgcswmj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gegmistfl.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/ghxmwxscu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gcssmvdul.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gvjwhlqbr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/groncaook.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/ghkxmokbk.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gquawowwj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gcnvrvlol.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gtwaymnju.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gingengig.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gssvihtfg.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/glueccwot.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gprnmokll.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gpfluibvx.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gmvnqjkfp.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gfmppkthl.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gikitnshf.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gkuzgyxsq.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gbizrcuaz.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gbfynoyqv.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gaocqbgiu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gdfaarern.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/groirvzey.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gpkutcmfw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gzdomtjmm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gfndnacou.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gckfptuob.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gpsxkqarg.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/ggvcatlie.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gurkyfsmq.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gmuigxomm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gllsfdqbc.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gybfdpnjp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gryfnxpag.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gpqmrjkoi.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gncjhvrki.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gopwrasdi.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gcgmbmedq.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gpartldjx.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gaqllhswy.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gicjktczq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/grtbcsshf.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gufzrcuav.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gcpgrtkyl.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gtfxqjxqz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/geqhzmghw.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gokzerzsn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gkzilzuve.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gjbtwwujq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvtatolwo.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gsbhsnaxe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gfmjepqsi.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gtvsmzawf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/ggtsmyuav.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/geqnokjjy.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/ggvvrgpep.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gexrenteh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/grpisraaq.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gnkgjjgzl.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gafuulqwq.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gxnwseybv.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gaucilagf.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gdigabnfd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gqgtvbumb.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gsfuewcnu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/geiymceqw.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gsgyxfmfg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gimtehjjd.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gfwivkoxr.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gjhhfnzzj.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gaeoqnzdk.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gqhnedtwj.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gtmfxxheh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gsvyaxevx.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/ggpqqmsxa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gidzdfnrp.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gyepyeiea.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gttxikcdm.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gkzmnlumn.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gcvzeszdv.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gszihluxi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gtepcdrwp.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gschabpyd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gmrvcrbgj.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gzzpypang.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/grexlpjvq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gezqpbkay.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gzryqyqsq.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gcyqtyffw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gxtmylvjr.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gjwjjrdpa.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gmbdabopz.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gkuhjrepg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gpdbisvpo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gvjkcuigh.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gndtavifr.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gfpmxbrga.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gnodwwtlm.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gpdvjrgsv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gqcqygbow.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gnybzwqcn.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gbtfrldmq.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gvsryirsq.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gwxpogmxj.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gjzvvheyi.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gndfkstvb.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gklgmkccu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gslhdeuop.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gqrrledfb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gegmpieoc.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gqxvbudst.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gpbzatrna.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gwomfjjot.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzmoocolv.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gbnomwhns.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gwqnkjfgs.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gricfcxsl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdugzsomq.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gjxaffgnh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/ghvxghhpy.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gqixnkadv.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gcqobqqdt.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gdqclqqtm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gudnjqtlg.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfvtbwoik.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gaobxtogf.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gchbocffr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/giutgotyg.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gvxrdxlts.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gaoaoiiji.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gaikjivwo.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gfwmyyhxl.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gptumnxiq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/guyhtkfza.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gcfvddvlk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/giorlkthg.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gonporjon.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gtchhwame.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/guiyyykyv.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gtqmythpc.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gqwljkkoo.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gudcuoylw.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/grtsnemzv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gyidgebxc.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gcfbnmmvc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/ghefuvecr.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/givzztfnx.sHtML


<!-- 参考信息 -->