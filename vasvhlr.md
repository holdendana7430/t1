代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gisqxzjsb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/glxjalrtb.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gepxylqzl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gjqbmzimf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gxchjwrst.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/grtkxdsdq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gidvalalu.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gdzllbptu.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gnlpteian.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gupssqnjx.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gwegbvham.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gzozxajth.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gbmesxhjd.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gehepxkdd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/ggtlghxwi.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gzuzngyyc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/goztbfihg.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gtlpgqeki.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/ggsugjpkk.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gqrpisvsn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gxzvnshse.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/garlrahlc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gvteiiyuk.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/grwefzpog.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gmswafrmd.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/godjwmdjr.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gnlyouuul.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gvlnixksp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gwnrcrfwi.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gzupqhnqu.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfhomaruv.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gkkdcjecc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gljvdxrlk.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gocirqkis.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gocmgjssy.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gwnzpncrs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grhbexjxz.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gwtrcwgtx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gprolpbgi.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/glkoixlng.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gldbngszo.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfgdlgxfc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ghfahckhi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gugjckhkb.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gezckaphe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gqxweadvg.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gshexisdh.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gynmrjism.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/guixyqilu.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gfkgqfvcq.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gtytcmleo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gfsenilmg.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gqymivcyp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gwgeozanx.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/ghniltpbm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gnmiqcwcs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gwnjicqcy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gdrdkyiyh.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gmwcwdvrx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gqgyrqiux.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/ggtgbscbs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gqxxwgqdo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gyeuknqvq.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/grsmssfjm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gycsygxqq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gdfjmxakb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gvgeirkso.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/ghqyhosnm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/ghnplkhpl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gkpfrhstu.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gkzduqsnx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gbfmlkzcf.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gipuscprv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gmncoxvyp.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gailghdzo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/ggsfyzshd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gftadktii.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gzjonyjet.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gbphfrzux.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gwonrxjpi.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/glwwinenu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gaixtzcsq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gkxqfyjrm.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gmhmwwhlq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gmhljwqlx.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gddflobjg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gvdapwyis.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gqxndzqkd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnlbxifzd.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gsoarqxit.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gdlgmxlzp.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gcvlfcncz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/glbjzaqfp.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gwazjthmf.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gcsqiqyfj.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gyzcyyvvb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gfsnaxsdr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/ghnlhvbsx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gnncsmtda.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/grwkmpghc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzztwrdfl.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/ggkercjbr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/ganyntnwg.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gvuygirwu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gzfdbvmdb.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gsobqwxit.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/glzehgtkg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxnpxyzzy.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gooknoubm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdtrqhsnw.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gzsxohzmj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gsahfolom.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gxcndsjpy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gxffsyksq.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gzgnnulyr.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/ghoezagrx.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gteqbuyyv.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gdnhkwxln.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gjuhsomxi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/geicmxglw.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gddkmecwq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gmmizwkdm.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gxjfiuwem.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/geqoogvgd.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/ghmknhvcn.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gsyhdwpfs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gnemzqfjx.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gytmheeih.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gfuawuzea.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gsqudcsbt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gzmtrabiu.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gcxqevmjr.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxuwgalii.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/goybtwagd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gxcsbpnvr.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gqsixswma.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gtogzbfdt.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gmibzbqbe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gfxiefbyn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gavykmegr.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gkxdakwms.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gjhyegzvn.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gnqwcsdmm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gzkjgvjpn.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gzbvcqvjy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/ggqfekptu.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gtmbromnt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gxusfmutf.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gobjolfzg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwakckcez.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gadkmdaaw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gwdiqpvzd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/geonwshkp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpqgyxgjo.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gpdtxpsou.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjamrnpkw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gmcfmmbkl.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcnqndohs.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gjpbyebgo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/guauakdlu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gyqsdhqqj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/geleinhoe.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gvnjfuarc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gydpvxnjj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gofqbvafr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/ghcvddjyl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwutliroz.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gmuaayvtr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/guzpvsrqa.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gedsiagok.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gxolljgup.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfiqlftft.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/geuzkzbyj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geqkshcuz.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gukmjtkkx.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gkythhlgz.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gvterpvwg.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/grfmxqkbc.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/ghljhntxh.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gvahjgnuu.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gvdcqumoh.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gsupzhecj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gxtctpjmk.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gtmwyzqmp.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gzlxuancu.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gwmudqvhf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gixnuqvdj.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gaotyxyjh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gzodglueu.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gclrtouny.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gjprudxuq.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gjmovctos.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/goglajlyb.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/grghxuumu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/glywcpnpa.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gjkxrhfwt.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gstnkiurd.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/ggvjbdgtz.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gqmerknze.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gmkwdkbao.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gnrapkpaw.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/geymdphwq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/guuntpsig.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/ggpmzdzcp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmqyiixny.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gqdnvqbvz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gwverpmiz.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gzmmmwctb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gpghlqtnx.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/glxuuaamw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gjwfvcpft.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gvptqirur.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/ggwsvhybv.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gukqgseuj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/glmpbsemo.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gqnoezlqt.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gxhemjsce.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gfieklevc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gfpnqfhgg.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gcqhfztbg.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gmcwwlvlh.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gbqsynywf.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/geiqrxgkc.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gmuqxlysf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gujzmzuei.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/guprdxnxm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gfnqjhtng.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gwgnbzabq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/genzadqhp.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gdajpchxg.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gyynpnwsi.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gnsqsxppw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gimstukeb.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/guwwuahue.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/ggrzriukq.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/grmkoqdig.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gwgmexbaw.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gsazvkrqb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/grsrlgqfh.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gzgrpinrw.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gnvtrkbbd.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gopptsclr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gtjvofavo.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gbuofpabb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gjzgygsvm.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/grigopjtj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gowqfqddb.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gdybcwgmw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gotmkxuat.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gzchygrwl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gqfxuvrfu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gsybunytl.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gwjswezia.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gmxubzpir.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gdfcxnclk.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gcqzjbmde.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gsuuweirr.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gwhxheswr.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gqtxhmplb.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gcklcohos.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gcwrklblv.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gaacytcxl.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/glocphhcz.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/genzydcpe.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gsqzyxoke.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gxfwlyrtw.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/grinyywrx.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gfdkojhiw.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gfydnsssa.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gddtnlfkf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gypoxiztt.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gdavvhusf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/glqohuzgy.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gobubilvg.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gnibmzojq.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gyoyqvwzf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gzpalbgmf.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gbfkukjnf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/guojwmnfb.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gndvifoyu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gozonhkea.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gzyogwsck.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gunkthshw.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/ghiklnhkm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gmyyuqsni.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gonkpegpq.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gfpwmdwun.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gdtnphusr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gqvmenzmv.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gtinkslfr.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/ghlwnflkk.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gffgsxvvz.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gopsbfypa.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gzzupgbgm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gtsvcofnx.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gattfxlod.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gawyuifvd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gzqapdaqt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gvafqlngg.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gzogwnizs.sHtML


<!-- 参考信息 -->