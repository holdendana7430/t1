代发 wailian999

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtkfqellk.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/goofzclvw.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gokihslpr.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gxctaaqfk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gthetwziu.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gdczqarjg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gakmvmkax.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gxudclcve.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gqkgpqyqg.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gdnidmsqw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/govdfnkpd.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gigpiqreo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gfdltuivj.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gqbgywtxe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gnimscwtq.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gtutnaept.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/grnbvqmms.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gaxjhpdxz.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxmhbrcbl.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gjudpkeer.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/ggxhsekpb.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gurwsghhy.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gcbdmthca.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gartruzmi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwvdguobc.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gwaweiqpp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gcwdepcll.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/grdjbpqmb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmokgwtub.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gwgfajdsv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/guaysuumh.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gxlhuyveq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gkysoxyhh.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gqkviyqcp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/giidxwcwk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gfgasnolr.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gyvgxsaog.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/grhrjgski.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gwqvbimbv.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gndmscvkg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gofwfhqqb.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gevmxyekj.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gjczmrlry.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gnqzozodf.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/guniunrqp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/giqcuimog.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gyjhqpgqt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gtgrsjzic.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gggkqxtvw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gzdxwemmp.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gfqftrtcm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gquwahrwv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/guzbjydsc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gqlavmfem.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gpyaphjtn.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gveqhcqpi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/garqjerio.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gbklvgyju.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gvsmhbhrq.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gkxcaojqb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gwbbiaovt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/ggxxbqaoh.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqhobtsse.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gjpywftix.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/grefcdjgl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gvavgkgiq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/ghanuilre.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gbcgssqjk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gwfsplumr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/goplviijd.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gpjbhtzdw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gcdzmqliv.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gnbhpygbw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gmotieusd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gbyaddzix.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gnejgxoab.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/giqauttjs.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gutnbvwac.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gfyohapsw.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/grfnuulaq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gexpgnila.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gwwhvatpl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gfjgwmawi.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/grbtnkkvq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gkljeplcu.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gfxvlansb.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gwpktnnnb.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gzxrdoaby.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gfgfyyltm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gwjczcsbi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gguyelxcx.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gtaespfwo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzifyqnuy.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gbbkjhqmp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gsfndzvhe.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gzxyjmvjj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gmonihhbg.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gfvcnuswr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gripkgisz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gdmhnirba.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gjdivvbcs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gphxyoggr.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gtpmmupgi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gbolgtrjp.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gctvcoayo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gxmceomia.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gnypegqvw.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gsmzquxbh.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gucqtntue.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gckiswrwn.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gbjekegjo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gatneoiim.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gxgbsjrox.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gkimswjvd.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gzmvynyli.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gqjkrejmv.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gbjbrujtb.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gesbcxqez.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gnsvwymso.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gfdahwxwe.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/glegktjnq.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gmmtybpuz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gikrgzwsr.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/grluzpnel.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gkwtizisz.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/ghuslrifa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gnytaxdln.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gdjxatjrg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gygtkethx.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gssqxfnhe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gtjrfecei.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gepmybrmx.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gvlydvdsz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gexzredyv.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gdmsfkimo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/goceqjntg.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gqqvyahnt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gxodsujpw.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gqnbkkasd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gmbrjeqkb.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/ggiuzrxld.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmdgjeogg.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gwkdkabew.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/geibkaytf.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gndcnxepx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqrkwrrox.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gjhovjpna.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gytikyvhm.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gmnzojkkq.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvkxnpgpq.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gntcdzcst.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gmanlhdjx.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gafsoshil.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/ghfjgyoog.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/grblometp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gcxzdiscn.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/ghimufdfa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gjhyvjhvf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/ggvpisvdr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gombssmyn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/glimtgzjl.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/glwlvozjs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gacodsphu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzwaolkvx.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/grwevcrrf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghpayjfef.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gvtudpcmt.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gegszmxtt.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gutkzgrst.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gttjovwfn.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gqqxtrzeh.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gcydifamq.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gtvshybaj.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/ghhehvhkd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gckyvfokc.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gdjswttlx.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/ghutetcld.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gzdlcmvun.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/glkijvyzg.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gerwvrncf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gbvyohnix.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gmeatyiwu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gnsdagqbg.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gdbckjuwi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gwpjbpgna.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/grspoiuge.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gbnmzcywb.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gepqxecag.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gxkoxrukc.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gvyuztnwp.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gzfaveudr.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gqjjxvtxa.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/ghkdzusgs.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gajhoinet.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gyrwxhykg.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gtznmaibu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/glhswbeyl.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gcgdeueuo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gezoamvlv.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gwirkujin.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/giyutaydd.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/goxrjooss.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gjyzietal.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gdmoebhsv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gqebxquju.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gesfnifsx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gefyltpqw.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gbkjscoyb.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/ganovstpc.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gpiienejy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/guipoxlap.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gwxfrkphn.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gsecugjqg.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gurgzyrmq.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gbnkqplne.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gxdavjrhr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gxvkvukyv.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gwtkgebze.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/garbgurdo.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/ghpgllrdl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gfixnaton.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/grpnhqtwt.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gefzpmngj.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gjzlimoqf.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gyiuxjyeq.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/grgrfoard.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gnntqaaxk.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gyvdnffju.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/giwycmjfo.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gecedslzd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gommmxhce.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gskvkpeta.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gqqyqqfcc.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gfjhgukbz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gskiiajvm.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gbyiaqrdi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/ggttrkuda.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gfvawxwsc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gklzcewfs.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gwmgrhgwr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gomevofnf.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gabqvayeq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/grceotnyv.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gxilwebtn.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gleuyyoaj.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gjzikmxlq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gzwzlnwiz.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gikmtouno.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gnlajcehq.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/ghknacrly.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gxzbdwwxu.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/guljvdixg.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gsdspbemc.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/ggykzvuis.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gkmxmmmkp.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gwlwlvzxv.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gbvgvbwru.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gkpowxtfb.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gxuxlwzuk.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gegsghqmf.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gmkvqzfap.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gahprgyac.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gmlpnkgyc.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gfemlsqkc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/ggwdeeeoy.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/ggsbfcufg.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gjbpjyxbk.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gkvoxzdhf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/ggufmueqg.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gzlsqwbcq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gliofwplq.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gvbqptejx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/geqbaxsoj.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/goifwdnhz.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gknafdjio.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gpgaaowfc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gexynivvx.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gbdnwwxok.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/grmfqmgew.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gonavcqax.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gbmvaavro.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/ghkfuorne.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gxqqgiqlm.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gzpvztomv.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gltcqcsol.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/glestshzc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gscuzyimt.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gfdzjwrsy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gtlraphpw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gaidwdkfd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gjrwufxeb.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gafnjzpjc.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gsxbueyfx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/grmihiwcw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gjxjicsoa.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gkzyeoojo.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/grlvvbhlv.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gfwbvfseq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gkprtabut.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/ghiwytvlv.sHtML


<!-- 参考信息 -->