代发 wailian999

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvbkmjkts.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gpbskjuqp.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grjsecnlf.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gktdhthyf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtdseizu.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/glkhqkgyk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhqregbp.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/givkprjzc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/gghhkgylf.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gawwudrnc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gpkzkjoqu.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gbgwygtbb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/giqwjgfji.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcvlyweo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/gifmvoary.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gyacjpdxj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocczvtvp.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbrvvnnz.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqffbhyl.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfvxaebt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/ghihhlqnv.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavtmhmpd.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqqwacww.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmawuryjn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxqxvayvf.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbbwlune.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gbxojmzyt.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldbjzdtu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyggkveab.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlrdsmpw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjndrxmg.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrbdvvxk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcalzqlw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gybgfsdlz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gvfuoyzeg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gowwxmaoj.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gwatwfcjn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gunzkgqfj.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gktmqbyyd.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gibbervjx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvegianh.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgiyugqh.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gbnuhmzac.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtlhqnmi.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gtzxkobek.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gwdgmeuba.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcjxwpzu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gaynphcpl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gjakorggi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmttgntf.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjripqfo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqhrceqe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gylkprigb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gasqbbjxp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gdrnmqepr.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtelaebx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gsflfgudy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnuevxcx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gtmvzygbt.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gkepdgjxq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gbbayqvgn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjrveuut.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwcfjstq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gxaotwsmq.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gksackmgw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/ggynalqyn.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/grqfkkong.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gtvfpefqp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gppohneof.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfbhbmoa.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gapgrmyvz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gquvxckog.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gqudwfhjc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwkvghwc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/girbbxexx.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbgzdigz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gdemqnsyy.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganuvdztt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcywcjjc.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpunfgyui.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ggkbuyncc.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyhibbyn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gdawwpyza.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/guqrhacme.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gjicgbcso.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gthnyrwys.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrvdlinm.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxpfaqiz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmdoelfr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwxuoueu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gcxssovgb.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbgjosjh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gujrsebge.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoxdbkkv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/glsjbubio.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmwfixjk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjihcbaq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsryqobzf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gasxgacta.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gsuylhslc.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gathugisb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsrznnqo.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gqcqgeokj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/guqywyhip.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gkcmzfbsg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvxsmwsx.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/glqmzchrb.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gsdxypdtf.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gyfcwsbcu.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gquotqref.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gptsokprx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhdehska.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/ghebjrcca.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gpkraflot.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gjvtphlus.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcgojcgl.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekuvruwc.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpleafwa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/grxklmbhz.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcggafsb.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfekmoebp.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gyhguavaf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/ggudgdruy.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/grdkttotn.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqefqzbjs.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gflejqlsc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryanuzru.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmatfsqap.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gqksmqlgm.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gsagdkfit.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwapuwbyd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gjijsfavz.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/giwabmhvw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/glanwxjpm.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gnxidyodn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gxynrepzi.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebxpfqwm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gigdxkfmc.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gmokgwixb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gfprymjrg.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrltfpwg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvdzwyzl.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gphqqvjuu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gifswpoip.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gujffugak.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqclfufis.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gstsfqvzm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkkhxxhnc.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/guhqrpysv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelbeqxse.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfukxwkz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gmdhntehj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/goayztwww.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gryzshnvc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeskluir.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gxjqlciqr.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdifoikhz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfvkauki.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glhqfqkfu.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaksavcz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbwmweqn.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gsskdaowm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgdavctv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghdhqqzys.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzfazxrq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepeuiukk.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvhnwgip.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvczcgex.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gxjcybabk.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gkpkiejbc.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbheeictu.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glubcacad.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gbdyttgfk.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwvtkzdqr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfflibdvo.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigareqcl.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getzvdhvj.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gcgvnlkyg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwyjpyckc.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpneqbmi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqiryjii.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gooiauseb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhjgioww.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtigdepex.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/grkmunwod.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtbebjtw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjfytvdh.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsqhvmcf.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gzcsvkuam.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggmtawlr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmozwcmm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gefbffumv.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxcdlwlx.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gldhjvohd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopkcjeia.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouwcpepq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlbeiymj.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmamlsvk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwgoeiyxs.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzytkkkjn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqrfcegs.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoqwzycj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwuvhjifq.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbocihjy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzhhsmojk.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gvcflcabr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwozrztqc.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gfelaimpb.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjhncton.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/giuoucqfu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gaoekkcbf.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgbtotxc.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuqjbifi.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhdkzyaw.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gohpekmuo.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfnzqyhc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyktfmms.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnimhupy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzldejjh.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gqdwzvrwe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfnihptf.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafsmbpnm.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gmebhhlmy.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gmveivumx.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxtgguss.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gcuqnogez.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gdshaejqr.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/goketupbv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzqmrvsg.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzjyugmz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gdsetwglq.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gsmookfsq.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqhrknep.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/ghnmadrej.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyvdetetn.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gqinooyzb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhtwzswr.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gjntlvhpk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gsayibybk.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdzkyuaq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwycjmnss.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gptyfclni.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwmcjqte.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxiblixjc.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gwktzhhiz.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gmjbcamsi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/genvscfnl.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gguvumkhk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnzxiivd.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gpysnanvj.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gvydcgpuj.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gnuhtcgdf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/grazytxju.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/ggpqbzstj.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glubzetdp.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdklrqdt.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcpamuoy.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gbzwsiofl.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/glvhgbams.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gykxvdqyl.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gokjogjzo.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdzflait.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgxzsics.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnkryjsie.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqcmavsku.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhgihvqo.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsefsahdk.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gojbiwivl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqcsbifz.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvcysbka.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbvmwxfzk.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlvftiol.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhpewvuq.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gcsawuafs.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoxhykyr.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/giaudmvhn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gddlraiqb.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gksppwjlb.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsebdhjpv.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtgichgv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gipqmdrtf.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyuxlqfv.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gynpmiyqt.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gsyobisdl.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gczmnubtf.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkwsejwsm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gnytbcwuf.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkkywvbl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbnbxpod.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gukteupqu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrjylpan.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gnogpqhcb.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gaajydgml.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbdgzormq.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/grpqenfvb.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/grlbbpssr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/giglfaeoy.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gunzpetis.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnpgucjn.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gungdjgpt.sHtML


<!-- 参考信息 -->