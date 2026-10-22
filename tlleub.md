代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt2wtoyptgt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zsfrlqev.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2lkkhekqo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2iwamlzqx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tjfcsodb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wqizjxeb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2rmrrjrdr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2qedsktkj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2jyccjqaw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vskectlg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2eqdjptlo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2dyafniew.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2eplbsxui.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2fsibwsfq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ejrkxfsn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2axgaogdc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bgucucgg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qpqtfzqv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ajwjpbfy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2kcenfqpc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2nkahgzyp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2dfqaytat.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ssiatmmu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2berijfeo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2kpudxviw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2criqutmh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2teycqaka.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2myqsdtzi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ktzwllmm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2tmjmycay.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2exusbyni.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fgoctzdg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ngpholtj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2clsdrlop.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ttgowsty.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2wxftbxfk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xvozuhnk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fzugxeeq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2gdewmsxw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rkvajlyv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ndtcehcx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fkfmzkdm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vuipjryv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2rdrravdu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kzuthoih.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jxwfhgun.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lmfyaikt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2leqrauky.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2uwmfvusd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2untbiart.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2invsyqfh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qjymazhi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2szlpqllb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hbluspis.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gyfpemjd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mewxlgji.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2udlpelvb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hygohovb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lcrqnkwv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2grxdlkcc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jxzvojkm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ntixhpsh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sguitgcg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2cbcpynib.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2cfmkfshj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2djzvdkps.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qljwhcbv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zuzmsfre.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ofllapjo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wxoebefz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2jwxyxpde.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ibdrcapd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2vrvuiojj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vqxvtflt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ffcixvqr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2utzhnvdx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2wjtdxmgd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2nlizcpdp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kukdkykm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2mcmczbeu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ihjxfoza.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2pwptvdlp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2efutnffb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2iaaecncl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vrfdteem.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2utqacuam.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ruplvrsq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2pdlgixeu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lmawqtgc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2smsvublb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2atblhyus.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fdxtetjp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vxsuwbjd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2vicefrkv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2plhkbonc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dotvkics.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2duozdfab.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uczuwyed.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ujhhnajg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2jllmuwmk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dsjlnwvm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhfdkbr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ytsppbdo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nphzbnpu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2toexduoc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2aujcphfq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2othenpcz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2pndvyoqg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zaoyggli.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pspbnqtc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ycralpgp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2iulhofop.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rgbirdka.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2kqffbcmd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2mcmfaklk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kbsrulql.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ottfevcj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ltwxfgjw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2aqvlagpa.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2lerwpkns.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rertqzfx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2thstvupx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ebafkubw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2onsaezbs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wuaqurtp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cbmaqfaq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2eapdnylg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sjewqnht.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2syysdykp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vwuxgfme.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2odwhtiiw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tlrcdjjc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xbnhedgs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2enmsfxgp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2sacwbbhj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2bhtvlrxy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xuylpiiy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mfjimsrh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xeuggyyh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2luopkvpa.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qjmeuyad.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2udcdqmrm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rypsdept.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rscpcbes.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qfesouqq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2esdvvpyn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ebicvpqr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bqzspgyt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qcikclft.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zthlvotj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qnszxckd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2yejjjwsr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jsknfhrw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2dkgotetk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pojipnpc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qtqnadvk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2omyjtpar.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hcdaciwu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bmimkper.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rsbbkypn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2glkdrcdx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2lhtnkfvb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lfcupfou.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2fjtlxgyu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2zxuuaqxr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2cydxlstc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2aqokibjk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ydxjmwre.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2kpnksgjm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2plxmnwzo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tkfaawib.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lelrgglj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bpfrbvgb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iktszitv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lbxdejlx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dlzdjsae.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uqkxkplc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2acsdyxtx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2zeqlwsbx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ivxutdaz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xslaglys.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2lxlkbatt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2axaxprxe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ugzrsfem.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2kctpinoa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rxwendoo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cqxpwqnv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bofchmdg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mmczvtqw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2orldqcag.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ihsuedcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jaouaepk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2pkaolnav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtnusaix.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kkgsmzfz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2qlkcwzpo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tnufqqcu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2blvaznhc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2skfdojhx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2bnuwkxiz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ewveofjs.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2feuqyemh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xoikjhju.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vogqaklu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ftjwfdlg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yvafpwfi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lnjyvyzb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2llazmpie.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2bpzsrxlq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hfftlpfn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xqatqijo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2otbifboh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ckladoru.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cnwfpiqm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pljmjvst.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2cntbzqfp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wwpzyhgn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kqrflsre.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pgoiwyca.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2olhutkeh.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jjzjtyxz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2cfqunaze.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2svzkrlny.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2eeearjnn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jhzqweuu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nyufjoyf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hymslpvq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwbhsuhs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2tbhyrkfw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2aheppbyz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2oismsbky.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ksalfylp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wfnzolxq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2yaeeduli.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jqhynctm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2guzuoxze.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2bqpojflw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ghbousow.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2mfuosmcs.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lsewaqqc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jtmymblh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hxkuhnls.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2bceqrjby.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zfxslbqn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2otydafmb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sfbutwhm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dwvxcxkv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lqzdumcw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2psgwhlvd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vcbssgfq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2emttvkbu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2aoulornb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ezykqpaw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ytciauom.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ditogmdf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hgunghhp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2oaxsuzmw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hxkqfxem.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2zgonbcie.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sdyfqavx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dondnhbk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qnkhgcyj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2brkblhij.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ddqtfvak.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2guwtnwnk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2aoowdrlj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zmmcljvu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wthrxplb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2btdyzsmj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2itzaggsa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2sqncvffi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kspxkbfx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bieqvydf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2zcsmjhvr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2uzxlstxb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2fcewiuvo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qefyqhun.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qrbvljrh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ibfjwamu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mivfgjoc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jsqgglso.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2xxibwrra.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zxohwzig.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rnouggmq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vgsburai.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rxukhtme.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2azeekpaf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2cpdzdtfy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cguxiosk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2bwketmzp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2iwuqcxqo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2kauppxqu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kipowetw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2itvpmryz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2poeydyys.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2umpadsyv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ipjsahmf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zjbejesl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2idadpnoq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2lwdxacmj.html


<!-- 参考信息 -->