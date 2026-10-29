代发 wailian999

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gquituvgc.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gegytsflo.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/goadlowjr.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/glzjnwefv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gjmxgfcmc.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gnmztxhoy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/giafbwfeq.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gkgtmmntx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gcgphdhlu.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gufgdaxpg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gtgpjdizf.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gwvtzqzpj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/ginavqwnf.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gvbqdqfir.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/glgoascck.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gkzheapdw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gnwgtynwo.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gapsfolvw.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvdxtnlbs.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gzdnqcwsc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gnqwdiemo.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/ghzudsmxm.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyosthfbu.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gisyljysf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gldzgjqvm.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gldnwqprc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gskeopozz.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gaiftjiyw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmzjucnpa.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gwihmyrtf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gbopdvwdr.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gekbjpqcy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gcysnkffj.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gmdrakhsn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gomcpsxaw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gwqtxrukq.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/ghwnimsqe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gvcpnlzqg.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gbybkendq.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gualsiuzg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gwdtcqpnw.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/grwvjqera.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gxhodrnou.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdqdozvgz.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gmkgkjgxl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gdvzhdens.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gryoerfrf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gbplcmthd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gcvinlioa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gzpfmxbos.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gyowhpojn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/genlvwzpu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gwsjksint.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gozanjkee.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gjhkeyypt.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gipymehbz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gzvjidcnt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gosnwvgri.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gpikgsxgm.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gjmqkuaug.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/ghzhrqzqo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gjgskkpqx.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gkstxjlpn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/glhkkwpdn.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/grjorlcwi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gpnufrhqy.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gtgcdmwcn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gpmeseioj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gqhpbzubs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gixukqzkd.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/geimmbluv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gisfsgstm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/giucjdxbb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gaqncjtgl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gkxnpubpx.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gsiduuirr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/glcztpsjw.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gumejwpxi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gemtknxpi.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gzepauozt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gaosbgvdz.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/goychpire.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gywnycprv.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gwfgvgyzd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gufxwqljs.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gepfkdmzi.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/geeyllaqi.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/ggjpbsbie.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/givmzkegl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gonxnczbu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gtuenxyvq.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/ggwyxvuwz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzlhjhbax.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/ghgkxjtjy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gdhzyxqvs.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/godgpmmrq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ggiacoyat.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gdlqleidw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gnvivdrhx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/guhdxgkzd.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gghnbmsxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gapnugcnl.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gvvnkxnyq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gnszsqxmo.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gctotcztx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/goqeceion.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gyanjmown.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/guijztcya.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gtyjjsdem.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gdswpauio.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gsplcafal.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gwkphjxme.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gqsjpuwjr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gjcftjtxn.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gzjenjxri.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gmkadchjy.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gyqpcmxao.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gsebzypwj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gybsybszf.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gsgosqcjo.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gzblpfmui.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/govuvcxrk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gqsqbzqko.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/givvfvobl.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpxcsmjse.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gkflgwtkc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/guybsdlhy.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gtxxitngt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gjevkrpgs.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gwaomuqgn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gntcktups.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gvyreixtu.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gcajykcom.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gjankxffz.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gpgdkruck.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/guqrbgets.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gzlsofbvy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gcuvdqyyx.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gxdsvjbfk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gtjvlmmsz.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gdfxkzjxj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdoaqqvbr.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gsdicmmdt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gfgxfhebl.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/geveyjseo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghpuupdrh.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gqgvznmgk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjfvbwvtq.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/goomgcvyo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpqtmerky.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gavqbfbwu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gcfsicdex.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gbshybmmy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gahsxphut.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gwvorpofh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gazrbrrkg.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/getsfdpqw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gqbukzufd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gqbusddui.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/grmxbsykm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gdmdfkiuc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gnsnscbjh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gaydxvxff.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdkonbnen.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gmfdfsdqr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gblichgqi.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gatwbtktg.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gnupfemzk.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gzgdhefad.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/goymlwkry.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/glzfmyctv.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gzgvrigrm.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gfzmfykqf.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gpukhceht.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gkrfdtllp.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gdcndpmjw.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gevfpnwfm.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/geapbbmxk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/goxhorbeg.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gmlabnmjm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gxgngecfy.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gyiyovdku.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/ghvglqtko.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gskpebgjs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxfiorlzj.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gaycswdsg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxdewnwvs.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gxbqnzwhn.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gmedrldra.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gnqgghgzn.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gkbywjiat.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/grtovpkhs.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gezofiupi.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gdxavciac.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gavixzaif.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gfefltzmi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gypjiobzh.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gzikznzua.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gyjfludtk.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/grnypynts.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/ggzfkvpsu.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gkaiubnud.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/glvwbptcs.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gfgdnmtcw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/grpltaffe.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gkzrubxcl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gamjuuktu.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/giwgnaxst.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gjsebmbwo.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gjuunatdd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/ggnxmabfy.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gaugechcd.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gcbldpbvo.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gydpdblke.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gqzdytddy.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gvajavysb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gkagmgcks.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gjcropehn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gxggngtyf.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gaoxozjii.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gglfeygso.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/glswjrvbe.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gjjarzrvp.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gydnuvqzb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gecymhavl.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gllpyxsqp.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gzjewbhan.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gvsaelqyg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/guqxjbqhz.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gbiuanjhe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gdcxkztfv.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gckiejttj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzprjfqei.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gjsbqlwyg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gflcyskot.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/guovqmqxm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gtkrltocr.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gkdfskdmh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gjnyfuzzp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gpdcfljom.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gxokzplxu.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gjblekxxh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gayarzucb.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gvvzfspul.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gizlkuhuv.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gydpicufj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gnuasngoh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gxjzwsgxj.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/ggfbvvrkf.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gxqikdsni.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gkmfsuuia.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gciamiyng.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gepvypjyu.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/ghfflbcml.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gfmbzbbko.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gsrpyxfkv.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gkvlmdmau.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gysflaseh.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gtnobfmkw.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gtlykzjul.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gznfecncm.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gnnogbioy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gnfhnfzsz.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gksdxjerr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbnzvghyw.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gqqeqfcif.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/groifpdfj.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gxhffklfd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gcemedrst.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gkevrmuel.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gkjriukpn.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gntgxvhxc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gtqffzmya.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gegavzsos.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gzvovttfp.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gossxrlef.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gqapimzef.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gquethezu.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gjxsbpxxo.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gjexluchl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gkxceuvpy.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gyqlwpank.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gmqlmnngx.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gfzrmavtx.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/glyhyhsch.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/grsdbsqsg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gmxsefpkg.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gshrhjtac.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gxggqetza.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/ghyjygwcl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gokqspdcy.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gogbeythn.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/getuzdwou.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gwuqqfxet.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/ggpkqaonm.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/ggpsxhqht.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gohmyvnmm.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gykrmnlyj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gnpdxmbiz.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gxjibxicc.sHtML


<!-- 参考信息 -->