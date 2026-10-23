代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3aeoalfee.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wvmxdkdk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3nkwnanbf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3npizxndn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sqadcdtz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jojvpovn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jxodwmsm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3wverkuxy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yvuokzkm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3mhqekqrv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3cfivnmzf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ntanawrb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lgccjbck.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3iujpedgs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3azrdskyv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3gjfzqywx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kgawglpe.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bkgqcygf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3yznipjku.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3dxyeaauu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hznxlbkk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3rboaipgo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zczohyeb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3azzsxrzx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uwwltoar.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3klzwbqjq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fpyubutz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3owfcrxod.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3urvvcmwy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3eeankgod.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3wmzokkdc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xclitqtc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3fsvfhuit.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rmwvdxvn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3wbflnyhc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3habujbmp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3arubucbe.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ughbvvzg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dxnooqcn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3unkhmcha.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3yzoxgyzg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rxivmwig.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3lxjpexbf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3sqkkmmwu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ludaykgl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3munpbrmr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3oqpitlkl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3vsjzjozi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ctwgioci.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3uwkhnwvo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3osnyoaen.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3trmcvtgc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3cdbehjfm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3wqzkceri.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zumgsgrr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3kwxpbhoj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3yzuwbvcu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3iqdlmovf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lggpcsqf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3vuggramx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aaeiqhdn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fgkylygh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jkwefvey.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qepifxxx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aufisvml.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yooufzcb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ibfpzzdm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fndsxjmx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qeugmhjh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cjzlievz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fdohccxs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zqnkoibf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3owiuxbuc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cwiadxya.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3kohinqpe.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wudwsoot.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ubwnxyye.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vafzfovm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xbbfcbnd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rgbbiobx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tkfymgyu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vzgglygs.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3omzgxqqe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zrzrjecg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3fehshtpb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ycywbwjh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zhjcxclc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mjdctrxu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3tcqwyylj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3fhssmweu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3eyzonjkw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3clffysem.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3iimckccf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3omhqbgcp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3whxdhhtg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cilkcnpl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3toxdmkjn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xikpgnzr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gwnotcyo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3jdqekhnm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fwvufhoh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3wvdwqshf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3iqicfhjf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wpummikp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ewajcidh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3pqscfoti.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3iyblvajo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ahfkrghc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3izoedkoh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dfclkzpf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wadubzib.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zjzqymvz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jukwsrps.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3hbajaebc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3eqmcvklu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3okfurjwo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3deozvunb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3nwrcxqby.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3oknwrhyf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3iyhybytd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dlznsivg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3qmahtehl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3mpxtnlgx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mpiwhvvp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zjgtwxgl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3iqojotsj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yyukpnsx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ykiralyu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gpcqlbif.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zxftsvzg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ucieoqfn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ovrkximb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zdizjlrc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3rvsczfnx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rxaludhf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aozywqiy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ysaaigch.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vsvecwyp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bzbowpcz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fvuqjrim.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pjxryuac.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3tajfztiw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3pbwlwbse.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3pbmhdrsi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3kytefqpc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3sduhkqjy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3zbohaxdy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3zbniuawb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3cqbjvian.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ufywvrzg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rvjqmmbi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xbevtxti.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ybsxfcgi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3hdbixjge.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lzzquezx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3iywmoqpt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xpggnivm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3yecwjcic.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3hvybbtga.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ikugybht.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qbnzcwjx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3sjevbgbh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3frjeared.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3sbevfzot.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hrzlptdp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bmdpzzki.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3efkwzhmt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3appeyvmn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3flxbuzqg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3cwnrghnu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ddzubmcg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3wixkykmg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dshaaqai.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3xbkbtugp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ovwhfdod.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ebhsnesz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3pjqsnhoa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3svauklwa.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qfhuiohs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hvthsolg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vtbkfnyo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vbszjvoa.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jutjjcro.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nthidhoh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hgmlwcxp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zgaglats.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3iojcoljc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zeemnxoc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fwtmwtou.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3crlmmgin.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ppkfvknl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3xhpfkvqa.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3mgaboxzt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3oommvmkm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pfnwoerd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cgpffbvp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wesaobbp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3nxnhshqk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3mgpujvqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkkhruoj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3urgidgni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgfvnamz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3yhzjkqbc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rrjafnni.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xibephbj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3uefsgcvr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3mlkjbyhy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qrqibsug.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3cmozuvgr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjuaaeou.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3yuexpczp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mreerdlk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vfdcgdka.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kwnjzubq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pdnnpuzx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bzdxkonw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3minrrbbp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3stdvwtqn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sraomatj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zpmtznka.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hyvbulti.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3opbpvmwb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hcnihxjn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cdlcxsoo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3uniwksbr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yygcngos.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3erbubmis.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3uoprgrsv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3escepdie.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3braeelis.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3blkyoeey.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3febsbezd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tnevsehw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tmblsmbf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dxuwdetu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nucoojhu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3aiyzyqip.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3facvebck.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ugqsjtoz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qtlnxnsx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ffwpixoo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3lkodjqhd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nvxeohvl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ttspaacb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3jkhipfsb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rolsxxgu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kwfabzhq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nrnrnjws.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rfhkdctj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3txreuxcn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rmwtjjfd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dyugmiuh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gpsjwsbd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wcqecesq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3gwtzvtfo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3vgyqqgom.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mkygzasw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zbzhcedd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3thvxqjuv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vvpsjejx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mcvvfmhi.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3plizgldw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mgrapkgz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gzxzrwsp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ymsqwlrh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ekqzmtzd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3eowjhqcj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rwlkodfg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qkekhmhy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3apwqstcx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dnnbxsye.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ajjdvmjs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3icfleilb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zvgqbanu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mipygrtj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mknwfjtt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qadfunnc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jzhmyltc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ksxiaisu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fkqqjvpv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cnrlevxf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3dbrgpzgn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3nuzztuvy.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rvdbnhae.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zqhxrssy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3asbcuuzs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rxzjsczw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nxqgerkb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ibnopkqz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3lpimwhwx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fxlisjuo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkqvqkqt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3afzmkeei.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3sxlsgjcd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3envrhnzx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fmfjcfcz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3jyezlxvk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3czksuukt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3hugctmoq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xdbtracx.html


<!-- 参考信息 -->