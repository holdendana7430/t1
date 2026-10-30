代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geapobxxm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gbkyxjaod.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfvdlzfx.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfavfnnm.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghejpfnui.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gxsrmzmxb.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwcdtxnv.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgtvnhrt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvtdlywj.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwkouptj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gehyyrutf.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/grwnxnawc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvbghqgq.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gntcqdaci.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ggkoapltf.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkwbhlvw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghebyymjr.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvdxpprcy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gzhukqvlb.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gstyouqat.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gmsdckfoa.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegdzqwnm.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/goultrohg.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gupakbsox.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpztekxd.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/ggsfxdtca.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlrvvhnf.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gaheglhrk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnzzrhfp.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gntotlkny.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gdhootoll.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdluopeqa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gradswrmz.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gemypgfzh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcopqjel.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gpziwcvas.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/grbtuzpte.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpnyfafh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gocovoizd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gjbbgxekg.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnhdpvpg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzowimspm.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiinaqhx.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwvnadam.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gyqyarlue.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ggqkddbwi.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gdoihpjvk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxbzakqe.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfjcrudh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohzoxhdr.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwlhslnz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyurmxhzi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuhuebqi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gtmyaqqcj.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gkvizafsp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gplkzvvux.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gojohehia.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsbeglhi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gucworbpe.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfrbheiy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdgjwnzh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhmekpoa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvvgqxxc.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gdplgunsi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gvssoxgst.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefjynord.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gzezofgwl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gpczplhfj.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjwtvayo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gecryljsw.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/grxhquhjt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gilsacowm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gzknsuuzn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gewjsllwn.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvfzavef.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gzdqceyua.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkmsoyts.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gybftrhpc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/goxlvewqt.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnqrrmjq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gsvidhavh.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/ggevjvwku.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gqlsahcst.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gporafyuo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrxgttrx.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqivtcbsa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gvunhpmrn.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxgglfay.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gymuqfhjj.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtdkkefd.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gjjqnsbyp.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/ggqdrfvlx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsvtcpnk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuocsjhw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmnkwtpw.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefrwtkyy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvmaxyoo.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gupgdswsc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaztleuj.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxcpzmjr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuapplfy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvomecym.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gigvlvzfo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyojolxba.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwqgokur.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/guvmkmjgm.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/geccnchnj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/grwpboqod.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwxxfvtv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcohwdok.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymcpafrl.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkofclolf.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjzhzxng.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gwibcnmrm.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvgijbzq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/geenjzumg.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxcrkcgw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gawddxeas.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/grqbebxsc.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgrtpzbc.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghdegxibp.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gkarfesxr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagpulivr.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gvkpyrcik.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyzuwcjes.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gswjopwdp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gryitjmra.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhwmloyt.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqkpnnxas.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxkiilaz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gwhrdqvco.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/ggqopwnwa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gidbzldam.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/guzayreso.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/grbkjhqpu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gwyfncbyf.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqorylbgk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqrnlatn.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gmugnlbmp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gaeimdhjy.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gnqzhacdx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gibygzkmj.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gixtjvblw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvlcnqlw.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gauussktt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjasrqsyn.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gijjghvyw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glffmyzhn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqnegibu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grrllpucx.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gnywzpdkc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnwmmqhhx.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gdkobiktt.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcstudjen.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpowkius.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnsbkbew.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gykiyngfj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqrcjaml.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/ggpbwmfum.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gfllladqz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gvwzyvsmj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gghrhzwms.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghotwtbwx.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gsfvxjkju.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gfbvkjbfs.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gbglbxakp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbracnpya.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gslgwjnac.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtlhmvrb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrtkjdha.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gkexbprxl.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gxumontzr.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnawgfya.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvkjdqji.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyleblxvc.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmqqpsyc.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gquazrcui.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gizputxnl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gttqisseu.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gecagnsap.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbfsqsqn.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoftfpbz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyvzcgovr.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghkhdwscy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxjgftsq.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gcmfkierr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gsifsmvos.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksvecmor.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrdhqmvd.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgfckrgm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gieedrgzd.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcevjkui.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgncdeyg.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmnkscpt.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhtjvkbq.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gzjglvjqk.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gegqilkap.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtatuwgmw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsveycpd.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gsndwwzpy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvluilgdr.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytdazlnr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqlqdglj.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghxnvlkoj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gabgwagpa.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grxmabdvu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqfkjdmqk.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gstzjksgm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjwhrqabi.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gxjwsnrcv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gndgulmel.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/giblklbrc.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdumpezx.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gurgpbivq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glpmbxibs.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gvqufodug.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkoeddvp.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gbusqzlzz.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghdglpjkj.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnjcgwlbr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwshrspox.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedecuepq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkcrrlvd.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gjayfkzlq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnixijbju.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gddtqizsa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgbbrjbd.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gnxjvvzze.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbvecxxa.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gpajfmkxt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtihjmysu.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtiofbmt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gkncmkoge.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/glcdjymog.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gecbvdhzf.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvsourvgu.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbljshfat.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgdojvdu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyqjaqqb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghowifqcs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwbvcfpt.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywqiewzh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoqzpnlo.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsajoflf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gokfqpfnh.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfebyhlf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gybaimsqo.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptrmotle.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsbcicyj.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdomhtqej.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/golmgpvsw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytyqeerk.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gvugbmvzb.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gmobuocew.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gveaadouy.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtheusmid.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gkutlqhgx.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrgkbuti.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxcjwawc.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gduncvdqf.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gzonhmpyc.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gxruvjwhf.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxhofjmn.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gludzhgul.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gyoidgsou.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjkuelgt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gqjffsnzu.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gttzkmfoj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwdzhghw.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gmbfjrvcs.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtczxsort.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkrifulb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gdusapmpn.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gwnailowc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjlyosbj.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gncibvawc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdysyftni.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbprqtgwa.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gskzqhgjt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoircgbm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvyxiknt.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxndfopc.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gibphadth.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gtiqpgyul.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbpyuuov.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gpdvfxrga.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxboklnql.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/ghqgwjvqt.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgrjccao.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/giifelsfb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gkkzsorlj.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gvngnibwv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyzbncwf.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gytsogrlu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxkaerld.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gckdjzivk.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyahseusi.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwlmvkiho.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlkdegua.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/guzcjatdu.sHtML


<!-- 参考信息 -->