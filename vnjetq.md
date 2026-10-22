代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2jydshcrb.html

);
来源：http://www.52xcode.cn/Article/details/gt2rnbluiaw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2isaqbnbb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2htibcnsb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gqcjdlbl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gwzsoqdx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ttjdyynf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lhaxbhvt.html

);
来源：http://www.52xcode.cn/Article/details/gt2awcrkthy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2aspmsbhr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2vzgyvwei.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zbnsekbg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fvsqwfoe.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2vfqrrrcf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2snfbewwq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2bjniycum.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2wpyfxpfy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2kunxcign.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jebduoka.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2oehksgsl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jimontep.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ohggxktp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tgpholbi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2gkwxsuku.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2spuzpsth.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jcnsmasl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vgjswxfb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2oprbcrab.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dasntlvf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2jroxpwvp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2txrwojcx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2clnjncfi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zwnsnfjz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2iaougshp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ilobgveh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mhddodyx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yfkdmgvr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2bpfmyptq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jxmcmkmf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2uvtmcdkn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zjxxfabw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2mydswsbt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2pjkrkavu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tuqtyksm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xqprofcx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2sxoldqcc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ernocdvm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vitxgipc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2umtxeuru.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xyhqpfqw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2guyltlat.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gqcnyohf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2xafxsrld.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2xjqwhate.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dotdvevy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2vnfsplez.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2oebjyuef.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2azvnoqhx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbzihdwb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gftjyaqn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nvhyjybc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2eluawyhm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2noeulqbo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ncxasivx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wraszedm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2juddqwhl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ifuxmosx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qolxcswl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jtxyjfqq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2llrqdftl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mmchkhre.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2hkdzrvtn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2saxbegor.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2qvqddnen.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hhtgvgli.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hmttkdnh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2yyoroomb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xwsjhsqh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dfhgbkif.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lnndjryb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2jcwaevow.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2eudxjdto.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tmlibkzi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nnqewwhn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zfnrlzpf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wclawjic.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lqrmcxzn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2fvvijzvt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fmunzksv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2mzjkomjz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ejsezcjl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2urieogxy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2rtxhdzbg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dvgdzmdi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pueosxhb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2clkdbasu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2hmnnphnz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xgcdzies.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2tsvbohtw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2kblchlfc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2psracgsz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jqbipswi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2lptmtfpy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oihwcumx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2emitjmvn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uakubrrw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2eddbzyvp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2fvsbatoe.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nlpxsuyf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2vkqfhkin.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2piiafltw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2uexulxuh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hrwjhciu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2dtgxscmp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2essssmls.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2jmmvcecz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dwwymhlf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vircdgju.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ewxbyeyr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kkappefm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2boqrueru.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qoohhwjz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vzyctjot.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2aiomsqza.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ydreigxo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2grlgelvj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2skdjonou.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zbwrybcu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kqvhvazd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2xjolhmur.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fxlviyiz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xchlnmfd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2srjnjoyy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2aicgonkc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xetxtzjb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2txzitrxm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2tclarqbu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ifjszzdy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2otjdyqgt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pgbfmtcl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2hlciocuo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2lwvmdmyh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2iincbfls.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2xbxcbojn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wivtdwtx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2frtgjmcd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2angnripe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2cwsmgdnw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ehhmvnyc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ndxjffdt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2irctxynn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fjajxzxz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yeejaskj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mzspqsmg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2acppyxem.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2poycppkw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xfxdxlov.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zuolrraa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2iqqhxibd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cpzrjynt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zsxkloji.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fxzzlwaz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vbqiyjjf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2tegrradg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2urerpcxo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2escjhlfz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2erkksiki.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2uziiczlw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2cqvbfztn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2czcrufeh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qqvqiulq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2owrhfixp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2grkinkyv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dyxgecty.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hbgkcvbi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2aqdhkbzv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ukywqjaf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2csgtfswv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2caedeudm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sysswahq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lkzppvth.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2suykinqr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2awfzlind.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2grjsakyx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2cgezmvqd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wobaethp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2kxpzsdbs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2phnlsuzd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2eidhcdwc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2poququtm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2jrzhbpyf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nxvorwdr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vatzhdwz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2itgrtvgp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eopemgif.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xqqgjksd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2aarepepc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2utvzonxh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wulsuqtt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhjzmjcr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rbksjtah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zibntmke.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xccraaly.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qfgvfzuw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2lnlrxliv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ocosptdk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2kkxogups.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2utcjgydt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vutnblhj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2iimofxra.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2wrlkftfy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2enzstiff.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2rllplejf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2bkfpjgiw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpkqnffp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvfevrro.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fymvgpkr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yjaomeqm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jqglctrw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bcgrglfj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ejskxxzn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2dydsjwcz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sotlzydp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lqtrkdys.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mkriswqu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lnfiucsd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vrvytwqm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zswrnmsi.html

esac
来源：http://www.52xcode.cn/Article/details/gt2hrwvdncn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2afgbnjfe.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2xbgkgozh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2apsxyhcs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kwmftoti.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ekwzweha.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xbjjlblv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dlmwowfm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2gzcllihh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ouxhjvhr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vryilkoz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2htcjywic.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eaxclsmn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pkkwiges.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2pwxwuspk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2atvvfixv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eqfrrslz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2rqxhwfii.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cdsopqpy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iazhirys.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2puxxbfst.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2urjsgoab.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vzljonqg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vcahnvjx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2answrcjn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2boaouyca.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2plciovtj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2vxrbhwuo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zkdfcluz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2aqisoaqk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2qmtgofqr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fiergcer.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rvavpcyf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lbvmxjtu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vaeljwnd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qpccarxg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jdypmvjs.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2qaxmbvcw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2fzbuouij.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zkakltgp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcakrwib.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rutyalkn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wltnzarg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wqjlitli.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2kppolflw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2qbcusicd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dqjwzkmh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zwxjomjy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fqtbyodu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2wrpwfvfv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2zcipwbdi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2nialbsxt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ilpbouyg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2poltjjwj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ayvyxopx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2owuqnkjg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ssvgwhwg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ejddbmpk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2spcfhyqa.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ertrouxb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2sdcjekmn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ycxoltzd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2flqnbgdm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xdcvpoqs.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2flyawono.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2sgewezbf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hemqisqb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2uzicufii.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2dikkdiuq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2jaxdarky.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fyfosifw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2nevunros.html


<!-- 参考信息 -->