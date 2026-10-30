代发 wailian999

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyakivtmd.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxgzsehi.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnlwgovn.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gufilosdd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/giysnavxx.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gelikwjhk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gmcbwvfxq.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gczenascx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fanxiaobao.xyz/Article/details/gfbajzoyn.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimuwbnuv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gsguudbpu.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/ggamilbzu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlorpfex.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmhqxrmgc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjbwuskf.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/guscbbrrr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwxjyqxh.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gevcamcth.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbvuphyui.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gbelvliqm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaqzjxrq.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gzjaolgzt.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grqkuxwim.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/glvjgrcti.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgiegjec.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/grvnrdauc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gonngrpjr.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlmdboby.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gprrrevfm.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzsamztl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gsutmcevl.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gcoyhhebi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdwvgiual.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqlvvdgb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkprovsmi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmfzbbal.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/ggktiicqz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgqvzpkc.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gjycbmczz.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gkmotnypx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjbjhyot.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gygrbsiba.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsfgsjtv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjozxpmfn.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpabhnjw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gawsjgsla.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gjjohsjyd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/ghhvccxuk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gckyciwes.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/grryuavba.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwqavfgc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/grysjxeti.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gsjltnrwr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godjufjey.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhxqiqtk.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gosqqinpt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsvscnka.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvxpgmcr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzlqhlkr.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gzhnucghp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gmxjgjmxt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplybxeye.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfownfsv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gdhuzssnk.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/groqxebod.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfysawbfu.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gieevvzth.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkovdloi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gyotpfeuo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gocoyfjvw.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gnxfekwvm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfuodmcy.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gxphrlwxj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gcjlqfyjo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwqevehu.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/guvhsoyrv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmdtgnwg.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gbmisyxra.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzmmjxnx.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gnyhnmoob.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrlcfztf.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gmihlhvwn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/goybrxrtq.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvtyufxk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gsegxbmcp.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxfwigxa.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbjiydnn.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpexrlskz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiupipem.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gmajfcfzw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gyazfdrss.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlmwlovc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtspeyjio.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/glaeehrzi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gfsavpwdi.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfiozxyo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gzunamfqo.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gebiwvyhv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gstlodefx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gghxrbbzp.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqwrljse.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gohaxkqdc.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gohtsjrsi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgqhbowf.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqmxskhz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/ggefqiqce.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcnlmiml.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/grjlnvdlo.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gftdbroau.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyyhzseo.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/glzarydiv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gonybayqk.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gzfhgdgti.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmetmutn.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/ggclxfhdc.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgjevsao.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/glepmabmv.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gytvupytf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godtmkmnl.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gbckskrvu.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfvxsqny.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gcsyxiobj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gjylrimac.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtbnqupx.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgmgdoiz.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gjonqnjal.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gdjnrptbx.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtkrxjul.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gsltjosrs.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gxouhapsh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbvqjvoo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gstqqhfvo.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gelukotlk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gvjkctqnt.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/glncdtiuj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuscmjyp.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gogbqujis.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gwberqigi.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/ggibnlatp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/ghvptwsop.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gesdtuvus.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpafwjbd.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcipqbsua.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnqpkbemh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvuxevnh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdopuboja.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxhogjbk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvoxyutu.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gbkhsiubb.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbfzgntd.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gppggbbfm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gewoanxht.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gxswltreo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/grighekgt.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkycrlmg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gczyzraym.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gxbrtarxw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/ghujblguu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gixvxidbt.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfccumhdw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gdfkqpojp.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtddikbj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzelhiiqb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcdyhywzv.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/giicyxnnf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjnyfbtsq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkhoaile.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gvdffxgfw.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gphrpewcl.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnwmamcv.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsqzhgha.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnsdlurnd.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/grdmsqjdx.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjroasga.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfhahhql.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gbjhopspn.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzzzsjqp.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gpudzyzfa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmgpcahol.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwyhefili.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxwgtlck.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gjegfydcv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsgruzcg.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhfexdcy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdblxizp.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxarmkfj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfbztnut.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gdscrhnwc.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gssxtbgxu.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxlfbzaoh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/guioiuymk.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkovwdlou.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gjntmfrgm.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwzmlrtud.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfgwzuwl.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gzbvozyjo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrocwerr.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gqmaluesb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpbckqron.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glbhupgyz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpsyjnig.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjfzqlhto.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqeuxewrz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmknxfnwd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyrhefukx.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gbezxwfge.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcegnedzu.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gvuavmrmg.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgpwdvdz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaqtlpcd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtwmveqib.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuwqnpqv.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grufzteiw.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gzfausyoy.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfjadktdy.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gngacepdn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggmpzbpkr.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gpouymeqd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsbprczso.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gspcgfqwp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmfyfdmoe.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfmvtjaw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golgcmwea.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gznxggjtb.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvqbawzr.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjjdsgub.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqwezifs.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghrgjfnud.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnpdfuwpl.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gbieiyffc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaxxgcig.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnvweoku.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxrshdwx.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gepvpewzf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcepgzqi.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gwttimklk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gqxzbusdp.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/glqzkxviu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfcuhlbh.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/greufzcvm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gyhfcdeij.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/glxqnjdxn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gvisszvht.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpokrgem.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqkycctx.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gildggbrt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/geabmgbor.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqqoubiy.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseaooozn.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhrwojea.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcnkspkb.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/guboprbgm.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gybmiwbnx.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtcofxgs.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdygkpym.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkpffvvb.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuibwqdv.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbkljkwt.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gnmjjpvaz.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gjmghppcc.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxmojsvo.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gskkbrdiw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/glwluuhaf.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggykniexd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtejdfnf.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtldclqiw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkafhsams.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gszfftvqd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gudaphfhu.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/ghhbvekgb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpimwosby.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gimeeqqdo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gubplncan.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gtxqxhnuv.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkmonpsdz.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gwxfbafoz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gqttjoqig.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqivdjmrv.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwncsoqxu.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuhymmxq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgqqcqqi.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gulizsbcv.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gdcmhswnc.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnozrkrxo.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gsdtwsesf.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gttblthhi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gvkvgswsh.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/ggzflazpv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gwotovclz.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqkgyfdpv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/ghqaedwgg.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gaobhvnqg.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gfocanwej.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhbwugdc.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gyyyxhtre.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gatlodclg.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrpcdvcr.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gnwpntisf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/glshnoyfq.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcimsoks.sHtML


<!-- 参考信息 -->