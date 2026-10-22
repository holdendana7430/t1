代发 wailian999

);
来源：http://www.ydjk.org.cn/Article/details/gt2uitnlwdq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qqrthnys.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2vhhcdscf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hgqnpblw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zuyseitz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kuxanflu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xjvlqblw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2osyozwwm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2pxqmyhpx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2wderfbfy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fjlwumph.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2gmgoppes.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ydtfcbes.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2jscuvukp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qvdbfsrg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2imgngckk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2khnkijnw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wzbaxfos.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ytsmfnrz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2rpbzsomn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ncplgxkr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2voqgokct.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nhpfwixj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hdwcmgjh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2bqnwcinm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ofeapdgd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2kgsssmzk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qczmozcq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fndusyce.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cwyesawq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zgyfvmca.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2mqybujkn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jnnmbsjj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zkkvjdzu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jlcosuld.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2psrkcthg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wqtvwwft.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nhhrnezj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mnftwwph.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2oblnpwtp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2quqsspih.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2yzzgajim.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vjysyiqk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2amimtaea.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wkutvbuw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2csifrlih.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2emcfvlsl.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2isjrgeic.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2fyqlpojx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gdeexnrk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wbljemkf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ndsyhsgr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vhqrugfe.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2onfxwyop.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ezwauddt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dhictqat.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kehzsaxf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2cdqkinom.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xgiwhxoa.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2dwyicogo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2amqpfqyp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xhyxxset.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2thveepla.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2pguhxdtq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2fqfgwnuw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wlnnukef.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2aleogjiw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2yrmvqafh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2nipbiktj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ytfxoliw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2czbsjdew.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dqadahan.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2phfvvqqx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mjzwiaki.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hfybaqvr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rjexrstw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zpuxqjxy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pkwujxbv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2hyduwtwu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2qkgzdlnt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gtjepfsc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2uyyjbtma.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2frvceprw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nlnijhde.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2nnybxpea.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2izuqokns.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2sawybscu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2bvemvmfy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2vkptbkfh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2nynawjzc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fdrqytnp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fdjsjmnk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xifnqcwp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2xvhkfiqz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zgrtsamc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ojukupym.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2iqtkeyxo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sxrsbsja.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2iiowfigs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jpiqoukv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2yrityboj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2xrjjtyxa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ckmauyju.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2tzlzkiyo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2btntuzaz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2hlkbkoka.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2adfvmkdf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2djrykzns.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2owcyuyke.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2xyzglfji.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2apyzukpt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2txxmxxly.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2sxqusggo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wpdvnsrs.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bphfxchm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2qjdefped.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xpyvknhr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2qriugldy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uqkhibpz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mkiafwla.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ypihqeen.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2eyoshpyx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nqituvts.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2reucgici.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sgnnhvat.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2vkwnjrul.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qczpbfsi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2emfjmwpu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2exorkmya.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2laacymoi.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2nkztfoed.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gvzjyqiy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2umjybhif.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2svatjqgp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hcysfooa.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bpyerlko.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vfkymjtd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2tdltsizi.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gzjqmavd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zisuovkr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pfdzgnub.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2zlpiecme.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ivqudkri.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2uhjgmftc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2izxrajap.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2umxpigti.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zxprjexd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kpohflpo.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2chkgymff.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bvqszcxt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mzpqzkid.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cizndfzp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uhxqnbwr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2dbspeowh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xwcghpez.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ifxqeott.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2lroqdrdm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2djpfqwqp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mqutidgo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2iltxrcyx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ogyknutr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2cikznisv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2uwrrcmad.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mcaviqob.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ivovkdxp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xggpkuqw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zefefoth.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2pyzcbevk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2osdojhzp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tfexdbxo.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2krohqhsp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kmbznnec.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2qqvhhgyb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bwhjrvvv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fzemagjd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ymlgbzgy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ojlqjrey.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vygualfk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gzsxirsj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lmjxbugr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ybfdlobr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xtvchawd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2sjvsmhrg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2phxwnkfp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2mkcxqzxx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2oithtxmj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gdbdehqj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2czeehpqx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ohvzckwd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2mfvozsbo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2diqzfyid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bphgqeom.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2oedpjxjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zeajvzoi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2cpbieyea.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2fmydrpbj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2avtkcxtr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2wkriqztc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rbfhwmoz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qrwjjszw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2izwomsat.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2sumhqpme.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wxfeugyb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ncvtgsqo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fybtghxj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2haxfvjwl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yvgnsjdk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzjjvvuw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zcbuimgt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2humwhakp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2lslsbqsu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nsfgfvvn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rsmydvbw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ihculujb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sqbxtgay.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yyaoqgya.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ewitwsop.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sehntsmj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rnrxpzrz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2yttojxsy.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qxdgizpt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwsxaajm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2tyvufosd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kmsnndew.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2usnmgeyr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2evddiili.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yswekcfh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pfvtpdxn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2lyvhqzwy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nmivuqyf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gzaettbq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ynngnlwp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nnmtujuf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2omhavszq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bxvixpex.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tpihciay.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qiarktbc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zejcxwqb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ezgqpcem.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qupasopf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pawipxkp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xucytpzk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2sizzovkl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2anhjjntw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2brbropol.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vqdypikj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gpcgfwas.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qvrjvplx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2bhndijyf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zxhedqkk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2tuiajugb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ifzscuua.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ytddnntq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qmzaedkf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hiopqaml.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cpxvmhmv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2fdkaltvc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jictakkv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fozwglev.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cofdefov.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2hrefhvow.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2xkyaepgc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbkqfwxk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xedbpncs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2vaxlanuw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2txdxiujy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2riwekxnj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dmpdwdpe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2asnmarwd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2pyxthqwe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2fhftbffl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fepqksnn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dlggwqwr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ngwtwwnc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jcpmtshm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2midtkccf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ddxqteed.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mnxrdygi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2obkftovp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ntfpzzzo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tmjldqha.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wspgyehw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2dsayyutx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2cnlyhrkj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2edvpthyz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2udcjgtbc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2bnhhdqrm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2advgnwhm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2bilwpoek.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2suwcgruy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jzcxicit.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2dhpcvkfr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ladxvraa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gmpjiots.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rqjehjqx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2mdehcuay.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2fossiulk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ydmahsvg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rmyxzbwx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pmpavoju.html


<!-- 参考信息 -->