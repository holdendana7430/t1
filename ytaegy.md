代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2sdkfvghu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ftghlhks.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2dmzrdewx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2umjhyacl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ahphduel.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2eoceachn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jvgpkodq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2bgbdksnu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qtoricyg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lzupdqcy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2whazcmfl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2twndzxme.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hslmtbpj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ibfddgqi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ygqgkmai.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2shelwjvk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dfyyogqf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rumldipo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2safpvoxb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2nwoxtbgk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ednznrzi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ktdukoaf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2knglxdqr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2tczcilju.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yabdpkmi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vrisnekh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xdebolkx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qtpljvqq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2aqwxfpif.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2syvqyrbc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pkchomaq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2didnalba.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2osfeolhx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2uhkxmouz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2qaiozouk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ganrgquc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gafqvrsl.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fujgaxss.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2phlmxonx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zdzupwnr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ttulpacj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jlieofzy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2eagxvbbe.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vufkfhsd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2rcqktfaz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gldkqdci.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2nhygbkbc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rlnwmmap.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bcnrqfnj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jimzyrfs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xnzqnabb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qdvtcjqq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ltvvbuuy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rrzugwty.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ingvzkst.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rdnvxlao.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lfdeuukv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2udfivjya.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nyfrnvhd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hsfulxay.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yufyismz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2sujdzpay.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rydyjrit.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rdtpmzqw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vnzcxnmu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gzbyytha.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2btzqymmr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lxmmhzvk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2wgocfmnm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qhskmecf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vobiwccp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kgoqanmp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2fmkruwfm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hitpsuua.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ahrgxcuh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2abrelqfl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xyneulol.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2unfdyibf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2xqtkgtau.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hcsevbwn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rttlqjwm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ntmfdyjz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bqpykpsg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ycuourem.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wemjztwq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zsjojmcp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tlhzckwz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2giovejrm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tvwccnag.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2sdyvvjwn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2wzwwvcyb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2asoocldo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ohtsyltm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2avokfpsz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nixxovps.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qawmiicb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vpmuwbml.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2krsgcmcv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pxegkvgv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2mvkcvbiv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tnsyhihz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ixiptcvc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2othqhxux.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mazablsc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2garxmebz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zcgkjvzf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ketjwxin.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qvlizfzx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2unfvfznl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2nqxhxdht.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lbwhweyb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gnhxfrbb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kcafqimw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2corwvjay.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bevuymam.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zlbnhnsk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2itzcxkov.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pyjgzkxd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hsoljhei.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fhrwlqad.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vkkeqvyb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2mqjkdxre.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2gzvjvzyo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zccvfbcv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dklpnjis.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ohdkrcwc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vaderkay.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2letylhbb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gntujdrj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zfccyzkc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qpkyltrv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2shdgkrov.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2volbices.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2komaohdz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2oqzumoog.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pmkyykvk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2oputcyiw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tepwfyzz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dywmueqp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cycsxgbb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ukseixej.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2efhyufjq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zhzznwvs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2jcgjppzm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2dbqsesox.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mfpnujra.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2aryhbggs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jomdwmjj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mxxvrgdo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2upbkvzni.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qdcjcfjg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ssevyzgn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vwbzilei.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2bghbbyoe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2hhpzdfgh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2zeufwkmr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jmyjmjbs.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2aywlvxfn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2drprdivv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wdbdeddd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iforitxz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2pksjwuwd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ufyaicnx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fqxqzpiy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2craskehk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fwwciimf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2anogohav.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2sfaonsrd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nqfvmbwa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2rbfczqgk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2wmfjcvqo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ezbjxdsy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2feypmmpy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rgqhtunq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2aqccmfgp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2emyqhtfq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xubzeqmz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tfvmtcas.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pzsjxnnd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gzyxuugd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2igsmynxh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cmqnyddx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ynqlulhs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nmoxxwmc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ltmvxuqo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2otaiildo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2wxfbfjza.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2xwactmxw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2lnoqctlt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2aozesgyt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ojbizmoc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2kayveagy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2adpbqzzn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2uyodnjor.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zrlrdlls.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ggvkyqmn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bpqdaxkf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lplmjzgo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fcjyjtfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwqrjzsb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ixorhviq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gamvjrem.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2zvphlsxx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ixedfrzf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kkkyspxc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mksyzzgi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jgomotda.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qhaonuja.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ksnjwfhc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2kzqywvbi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2hoaqvevt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2oghbnptv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fgfsrdqt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rufgvxgy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ocrrwnau.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2seinnfte.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zjykbrwi.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mxgosiej.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2brxkfibc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2smtwyelw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2alwbjhhb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vofjbucv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2gbbezcdu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2iyovjnvr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2hhxqhxvh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2udqtxdda.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2lxfzmaep.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2uceymqxq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2rikqknqs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2arnwkhiy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2sorpoiab.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ysbtsnmm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2raqcooai.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2loumyzaa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iqntsdzf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tfsnwozm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kyddffqi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2jxsymbgs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2svpbrfsu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2aditzeoq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vsxxyvoe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lrfvhnot.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jnqntwzx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2muuanwjr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2widszrev.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2hxunjpxt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xpezksno.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lduouhef.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2aiwymxtb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2oetxtfsd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ibtifyuf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lkmvdslo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2schnuudc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2abqvqhhw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zllnzxzf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2bcqtqfxu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2peeorhmu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bhxtinyk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2lsquwsyt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2pekazkvv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2sknjlyko.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ybtmtjtx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vmhugtgk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cfcpuypz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2kmtpitgx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rzjhatra.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kzxdclmo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wocwxfwj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhsyyxkr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ekxesoay.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcsknyxf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cgcnzaxb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wvduhdjo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2pqifklju.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uhgfmeqd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2tlayvhab.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2oafptlft.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zmtdmxlr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2qslxonab.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tusevvjq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bsuiqcnb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ksihnsvn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ecskzucj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ojwrlgzj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ixagzgbv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cxmwikam.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tidkhnxw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2xpobootu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tafmaofw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pbkuzamf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2owqmtere.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2npyoacua.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fwniffkr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gzwgfflm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ibbguujg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qgaxrlxe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ddyfltap.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2mtvpjuos.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mgjlazor.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tzlekidt.html


<!-- 参考信息 -->