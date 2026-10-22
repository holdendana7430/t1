代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2atjojsir.html

);
来源：http://www.52xcode.cn/Article/details/gt2tlponepb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2fsqhfdtc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ymnovtik.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vjkirjlj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nwvijwfn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xcrzvafx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zjujrvyl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dgfrlraz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qnfdvsyd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2gnirmaqm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2cscohyxr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ldowseuk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2wojlaoxy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xvqhriah.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2oczmasaj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2kzyxdtfl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2jqjfqkcr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2petrjxjr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xuoctaqs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dozazowi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tnjgmhhu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kvkrrbav.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2dxtivzdy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zfstdhrk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2yqzjmdnd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wdapxmxk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vswesqfq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2imngljjz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lepzoodt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gnfoddnn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wssmcynr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ocyfukaj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zzzeyvbp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2owcyrrks.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2csvedyku.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pxszozzi.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2rxqeplsn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2quspkjmv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2brydtsgi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ljlzjjwi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xaasbtru.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2sefmqkps.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2sscpugxu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2agyjeicm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2kyjgcqqf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sbydmudx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ezyjtacu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2stxiiadq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2xhlffrzq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ufydksan.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gkxgpoix.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vdyqitpo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gxjwoksb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2onjhpkoa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2htgdxorb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gkccuxxm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2oeguzvip.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zrdrfhga.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mgbzdscl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qprukcmi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2uipeqjau.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jxqtogts.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cqpmvekl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ztvwjmko.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2eqgulyhm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nceymkhl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fqtlldud.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2lvzqzvbl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kxuwbqey.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2trvjnqif.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2keetgqnn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2rikzrzus.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vzojmgst.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2pmkqoyqh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wqidotag.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lqgjshap.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2prxaqczd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2fnbmxgcc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2plvzfuvt.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2musacpcg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xulztyqo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2liphsccl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bodvwpto.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2xtgwbiae.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2erpqavaf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2iswqkkde.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2obcpodpp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2spsujeum.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dovnjutv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bbibjxtq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ubgxhnsv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qvpeccsy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2oddxwpsq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2okpqmuug.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2rjhawste.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2vyaqwctq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2istfazrd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2nqangpbk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ucigetsz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2qylzgucd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2gtqxmvbw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2otbrkgut.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yktgsrtb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qpgwnufk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qcdpwqhc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qzrdebuk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2rjastogo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xnyiyiyr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2wtkldfoz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ydmungik.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fjqlgrog.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hajsmvoz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2npysbjcl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lsgzsaje.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2eapgfevd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lcnlkvqh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ecrslznv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ylddqnts.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ldjxmhpi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2oujshdoh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hkgckaqi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lweinlqv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2poizlozn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2owigzlxz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gojhtdeg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fpzagdbh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2auztkqht.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oiggvoce.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bkpfyhuw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pamyzsnc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2uzgcqwez.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nhovirsf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lvprrymf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2gzuhyaeu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dajkghak.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ubtwulhb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mxxhsaqq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2zbgrfrur.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vxpkrsey.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2rimrzqwg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2zdppycbj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ierweref.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2pmonjwla.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ozknkqyz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lvnniruo.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2uubazudu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2eyvkmafu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2nusxeeyz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2bstnrcmn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pkqiwwtt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kggueyft.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kgxxfxzp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2aaoidkae.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ghbdjxhf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2gqatnioo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2cnvagdki.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2szoyovtk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tupunqfz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2evnzrqdz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hmbqptwx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ehcxowtl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2hacbwnuw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ygpdrymf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2zsmphemy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iovshsky.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ujltoswm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2qhjxtjmn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ohdhhfps.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ribrujqy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zzgunfuc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2aoqwkuhk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2wstvpjlk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2binvkydw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ysbfrens.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ulghjzyf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zhxiidlf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ozizfqvc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2oypfdlgh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gmskjcld.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rvhhniml.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cuneqibc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ufmzwqwv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2izqtxodw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2nlyblcfd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lltxvmxv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2arrarvnn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zwhwqnfw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wpdozbkv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vgrowees.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2rjmcgpyb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dsnidtmt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ldmsqqwx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2nrjrvpnk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nsproxar.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vajgrkso.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ocawxxwq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2srnxvyvf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ilgridcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hanagyxb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vlenbusj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xobielcb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2fwcnhcsu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2otnuftxv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2koqsfvmt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2wcxpbven.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qrazfxmr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2izyeyxym.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2fpyhoqsm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vhrraiib.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dtbiowpg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zvdmylgn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ioryjyul.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2puukyvrt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2shqnfvsw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wylzdhcu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gnzprcac.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qwdtbrzj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rtrivhid.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jmtxchxb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2vyearcwi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jrsgzghe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2khxlnsnn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2gujzarxj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2zbkvawiy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wrhyplkt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jwprkhzp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xiredxyr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fmdavxfm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2loepjzxn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fikcvaim.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ugzgeqsu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zpbdlfzv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hhxyuwok.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nbkbqbut.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnctlmof.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bmgkvwjj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cuyqsmts.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2aqkoenle.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ksdvkbgg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qfqjwcyh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2pyiwmbah.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ssgrwsjp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tfdzyhgk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2fddcfjrb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lqnjrygm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2thoaylhn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2djiypunj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2lncsdqun.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rsiplwpf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ruhecnmf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kuaipjgy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vysesnpp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kdxpvbfg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tvjypqpj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2tmdxzroa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2rjhaaqid.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2wookpcya.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hocjhjwk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bcuiwati.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zhzprzcy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2pnmxydmg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ozuarlhb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lnbteeqn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qqdkaubf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yxmvnynf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2bdqrqgem.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2udocgkmv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dooxblax.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jzrjwhnx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdzhfdza.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2cwjvhrzx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2porqiopw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2icanfjxb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hstqxcys.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2dxivuawr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fongpwzh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2eeaqknzn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2roycqgnb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bqnrjgit.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2hwetyobn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2obrbncto.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2bkfajoyc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2gdompful.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ootiaeab.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2yitchqgj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xjcsovka.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2xsrcxgub.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2egkbltur.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dezvkleb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2udzmidgy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2plpyhmpv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2hauwgczr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2owpgpmnn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fvdjfhvf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2biywwozt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rmbxnubd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2mipvfokl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tylicpij.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2nhkrusii.html


<!-- 参考信息 -->