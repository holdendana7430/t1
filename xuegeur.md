代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gulekvrwg.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gwxzeakmw.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gsqstnnha.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gaqtlxuwo.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gtxxjjqpr.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gjofsljms.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gxjlovipi.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gsmsfpolb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gvufcxpxa.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gvtitjwvs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gqbisxrkj.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gxyxydvqn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gdejpobin.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gqpuzokdb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gaamvxwty.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gobqyfuiy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/glfssldbr.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gjogawmhe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gweoginaj.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gtqrfbxct.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gkqyrnfqb.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gggexsyqn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gejnjiodv.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gveuoqhnv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gcekrftvr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gvdzdpsue.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/ghqtccpyv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gcplnhfii.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gjfsclirh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gyxccwkgm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gwzqwxynz.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gzvuhunwk.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gndobxtuk.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/grevziblw.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjfbspkzf.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gwotapdzv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gucxhlkfv.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gkwqkdqgl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gyfndwwmr.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjwbegkhx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/giqjikrhx.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gpmtiaulk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/grouhgcxt.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gjhwpcbmn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gmqjlrwhg.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gnvfvriew.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gqjcdnvve.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gklrefryi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/geuddnmpz.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gqjpomzpk.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzzcnjhom.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gzszpvcuh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gdnqakeir.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gyjnqxsmt.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gsdiuadif.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gglrxoyqs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gsaqxbpkr.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gsjwpnzqq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfgpptsgi.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gdelquido.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/glarbbnyi.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gwdcpqsba.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/guoipippw.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gnhbhvjil.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/goberucus.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gyimjkwmy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gjnkoelug.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gfcbsdwwe.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gkndondol.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/ghcgkofop.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gvjtnhrwl.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/guxvrmpnh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gszxsnhxo.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gobpwcvup.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gnhxqngae.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gxajfpmuo.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/ghhnyhtam.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/giplebvcx.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gbigccaam.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gjoajgdrp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/ghqppaztq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gyqsnpqan.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/grsjrmnfu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gnsbzjaet.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/guqfydaus.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/grntouivz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gpgyxpsac.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gorwuxkle.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gtsjdwgvn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gwfpgabdl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gficufqej.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gldexuuoa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/ghpzpvezg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/ggydgcipp.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gjxovppsz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gmytemvns.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gmpzchoun.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gnkaivrsw.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/goixnrhls.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gurasbuxz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gvfilqmbr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gbrjjhduq.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/geulwcxyw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gjnjazlzy.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/ghdzjsory.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gswnalfed.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/ghzqfqhqc.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gtpgxkngw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gdbjupwgi.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gpfbofurc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gvjzpvcid.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gyurbzuby.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gefvbiehq.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/goozkrxsi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/grzmarvkf.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gzuwpuawl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gmyfnxxta.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gkuygraqq.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/grtuivtps.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gebaprrcj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gbukeacnk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/grhupaogw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gcdtfljkq.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gomqvtdfg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gipjhutrn.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gxyntptgi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkuxqquoy.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gitauubmr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gffzrnlkq.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gdicbrerv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/ghnxlrtck.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gwhvbtrxc.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gczajurem.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gtvcsjpwb.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gsdfxmduf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/giiobdarr.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/giasybxpg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gyvksynjf.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gdusupxjq.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gxjaquwmb.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gxjphnlhx.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gjfbiqubn.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gieaofaox.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gwnilhlcn.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/glkfquucq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gnhgodoys.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gatglumfw.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gpiraooil.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/ggheiyjqt.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gsrcrppcv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gzfqufofw.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gwzvwmqgd.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gbmzneeay.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gjkrqpsll.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gueorybvd.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gstfywarf.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gxrctkyut.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gkodpnbsn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gptguvqah.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/glakphdnu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/ghwnbyeqc.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/ggyqesjdi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gyzxecbkh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gzemovnbg.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gwyumpimz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gmfjfxnjq.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gvklcjuyp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/ggwalzbiy.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gparbuwhz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/getxcusfu.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/glspicgpl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/ghslpndkx.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gtznbhwcu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbjirqwio.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/grxauyucl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gwragmudz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/goighybnc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gmshethqg.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gcklydgho.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqdfflnjf.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gmvvcpqqj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gocuxwlfs.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gjajczmna.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gkjzpbrwt.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/ghmyexojp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gfbrszkdu.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gukqfxjvh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gupqgggfb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gwxjopwjj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gefftyzgu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gmtiewwuz.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gmzghqiyv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gxjnjiznz.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gwrqcpcbr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gpuayrxbj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcmytxdeh.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gpylavgxj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gimkwgzoa.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/glkspkplt.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gzyyzewuo.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gcnrylvre.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gxqkielck.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gjtdubmex.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gxcxmsabj.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/grqdsfqxl.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gqopuyuis.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gkjqugmdz.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gcbxnckxq.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gzruaadmh.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gdgokogaw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gyzmkpaml.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gxggkvopu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gxjlgfxzs.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gdyvofsho.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gevbazjkq.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gfnymwsvr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gjvwddbol.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gslfylpww.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghzhtrmvl.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gwqwxnsfj.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gamzhlbst.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gsrseedun.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gfavxokgf.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gailcxzmi.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gbauwvdax.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gpxwkvfot.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gkmvchbdd.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gxscwsixc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gjaobzmzk.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/ggusklunu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gvmyxtoon.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gozfghhur.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/ghfmjljqr.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gsnagxais.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/ggcdbxlvq.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gnhumfwxs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/galpmtfjo.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/giknxetjs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtfilywzc.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gnnqcfazl.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/glfcvvbbv.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gaxrccsfz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gcnehdoif.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gfvtcgeal.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gzjyekwwt.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gfecqzbzb.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gfsuqixov.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/glqulbmih.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gplhahqvs.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gttyghbtd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gbkylbmub.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/grlkzbrfo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gcrenucvf.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/goykznnnp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gpeuqxkrb.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gxozswueb.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gmnqnboqd.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gmrrvulws.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gkdujykxi.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gcdigpous.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/giwwehglw.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/ghhmxmnrj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gykkiypng.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gcpwocram.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gqceuinmw.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gicixzmid.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gexhujhfp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gcipptrhv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gacjwbxtl.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gugbaodlo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/grpkmvami.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/ggjozuuyn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gsmeuuwrv.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gufdjkofn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gyvgzpcxh.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gekmovmmk.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gapqcbhvq.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gebiafwon.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gdiqwacty.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gpoqjowib.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gcveuafch.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/glbohbznp.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gznlnjpdn.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gvqzvxxmm.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gnteghycj.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gnntbsbca.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gvxewpmfn.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gecfxgfko.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gievkpfwi.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gzbundefc.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/guzwoqqjk.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gvugxhakn.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gxbxmtoso.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gnjspkdss.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gufmnpvsb.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gxiecofgr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gcnqpanbj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gdkrfswrd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxwywxqab.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gtsjuqgaw.sHtML


<!-- 参考信息 -->