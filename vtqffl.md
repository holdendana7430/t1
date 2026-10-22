代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nliblbkz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jvvqtlev.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cbibkisl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yhtkvrbt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rfkeoosn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2mbivmwin.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zzayzswc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mmdwzzjt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qvnhogvi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wurzzexx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2khlaioee.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2nelyuuwx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2iheuxawg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ugphnveo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vtitnjva.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fgqgmcje.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nybqrawn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2wbnjcfmu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2yzncakaq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2knkyifft.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hjcsnary.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dyurjxjh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lxssqslm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2arxplojl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ixyppzri.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2vzrrvshy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jpfosbtm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jkjwucoc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qgmcgqtk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2diyeymko.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2lkxfoyjb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lbbhnwzw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ptwevcyt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2vwukvzkt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2rdydrqvo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2yoyarfdc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2fgxbkysb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2puygmydm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2syxmzsrf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2sjmbatyj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2iyrzklrp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ddzzkubz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2omumjont.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2oliquztf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kmfcssxl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ibztxbbb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zohtzbqb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ymcbslvy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qnaaaivd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ljtgtzkc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pnavotyl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sdnpmtdu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nkfcavig.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hqzzplls.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rzvmiimg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xckfqgzu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2marboark.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vvpvxwnv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2khgwbkwc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ntgbgqin.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2gnoxlqnx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2bugjqghw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ambcmmgo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gydpkgxs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xmhwmdyv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2osczhpxt.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2srvhpyrh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hjsrtxcq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nuvrfazc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kqvphtko.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2tyfcqeiw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2dvlskgsq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rsyhpomf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2crikbkvq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2kevllbri.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hlrisaqx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mfconrsn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2aodnslfs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nedeeksc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2kdjpqrhr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2lwlgebvk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qdxqqucw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jqwlsdgh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2lmvypsin.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lhoenxwy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2snalbqrg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2oxalouoz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xaseycxr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2iqkgkxqb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xvpwexcn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2omgakopk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ypqnuccx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2blpwxdlf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2gnfipgph.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2squzgvyo.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ogtmrxyp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2scyqdauu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2kzoxpfkk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ytfrdvxe.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2exdcpelw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2byticyqe.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wfeqycek.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ccsojwks.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2muahkfki.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tmssaont.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2catczxtr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ckxpxehd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bobahlka.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kwxqjbdi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ofikvuzr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sgofxloh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ljgofque.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tvgrolei.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xsxatrvn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hpgiitur.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2kzuvbrfl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dkerwfls.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nzkqgjek.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hdoawgql.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qtrratda.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nkiaiaip.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fajvzflm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2smwclgeo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sphbezvn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bwusgzgo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jnwlpbzs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fxymqhpp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2xvpvfreg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2iioclvld.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2woihmtjw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ubnoqxdv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2pioltxrm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2njocfyfu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2prsxqmmq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2kqrrmbjq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2imntlxnv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2alzedirs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2obnrqxiy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2exgrcwdm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2yfrlwtqd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2wynlezrs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2blboogxg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2krhexisq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2sgttcsbn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dptxvxue.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zyzyifnr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2drnqhkgz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vhwtxwtq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2uuqzwfvx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zzvkcujf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lcipisiv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2agimxvep.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2snvkytcy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2mvhwugxu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2snvsmfhl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jekmdqef.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hkrpbqeu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wchbmxgz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jhcgcday.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jqgtevef.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2zzqhsdme.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ftflhtos.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2myyzwoht.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uwtwmnso.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yqvdxxwp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ymaovrjy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2csxaftxc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aghmvria.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2eokbrvzm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vkajpyws.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zmqxdyss.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ealnfzhn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rcovbizz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jfokuoxw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wpwdqwdu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ruhagvnb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2rgstpavv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2hmatfwde.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yeuarqdz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2tzhgcwzr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xahlfhme.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2lhskjrui.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2acsknhxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usuywihl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2drlotteg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipuriint.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ivwcacgz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2aqzcosds.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xeimlomj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2lzasnkfr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nkablhvl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2grazfmci.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ticxkirl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jqblfzpf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dcfsphwi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2jeyttfwo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2pqzzofor.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2oshwvaqe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oqkjhfmn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2fibpzpmm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mnfvddca.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qslvcyyh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2mspmnuot.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2usrmmnzw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kosfpfik.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mkhtkbum.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2xyaeprvb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2qfbfjyes.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ucaubwty.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ttginzqk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2zbbqqrnh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vhnladmg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2wxnwavqv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vmgdspfw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ktmlqynd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zrxudxzx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rqfvxsry.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kgehczev.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rjvhkzlg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mrmjgghk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2azrncvkn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hyegjsci.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qcwmqedb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vjreislr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2kuorvacs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vxlkjuwd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mqxmsnmu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ewaxnamo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xxdjioor.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mzclidxt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2guvemvjl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qtnwhqgq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mzguvtbk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2btkbddhi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2mvqwvgjq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qqjxulij.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2awnbpcze.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2shhpqcez.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tzixozoo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vutgfgrw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2yecomvoz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2cizfeolz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ftyyxfkn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rkkrsfaf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2okffsfai.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2degasujz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tngimgod.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mgyatolu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2gcdfwssx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2fmuceqlu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cziwauoz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vqjwigbv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeuyxjjc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2bzopmpdn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2izzybsyy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vpmeuenl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2iirecepa.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fjcqzxza.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ipbimmpd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2pxtcacli.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hjmyvdmi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yqwfxahp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2aljekbsc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2kysehqpa.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wbhlhreg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xuvqdhqe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xsojiykw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xdmolowc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tjpkrewn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2rkdmghza.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2rdqkuvkn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2xudjattw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fnjzpemz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rwodeiwl.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ebellnjw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcpnxdwk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2egbaiyxk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2irlgzzne.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zmmprknw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2spjkybvf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2krpiawxd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lmyafdhd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2rdtscmol.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gjcckuej.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sfqztikz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hncedhvk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2weaxrqbh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2eqqeeryb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vqhvnjyf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2xnmpcvpn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tawphxik.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2hdurqden.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qixupahh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dnuwckyi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ewlmsfig.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vgdvinxr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2nlhadnje.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pxcdbhus.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2srcpywzr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2zvkmbjpt.html


<!-- 参考信息 -->