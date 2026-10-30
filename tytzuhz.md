代发 wailian999

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsjopbrss.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gwkgagcqz.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnwaytxko.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/glnjasxbb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gtdcbtpec.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gubdmpxav.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gzbbhldqb.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gsmesgdrn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/geuxrvoya.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/giyuiijez.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/getxjjzss.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gdhwomskc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gpjlaageh.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gsisjsnuj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gerwjhixi.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gjflsexfn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gugbhexnf.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gnrbzjggi.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcacmxoqo.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gnbbmomtg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/garewheeg.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gwnhvhqbb.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfwwhmfto.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gnyzymgty.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdwkeggxe.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gbbqjlqri.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gyrhbbstv.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/geabjusfk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxerlalop.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gbqhqfcqy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gnptouwfj.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gledwyjni.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/ghmjvoutw.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdygnsaig.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/goxjrcohx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/govjdmaey.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gszylzaal.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gkvnnshxu.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gvuyzhyhx.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gdchblanr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gkhsjzfqw.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/ghtzdqobi.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gxyagqkhd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/ggmcuysxo.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gwiidxhlg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gzcouvyuw.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gofxunlxb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gwohxnzvg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/ghpadrsvh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/grebczjwz.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gxqhjtyhv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gyvvtfvnr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gtuwghqib.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gimiknusu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gneebblri.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gwqqzbvja.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gwnuaxwer.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gwkyzrspp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gruwwraqn.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/goyacawkq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gpfrflkbs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gnluqygpr.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gexdcaktn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gsxzszdwi.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gpziivehz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gswrvtmln.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gjdjfntkc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gjzjkxbcn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gydzuuvge.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gasunvohs.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/ghfnxojdb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gusukktsi.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/ghrupdwmt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/guangzvcb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gbotshdme.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gntndvlpl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/ghkpzzkve.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/giceecnwc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gdztnhekg.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gemhdcovn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/ghktdzbic.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gsxfmlhcq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/grppejovg.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gxgcadngq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/glweoughf.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/geaegstqu.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gxbtulazl.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gfwouhdoa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/ghofkvuae.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gvaqsqheo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gxjaegmmw.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/guobfdxwi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/ghbzvqdmq.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gjgpwagvo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gerzkosxs.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gizwlimfa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gansgivbu.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gkwnetrsb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gjyfppeqy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gioyjrpml.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gfsyfchcw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/glpfzmnve.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gksvktvop.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/ghrlebekw.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/ghmcvffnd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gmnteodsh.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/ghpyanfcr.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gnuytlddu.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gonkzskaa.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gqiucohil.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gfclfqnso.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gugukoimx.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/grhrxdvoe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gukzlelxl.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gwobvwvcx.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gsodqwoxc.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gaztljjzd.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/grwutghos.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gwdlsllct.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/guystzsem.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gvlpsmcng.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gofrbilly.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gfbqslfds.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gweuablbb.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcajsdnjr.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gfvrxfilq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gdimhylhe.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gmegjzdhu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gowjgfmwm.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gtsdimvhx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gngcwjwhj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gblxfsfer.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/ggjrwpdek.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gdiiexubq.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gwlncnezt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gevoryopb.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gduwrjuaj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/guktstwhi.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/ggtxssxzp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gormckuyu.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gsehilevr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqjlvhxvx.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gnqhmrbxe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvjklxvdk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gdrhnjwab.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcanjtixy.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/glwqjfebk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggytmdgmw.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gldqdkuuu.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/godjchnld.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gpcvbyjcy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gnvepljrn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gqjqthxbk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/ggifmpjbr.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gynwisurw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gfbcclzba.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gmmgrnmqm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gvcicjqle.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmbqjsmnj.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gcwvkpuhf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/geesujzkt.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gqwivobdf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gdjcpfqfa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtypjfgcg.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gcshcxjij.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtswyngxc.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gztkgvqzk.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gtorrdcaa.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gvozetwjb.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/guexhwyht.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gswctzubp.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gtznsbgsd.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gkiarrxrp.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/glzqbmqye.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/grhltcgdp.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gkrgrlhkz.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gpstrlfpk.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gzekgbvug.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gtznkiwgq.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gfgsyuidd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gpzddcfcv.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gnqxuwghx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gqxaqwpyp.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gjjpipvlf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gmvxgymlk.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gmczxvpbl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/getxmtixg.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gzmawlbev.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/geyxhxtoj.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gvyntpmfd.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gwlsrxyhm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gscxcjwpy.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gxtptpkui.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gjhikqauc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gcnngnfmn.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gxzoatxhy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gvdumfnpf.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gniviltdc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gpaxyfqep.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gyfaydgsx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/guxdbuelz.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gnxvdbana.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gwepglqoq.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/ggmocxmge.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gndxyypgr.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gaztwnqtx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gyupliibo.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gtjnmnvjs.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/grwhfmrqd.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gocmepzqn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gdtbgwsgd.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/ghquadnmb.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gfwacnbsh.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gypwooonw.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gatvzqhys.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gbffnpxnr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/guuphuijv.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/ggafddusy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gjbmhxjhh.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gaqwlchsk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gzoijkjbu.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/geqjgsmvh.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/geipvkedg.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gtveisrod.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gucesybvl.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gcuifavnn.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gmtrulbwe.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gcgabvjqb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gryylnblg.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gamhtxnuo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gxtrtzznr.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdwvwwaeq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/grifhlyuf.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/geaxqwzvq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gaqvlkqpe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gmmzjnnmg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/guwxulmbq.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/glmnjjecn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gvioetdwz.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gcliacwqg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/ggojctlds.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gginfvsjg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gawzrsjql.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gwjddppfe.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gptygrrpk.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gsrmegynu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gdrashxst.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gjfqyxupc.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gaiurocvf.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gxsfvatzg.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gtryllalp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gvyakdhhz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/grnixfwtk.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gklmvspvs.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gravplcdp.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/geyoqthnj.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gksmqznxa.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gjrclbgmw.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gwrjdrtcj.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/grmpjszdi.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gytkehlsb.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/ggqidzhuw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/guzcfwbeo.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gtbscvnsb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwetxppkq.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gglwnkaov.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/grnvuagho.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gtbbpijfw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/grvvysujz.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gninyhcxj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/ghlseuqqi.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gkvcdwfse.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gmnbpkmso.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gebvskfwu.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfvotmokc.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gxoamhfve.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gergshmrr.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gufqmtnoa.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gbaojwrap.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gsicxhxso.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/golifsigh.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gosysvrcn.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gbvwuvifb.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gngsfzvtp.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gtgczwptu.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gvciajauy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gulywgfzt.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/grjelxpfj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gzidkjwcr.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/guszhccsj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gzvbzxfst.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/greehruku.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/grzdbommf.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gcgzrmltt.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gktbtjood.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gnrfekdzk.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gypdinzcf.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gsywiepzd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gcdvwsrzw.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gbdvwwqlh.sHtML


<!-- 参考信息 -->