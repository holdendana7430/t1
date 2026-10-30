代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqrlaped.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkiinryv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ggtatxahj.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gluibdguv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/glzycafxy.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/glfmdndub.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gbbeuycfg.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gqkhuddnd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdttdbla.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gocblaerk.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvtjskipm.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gohidqpzx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawqvbzlk.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gatqckpec.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxetnaet.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gjjeclduh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gykigjwaj.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gknurpugv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobbegjmx.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlyvvviu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glujsidtg.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gxsxvvzsr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gysajfecl.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gelxtkzhh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/galearafl.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gacgrwfal.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvhzxchi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqagwoer.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gadvyqnil.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwduuzefw.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gaphynaaq.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtxkgdgi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gurxruwzn.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gicrvzckb.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpuejtza.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gxzhyimgd.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gnqkzdpnk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gpumpkvjh.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gjozczjbd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxthqkwd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gqzgtknmn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhuwzojl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxkqhecb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gemgaupqu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyureybgr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtssiqjlh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gryauodic.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gffttwcxz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gsyonexop.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gejcrnoxd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gjcxhfjid.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxlpzmhw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnueiweai.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gpftxlkrw.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgqkxzkg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gwthdkimt.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdcshjhl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuswaayf.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gmqhiyfbq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gowwdzqsk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcptmvomm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gpoxhyrsp.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufmlicil.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/grbiugcct.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvkrxdgy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtvnlwvm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gmywnwolj.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuplrsmk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoegclld.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gcotjevzt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/ghnpghwjg.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gtgtiwbtn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxznuvob.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gieabwdvx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfliapvxa.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gbnlmdtii.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhhexlyx.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqclaaad.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gfqdofkbp.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmmgohos.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/goryxolok.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/ghnlonlba.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geocaxbsh.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/grasvtxga.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gasbdznoa.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gciubtnrm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/goocxhqey.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqcsdcas.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrmogecd.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gnwvsuxqc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjatcqxqu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gqowwlmwk.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhgvmlea.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gkziasanx.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gfezfxxno.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryedwlna.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojdlgqag.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyqeuthj.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gvjfjqeyk.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gfbzoptme.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvgiglrc.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/geqpdjdvz.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvidwmfz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gwyzzmfmf.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqojfrsnp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvyakadl.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gwuqkfwts.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/grvzeolmv.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsscjtqv.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gweeqawyz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gyecfhrpi.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gsrfkxrgy.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvppahca.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/grpfuvkwp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpzifcex.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gpihcbbdk.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoxuryfi.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/ghteiqfut.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gpzmorzkl.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjelwzelu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/glbzwmohm.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsicbexw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gtzwvznio.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gyvnwvvxd.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/ggvvnaevg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/glulhbhfq.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjwprzfs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gxkbosvqo.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxtymfck.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gxnnckndy.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukavbqgr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gyptdtdsf.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gcxvrfhsz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcgkqhzil.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmkxdtorp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkujwurre.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gtrdarpbr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gosvobuef.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxebgmzed.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfejjlcvg.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gebroreli.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyszqupe.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gafnhcqzx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gloaggioh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/ghslsqnya.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggopzffzp.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhmccwcq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyntgvkte.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhjvdkbd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gouvegigi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqfwwdlvd.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gxmleqatv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpjpriyg.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gharpvqap.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvmrctzn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqjohqgm.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/glwvlkxfa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbopunao.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gsutvygyj.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcshgvbq.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gikiuzagr.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/garicogdv.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gbfwcycwi.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmhuyefe.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gempyqlrs.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gicmbbtxw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjygsqjq.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwifjnqjh.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfvouwqg.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzkhepyf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuikdzrz.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgwmluay.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxmiioxtt.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gunxuzaqj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfadvegvf.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gckugkpwm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyflsssz.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfbqngns.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfvxfnkf.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbskdejz.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspnnlomb.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxgzbwoo.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/ghikvtbiu.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnpavsek.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbezicbu.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbhvhsgg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxmqbtvai.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gvodytewb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwzdxcooq.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gayzeswld.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmydtjdbf.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpflireej.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqeaoagu.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gdualmlfh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpnzfiik.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybioopfd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmboppxxc.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/goepamycz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmoxalppy.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdwrzhxzi.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvmkfgwhg.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gfirrpnyz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddhjyjbb.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhkpjqtg.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbfombina.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxqmcgae.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gibtoooga.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjjnixdw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/glivgtlzc.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gejdaoxid.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grdedfjjz.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gtcthokab.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geawgpymi.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyavgqgz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gojlmybjd.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gogtabcri.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcpwbzvy.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gndibwdwg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gmljeaqry.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grpyqbucr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gthccqojv.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/grtwrmnxg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/guvnmdvru.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/geczlhhrv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgjeyytr.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gheriongo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmtlsear.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupypmxaj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gdghsknri.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzlxhsfy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gngghkxtf.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gfwgajcua.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gbessgfva.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gnaqyrxvd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/glouhmcfd.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqlghsqdj.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gzieopnoy.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gptxsssoh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtggyenbd.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gzqzlutqi.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gpfilzitj.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcnryyan.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gfrtpeeei.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gymaqeyuf.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gynomcstx.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxuefwel.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goxapqzbr.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gaorqgqul.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqaljbbt.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gaappicot.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ghxyjmvie.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuqmtzes.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gweubxzwe.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gkydzalaw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/ghmuokxge.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gozjmwkjj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glmmfmgru.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gfczkmyno.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/giomzkpak.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gallxogfj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfcvgecg.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gffevlpyy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqzjkrtgc.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/giwcucbze.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcnkroxw.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gtwzcvwsl.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmazgoom.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gvmzrvgrz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guemmjeqq.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgaherpr.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giuceuzpu.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswrserrn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gjulimvft.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gatnqubqc.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/guoneodwl.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcsvwjtv.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtuzquju.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcudtbnee.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gbafdyedt.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gpzxjjiwk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gwvsdynww.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gekhveuqh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfkvxchu.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfemohhon.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gadwvxnks.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvtzrshay.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/ggqhjfimt.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/grwvzuynr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewqfuxoo.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gtijcyjtc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/guwkujqbs.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghknwpjdd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyyetjmx.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/ggmukipzf.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrssreqw.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gxaohgogm.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gbvnwlqls.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjzaqdqp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdovynwya.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gokucqwfw.sHtML


<!-- 参考信息 -->