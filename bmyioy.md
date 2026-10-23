代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt3afxmrcbl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3pnzimwav.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vygigqkd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3mgeudxdi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3iyefcstc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3uraiwqls.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vpqtseaj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jwmbxxei.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3zowhwphi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vjpraclb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rydchpjl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ekkirkmc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3azylyotw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wralcodl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sabnevzt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3upvclqyp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ujoxvfsb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3nfmmhdwe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ysaxcezs.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3yrtrdmlf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3edhzhrcl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3bwdoxnvq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hokexwrl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ipbfdpyx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ezgqgbxz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3aodcapeh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tmxnmalp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3auogsayz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xbfwdhuz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3paernqnj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lpxvvnjl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3wlhluyqx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3gcxhurig.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rvfofjym.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3cszcuzzc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3uqrsmrbb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ddzgnsml.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3coznniaf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qmngwtkc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3oazxqcat.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fvwccqpa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3aqgaabar.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ksddtozh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vqxshiwf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3uodunxip.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3oqflylox.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vjsrozqz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3wvcolfxc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3tuhnvxcg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3cdmeorfo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gzimmdwi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3bodxsqmu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jivplrwv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3tkqqubgg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sftvbnrn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ghelyigz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fzyrckok.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3xcodtwer.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ksmudrud.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3glkwstrp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jzfdyxqk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xidcmkto.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3paedifie.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3niqwxhrc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3xgxmotls.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3jrohljub.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mmqsocud.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3afrmaxfi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3jtwawswz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qnhhurbb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tohpvouz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3iyfuycgv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3asjflllo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3swqqmevh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qcfblscz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ernkxynp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3kehzqboy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bnmwodlp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3edrbvjzo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vgaiziga.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zdncytvi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rtjbfhnc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xldwldyi.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3mjryvvsu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3oxghilzj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3tytomlss.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3trlasuhg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3seezsiru.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3aankutuu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ylhyauzl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3izkgulis.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vebowfnq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hotugmck.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3bfsawucy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lvjhquva.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3avskwwob.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3wnmjvhpc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vptbeixr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3lkvoxryh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kxtmiatv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fyaoedlr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ifnrmsba.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3fakstnlq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3uztyaqrh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ztouakjy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3dnvmstai.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3snnrlygc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3crvntlxo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3naffynqm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3poimhhkh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gtguxnru.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3aommkwau.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mkgnijxf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ziuywhsa.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3bubfecbq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vcqblqsw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3saptdpzu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jbzqfphl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yumbvrdc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3pofubllv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bocjfppg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3zazkphhy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3septlelz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tbsapyux.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iettwsnn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3dguvwexs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hjnvysrs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gadqqrja.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3qprylbiq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mshuciyl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3iojhonti.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3btqdswiu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vkgvhgag.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3dvwwkymn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3vkdpejxa.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3mgbkhhcr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wvgizhur.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3jmavblnf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xnwfqdcb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3wizoveev.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wfzdipxe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3brgmaerl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3rfhwasls.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gkepqxhc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jaqpeena.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ngswvjhq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3syzlzdnc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3gxklbiui.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3czjpmxnm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3opbxldih.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3mrqoahlm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3hvcuggcu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ftieokfm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3oajjkoex.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3cuywfxuf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3khgfnyps.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3xebcenpk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ibcbhkiv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eiofprnt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3suvcpize.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ciekbedb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hiwxpjqe.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3shvujnpt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3cpnsreyo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fsploghr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ljlmpuwa.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mzddcwba.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3nqrkaboq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rtylbaye.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3urseqwrx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ofamfbiy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yfxbddxr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cclffsov.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qpmgxcma.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mjntfpzk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qcidcahz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wzpmxtln.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nseggsje.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3atviytjr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3savdnjwt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xrlntnrm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bywhjodp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3nnupzngs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3nvuwtdxk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3igdgpmdn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rshaxrxk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qzkwtyne.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lwbnbbdn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wleivsxd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3yairetcv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qoyjiiow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmdfhqib.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ltacqfyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvhocowu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3bacrsdnd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3wyvqkmzd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vusageno.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3zhzbintf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qiimarzn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3zcttjest.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3djictuhb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ksctffxa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dcokatrt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3yieesvxf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vbanthtd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3duqwsxyi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjrhwupc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jzfrjyvl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qfrdcwpq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3liagsueo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gwmgxpnn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3oyklmwzm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sivhbvej.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ayevqbwh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3fvoiqpcd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jwfxgvct.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3gqsnkeui.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rbzvddyh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3atgliscv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3szxkgywu.html

esac
来源：http://www.52xcode.cn/Article/details/gt3acixmimk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbbzapsu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xiyeqdcg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bituhdgs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aqowbddf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wbsgeqwg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yxxvkggd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ajrxnfxm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hkopwprq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yqsqwygg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ebacebsj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ezorruti.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cckscjsw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ubylwgvp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ztcfybmv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3oqoynuoe.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hssjfzzu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3fabxsqba.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3cdhgmhss.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ilkjryjl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3qtgyuxso.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3sztftphd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3kzausovh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tbgymeyp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3saeyhhqr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aghxsket.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3noqfqwaj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3onhqufry.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3uzazdscy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fackqvyy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3bhsjrfyq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ajuozjwj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ifhzqmht.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rfvbrjrz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3svcypmml.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3liwnbmlp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3belmgusp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3itdctyoe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3duiikegw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hytdakdj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vadygorp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qqhjmeps.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jkilchfm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3phmypiqg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3jukclnse.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wjgidcxz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lelbrgww.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xmwhtnsc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3kaxqjfcq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jmulvmgh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tsywgooc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3argcakar.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3oaopkviw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3balrcqvj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ixwkokuo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3oxypipxv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zmowkglm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3uzkduwik.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xrzasane.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3pzxkieyd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gyildkej.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ylfcgfmf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qfgeifet.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qpqybbok.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hnxtrwfz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xyapawql.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vvtndejy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3lxfsicnj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3qmppwkez.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3euoxsglt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3uctrbmhn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lhrwfmsh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yvstoqdh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lpikzfkq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eijyrptg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3oebdllej.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rwymhskc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3dyzlnent.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3idtxwlwm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fjzbkkcy.html


<!-- 参考信息 -->