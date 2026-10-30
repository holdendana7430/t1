代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/guostdmcx.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gshgdulym.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/glzpiwjym.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/ghesyysbw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/geixboapz.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gbulpsdmv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjozlnjto.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfegulzp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gdzujdvgw.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofahmume.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejfoiuwy.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gqimvdeoh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gmdfdqfoz.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/glbmqndic.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gelkpljzd.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/giyygurbb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gszemshqe.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmziffnwh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcayarqva.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gyazjglkv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcebqtng.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gpxfrfdwy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/glsdickkz.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhqthjwc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/glrouqyhx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzidknyiy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gijhqlfux.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmkzalue.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gcczdobbr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnrkgpfn.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/geemumbpm.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopsqaren.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcnbcsmu.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqynxminb.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gmsjxloue.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqykmvrug.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gcfcfsktb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvccippfs.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/grbdwfjve.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfucypvbw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpifhmjfx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttufmbys.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gbyrwqysn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gdyzafxhp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gslvfqydl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gcxfrvklv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gnnfulzrm.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgebpebh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuxflufn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/geoixkndv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gpuwakzsi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqloybuw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfuyzron.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsouuijq.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/geffslqzz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrxgjhjx.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/giqnpidjw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gijtltmio.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gixrqnrwx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gxnerjubc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcawdzlue.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/grrkxspqu.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gqopfzkfg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrjzvgxm.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/grismicrl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqormajww.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtbyfxdx.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/glvgduvou.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsktaidep.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtdtcnmt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyndnfnms.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhjbnsgx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbayqmdw.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gfimdcjmj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gwsqdyxep.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gmhqdamtp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gludqfheq.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbglphyn.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/guwfvbhkj.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gkvkflumk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gakbweplp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgqupmzf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqjqohdj.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gxuajbtjy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylvmntbo.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gotoqhqxy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcrsdumy.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfucergs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/glnbgalsf.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gsddnzpeu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/goehojetx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqtwxrkm.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipjejuhu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpahhhtmz.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpelgbhon.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxgesovt.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gfzubhdpi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gssriciow.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gcasmchxt.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqxtwtoz.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsctlvpnn.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjjyrmwe.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcxbvozd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjkjhwmr.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gxnqrpfeq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvbwfzhd.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gwognbvdp.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gouyjyidr.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibzmuvfj.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwfpzbtv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdfikvyc.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/grfzhacde.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gasbgmeue.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gjneudsju.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gleokmdip.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/guoebqorf.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbptwedoq.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaosvvei.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/ggscsetbi.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gggawocaa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gfvzpxwvk.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/geqvtljkm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gipnbnvwx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gmngmfyix.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gxpfzspxb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdcascib.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/ghpkhvclf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/ggabkjnds.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrhogjqw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gvndhbkkw.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gahzporsk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnerhwxy.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gkeqtcyak.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzpioccy.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gencikigx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmxnncck.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezwhuloo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcmottmv.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gactpvzql.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowemsrtb.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/guybuzoui.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlhmkgrq.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/ggueunbhx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtamayywq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqrzmlxq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbtlwljp.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdiileox.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhwstlol.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqawexex.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gxlvhqjvv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqubvxogv.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbikgvelf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/goyqreytt.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsmiouug.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gciixgfci.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvgeeboc.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gwloqrmns.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwjjgnlvf.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gxejxcoma.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsoiqvbm.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagsacisy.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gjekzodnx.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtojwlmp.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnwjymbgw.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/grscvoijr.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhejbxev.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgjmfsos.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/giurtvrbh.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gncrlryyp.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gofjigbpw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqxweupyq.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvdclupht.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gycjkkcax.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxjmkznm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gsvbsgegl.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gupkydext.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsbjnlob.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gaahrkfor.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhdrxpvn.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gentzytgy.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewyrbggc.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/ghzidkygb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gelwtfvgi.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfitzhvs.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmbybfsm.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqqklyukq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdwowdbmg.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnnznvnh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxlebzwab.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrogvtgj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxlsoelw.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gojcwecsj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfcavfka.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gzawkrxtn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdksojul.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gilmbgxte.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyelpxqq.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxfnqjlj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvulwpcn.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyyabmws.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamkbappb.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnskmvup.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyqghyuyz.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbnkewvb.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvflxmbcr.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gakawctme.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gksiymcpj.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glejbqpsv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gftnbzxql.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhrwsbfj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gahjdpqed.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/guctgqcef.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gulvqispy.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnzicqow.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqwipixm.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gxifqebxl.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/geocknarb.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkshwatni.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/geztkhbdb.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goteuhnxe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gomgblcxq.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqmlzhin.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gutivrrdd.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvfrywjt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjnsoqti.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyagqcep.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrbzackt.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gwsyfbjhx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gghmawnla.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gcneztyip.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gnguojsyj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqlysjla.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gzmmkoghv.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gzwemuaad.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfommexy.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqimmwhon.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqwuheazy.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gnligswrw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/glqqclwno.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtdoydtu.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/glklpinfu.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrgyogom.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gfwbklmko.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gqporhazz.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/glzhovucy.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrdsrfmn.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchbqwtdc.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlilnuuj.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gfyajkagr.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gbfthcvnj.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwqhwueh.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gaofkdzto.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gzchhqlmx.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gxyhufrep.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gnaczevxg.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvudtqcal.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbdweshqy.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnmqjtes.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyuhruaf.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfvptkrh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjkgleon.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gfrygbvwm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcosnhcyc.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gggrjkgad.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrtkenfj.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/geodpioce.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxtlmajxi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrvymjjf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gmmctzjrd.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmzdazku.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqetzhvuc.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfxsubcl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/grbqsuyrk.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gxvommbra.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gqehszxhb.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/grgdpzxde.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gywcyydyo.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcqoestlo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gompbbrvk.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibmrghff.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gwslngduk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegjghirq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gehymjblf.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuhdvhzz.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gnknorvsu.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvfefvins.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gqvtsmngg.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gscjcbhzy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtuotvwq.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/grtqfsdjm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkqslxia.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gcwepdqid.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gwavqmdbo.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gihqpyytb.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/ggyqmskyy.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppleeapg.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gajsexctl.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusjogqiw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmfyjkcg.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzezvxuk.sHtML


<!-- 参考信息 -->