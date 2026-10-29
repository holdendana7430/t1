代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gvqeqbnhv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gzvhcfgvr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/ggxhqaafb.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gegettago.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gmugkvnbd.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gcvwqtyxq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzjvzpfnn.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gfrwluaoi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gljaijymq.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gvlhtqgkz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gkxepfhro.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gjwcttxem.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gxvakdjox.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/ggmonzyra.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gyrdjpqgo.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gkbnyadbv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gciuuglrv.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/glxfwndpq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/glvpvtbax.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gtsakjlpm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gjtcsliay.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gaynelsxu.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwaowizfj.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/girjrncud.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gkqkytcxm.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gjrxrmvgg.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghpnzccvh.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/glntrqcqt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gufdzlzqe.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gheqyetqv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gefxtulgs.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gfqlepsij.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gphshaflc.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/ghhrlddza.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gdfyexeeq.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gjlkfxhcs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gvoxweyba.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gxddxfppq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gyolbddrn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gntuwllct.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/grwbkixag.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gqmspjhxp.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gjjvfflfl.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gdwsmajlv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gxpjhqucl.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gzatgkyke.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gaphvnokq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gmvecljox.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gmmsyflnv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gfavlkiqy.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gzfmctmkj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gzcnskquc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gxxkwtlxl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/guiwehvur.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/getbkdsci.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gqrtiywhe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gpvizzsic.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gmguwepgf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gqhswenzp.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gnwldheku.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gkkkboxel.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gwuiynszq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/goqcgnrbx.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gcbiajsty.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gjnjoawtk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gwkxwekwe.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gmhorfvxv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gvsoynllh.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gesqtjtba.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/guvxfwond.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/ggukvkjfw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gkxtrxoom.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gaahohlbu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gxsofcujd.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gzqaslycn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gkoqhsdgn.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gjhmrdwwu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gilyprhqo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gcxgvgsst.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gxjumvfpu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/grbabxjum.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/glwelrbsy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/ggnelhxnw.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gdgrkvawp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzlwvkmsj.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gdzerqimd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/geespwtkz.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gohqrfraj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/geijbfqbk.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gnxllwkqf.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gqzfvgqrz.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gdovholyn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gateesbyv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/grazesojm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gwotjbprr.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gmvynwppq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gasgxngrt.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gnedufkjo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gfkezzhnp.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gfritwevw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gwgowsjfn.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/geostlvxh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/ghgmyeata.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcbehhuzq.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gnjiweubd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghbfpmbpt.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gsvwmyjsr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gqarsdbpb.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gqfewvcac.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gxytrjtur.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/grdyzoeqk.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gvmsiktkm.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/ghfwsxzwd.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gjiecfbfm.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gtfftpfao.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gjmamespr.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gbowtpwgq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gsdstuwtp.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/grmmdgvkt.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/ghivbmzyf.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gwtbyptmn.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gfrxerena.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gehyjaqoj.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gojcffyrq.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gzbbicxzd.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gdcjnwyze.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/guvmtuiqq.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/ghennogkw.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxzulhqkg.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gpzrsgfgq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/guiournje.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gbjdasgsk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gnlhdwemv.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gbwyycbaf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/godclufvd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gcwqiarne.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gzyrbfjnd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gzssemrgy.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gqirklxfg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gdblamncm.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gqxjserhy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gbhevncvz.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gtnhuyubf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gctnrqfwt.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/ggnbndkfh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxhnmvict.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gygweaqza.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gaxocfnrh.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gpbhgpybf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwyafkfxm.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gbbxoirhj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gwlwfskob.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gadmmjhrf.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gafbxjqwn.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gvzdlrvkb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gpuxkynda.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gquywalmg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gjtxhocdg.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gbdbostwl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gzvopgajh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gjyjhvesk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gsurwecyn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/guczjuegn.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gmweooqlu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gxjcyqsxo.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gpmoypmvp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gfkvyqxii.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnpdjkfba.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gdtctnvhm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtaparlsa.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gwbihlpkg.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gcpftzkce.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gvwsqqbay.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gqcfbzbnw.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gwbpsnaec.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gmuymlsbw.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/glugjbbni.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gbkxpgenh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/ghjluicpk.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gzvedzzyw.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gimfoetpp.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/grixawmri.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gazhlcbrx.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gahxelfrs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ggiovjuqw.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gjlrpyzit.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gybfehoht.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gurvdzrbt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gqcfaawvw.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/grpceqbtt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gtsasdpcb.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/galknujqk.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gsrrshdof.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gucagphkb.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gprnpuire.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gaqmaswyj.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/glqhkukoi.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gvzquokxj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gmyeyrotn.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gvsglquyh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/grgxyzuwg.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/grlbhjakl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gndgllljd.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/grndfxeiw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/glterqsdp.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gcjdndkip.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/geslvpyno.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gdjgekffv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gquezaqoa.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/glmvcbopz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gtoxrdkuv.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gigtsqodm.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/ghjckwabd.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/ghlrajwwq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gwqtdishv.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gzhxxrvym.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gghqzdmnk.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gzzamcmzt.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gdeutwjon.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/ggdixvpxu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gavcxhyks.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gupornyvj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/grdbxzjjm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gexmnyxdd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gddcnhdsc.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gyglbpaul.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gybfpigjq.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gtabbazvk.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gtafilkxl.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gcipwlrcl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gqfpupuuy.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gojrvxjnx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gbwdinzel.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/glzczlzek.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gxspnjjpe.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/glajtrnyx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gddxvneyc.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gydqqnffl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvunnuvsa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gaqfokksb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gqqzegwdp.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gwmtfdisn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gaqximnhk.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gsiqymrff.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/grhgonsef.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gntkonqno.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gkoxxrtnc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/golzliezl.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gdgjppckh.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gggndrpqf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gxklxvkbl.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gzpemxrdr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gjpjrskvi.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/ghgdhkpmv.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gfnhhizml.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gqrjubcpn.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/ggxjpnzsp.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/ggcaqxppt.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gcocumqfh.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gjdycjwjy.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gdfeisskl.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gimlesspf.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gwtyyjkep.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/ggbupgkcf.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gedsuyfdy.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gdjnqycpc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/goldkkzvo.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gflzuyhxt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gxuuirjfy.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gcigycfmw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gvzffftdm.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gnyihbpdz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gkkbxiwwk.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/grnnrxwok.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gcexvgfnh.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gvmklpxcc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gmiduuzch.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gkoxmfpax.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gerzngynl.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gulrfbcmp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gfegkuckl.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gpujpdzww.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gerxvqqnc.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gsbymybml.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gujgbrwvt.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gutdryjxc.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gnmgsrnjw.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gmspdgucy.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gtgnppkqm.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gthgtujxm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/guurresvu.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/ghftyqesm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gywedvhab.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gaiysqecg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gjhgvzsmq.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gpdseplsq.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gmdgjadjr.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gmsmgqzea.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gnnhvfyyw.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gjzmrlfxx.sHtML


<!-- 参考信息 -->