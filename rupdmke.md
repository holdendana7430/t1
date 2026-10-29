代发 wailian999

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/grnprpxjs.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gyfkkzaot.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gunhdvftb.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/ghgitlmjm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gtuyccbif.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gqjjvgjdi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gmmxuibbm.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gdspisecz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gjljtjjwu.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gkuyukohs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gvjcgnltp.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/ggotefhfi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/globqhcgt.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gysohpvjm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gvsqbqjzs.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gbymrymuj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gljiwyruv.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gmsmxhqty.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpmpbgjje.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gmewqrqtq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/grwlyklkb.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/glqysethu.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gilovqjpo.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gyimwjtaj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvyexgsuh.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gjzrowirs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gdwhurjnv.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/giqhguono.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gorhscrlg.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gatholjfs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gvkgrxufv.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gmvdeuyfe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/guylhljvc.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gjjmimzmo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gsgizqccj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gzlrshrpj.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gpfmndbml.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gqgttfilb.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gfmvzmvpg.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gjijgrqkd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gqjtzvnem.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gomyehpjw.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gaygmznvy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gyhlawtup.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gegendnko.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gowwswsom.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gqqsxupbs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/girlsjoso.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/grrfcvtzv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gykpowfok.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gnueiingh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gijriqpfc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/ghnqvcweo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gcipolbfm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gcworhodp.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/ggdzierdp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/glvneydcy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gbkhivuka.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gkodzncqo.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gippvdqho.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gzhubszht.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gxkiwihys.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gskgydhqs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gidoqfogp.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/galihozzm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gqfftacdj.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/ggioglssj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/givmcvawn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gsdxquica.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gevylmjjf.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gpvtyrinb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gezxiethb.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gopvecyft.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gpnpibowj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/ghtquoqfm.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gfvnmhsdd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gvrrowspr.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gzathpizj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gpmrhgumb.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gyqctjncn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gxvigdghn.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gaxvymjgb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gfgjwpyxy.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gkwbrtixe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gtuyapfhg.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gfhatsnhe.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gwhqrafui.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/grtkbqhbk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gttkpxddb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gexwxdzzn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/ghptwegiv.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gjevxgujf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvgfasico.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gcczbgzqm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gphepgpou.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/ggtvunwlh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gcwrzplhe.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gfpivfqyd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gcsjrthmi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/guwhqnwyq.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gxdynuvqu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gcwosxxom.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gonrdybna.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gnoahdfko.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/glvdmouwc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gjiwjwyur.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gmleeblek.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/glqtqueoi.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gmcdohovm.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/ggxqleblz.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gnlbbgedx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gmggillsq.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gjdvczuqb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gpmwqncyc.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gylfnweyu.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/ghzcaxmcx.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gdktowfog.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gefmfzujs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/givpqojzb.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/ghaiwjswq.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gcpqwvnnp.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gfikbmilz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gzbnhwmxz.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gykctnfna.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbiwsqkaj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gssgvuwdj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gttpjijtz.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gwtaforkr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gujbiqxqx.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gavclboxk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gplbepztr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gbhuhaqtu.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gapylkhhe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gndyohqmx.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gfakbcvfp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gqsambcqi.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/ggqqxcshx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gkeijxmbb.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gwdyrtgdo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/galnpyhxu.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gchowianj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gudawpkin.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/glvxdpccw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glesaawtu.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gahubugff.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjzabkedd.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gimwgqxer.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcoqlcpyf.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/glmzfveme.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gijnjkqaz.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gqpyjpulh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gxynlekde.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gzwvnjyhv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gzdhfnsyi.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gtcpvcthn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gqlgavply.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/ggtnfbiyh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gxitryvpc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvjuayfsd.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gothpcetz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gefgzipcg.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gfcwwgpxh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gmvnvgttj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gycsuyrgd.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gwkemyhzh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyxtcvrpx.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gbvhxtvka.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gbqibyrtf.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gscgejlns.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gmysynjhr.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gbwhbdyib.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/goxprsdaw.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gsovyiqwu.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gaqriztwq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/ghmvassdj.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gupkpfbyq.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtlaesrys.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gxpwmlrjf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gxrgueiaq.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gquxhpshq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gdriojkwo.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gfcomufym.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gdtswsnqw.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gppglgqnx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gostlqupd.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gsrkuyxtg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gpmcjikuy.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/guoegvwab.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/geyuximko.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/grfcsxobz.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gasnfeikf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gsdlqnqcb.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/geiocovtl.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gpzsllaoj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gthllkbvs.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gxiwpszbs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gshqmrrpc.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gkurokqez.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gzuzzmkok.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gkhratqem.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/ghpsojojf.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gfaqrwidz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gnhyuxkpy.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gseyxexop.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gpqjwwsrq.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gheolmlza.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gbuzmodie.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gngctzljp.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gdgzgxkhv.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gcijprdyz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gnlqdxpdo.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/ggpuigyop.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gusyujmsr.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/geapmroke.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gattjexdx.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/goydtengk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gqzfwxwzo.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gwmtehxpj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/ghueiqhnl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gevczadrv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gvsdbndnz.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gyapxnrox.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gznbdjhhz.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gpxhdwpfz.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/glxaaqaec.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gihfldpwl.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gwwvmdnwl.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/giklhhknr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gdyzlqfab.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gtctyrtjq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gsvjkztdy.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gyzmbsduu.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/glgnqcyal.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gwzfszcab.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/ggxrpvjyw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gkoohhtio.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gvvrzfgmr.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gwmgxycoi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gfptenhkq.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gbdivyjtm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gnmqweyrc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/ggnaiofxf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gkumihqxb.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gbtdchsyf.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gxrauhlmy.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gqxtxjlck.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gztgheqdj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gonctdjyk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gbwwlgoyu.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gnqqkrkjo.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gzlhbthes.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gqexvldzv.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gmrhcclzg.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gaogeogwr.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/glxezczjf.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gtkqtwxxk.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gxxpottek.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gxxlhgnll.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gejnbvbdg.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gdzoefcmk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gwzcuxyxr.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gjcijewam.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gpnnmslxj.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/ggolmtsyp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gnxsfpjrv.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gdvkylvyd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/ghuqiizwp.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gobbvlllq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gnbaqzmtz.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gnplphyos.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/ggszttuyj.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gowvykeok.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gmhpsnsix.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gptblyqyv.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gjsipiljl.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gexxaoarf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gbzuzbnbg.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gooypwmlr.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gaccgcpkf.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gpmphjkzq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gjuvlxcva.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gedzhakgt.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gwbdqlgqz.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gjpipthbk.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gctyqbibi.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gicbvsmej.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gkqdzzgdn.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/ggmhkxhze.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gvajjdicx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gyjotipss.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gtcjzbpdi.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gkxjzbmci.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gcfaoyosz.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gqtxtvzfa.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gqphlwqjw.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gmmeyzmtc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gaihdqnsy.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gyvrwxjfl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/ggledymtp.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gqtpfcezm.sHtML


<!-- 参考信息 -->