代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2magrovio.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qcjweajl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hwfgiqmh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gvbgfqhc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hwahryjz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2isgqjbur.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xihwokrl.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ftnsygwp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2typtmgci.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lxzqwhnj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2qhuxowrc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cqrclaqm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2iolxybyk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2azrabgjp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uwdbgnbq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2dfmqdonr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hnefekfi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gwajfqtj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2hyjfffuc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2pubmdzmf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2rigbcloy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2sohtuzbl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ojfxiwna.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2rzilygkd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2apifmwpj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2bmjuazkd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2urpjtntc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2stegksvh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zatkeiua.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wktvokhi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qcxzbsop.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2rlbbermn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2zfkwpqsw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wezrwmoo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ecjncgva.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rwvlwrqt.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2yjouhjhh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ijntafbq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dagzlynu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2kmvzchfm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lklvyaog.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zbfwiiws.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hpydbjuv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2vcnbszhe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ongdzcsn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tkjaysld.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ndfhainc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2utzgjheo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2aqnchujf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2miyqvpdz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2spglvgut.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2anfifooa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2vwwyhbgt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2duwpjvrj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2plwhiebv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ysxmdzkj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2viutrolt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2bodznmkd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rqsclzyh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rjixuqzv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mffipajk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xoedauzm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hqtzvodv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2jupmlaco.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ruyrzcwz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2oclzsutp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ocstvtcb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2stwismav.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fzzdunfq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2fxcndnbn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ncpksnui.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rsyxzhjk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rsxhszpx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nxdlsiqh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2smwbdqqd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2jtukfcwf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2vkjnjyap.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2iurhfvag.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jzfjhbbn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2bdzczybz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bidswmpa.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aejwbltc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2brcojivr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mxqxdlkv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wulzqjww.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2czksefwc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2uytauslk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dygdunqp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2dseefccn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2autschzz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nwvpquta.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kxidtnst.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rleyafhz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2kohpkizx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ndnmjtmk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2tmgmiuxj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2tjjsdxkf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2oexnsyyu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2uwhkmxso.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2dysbqmcr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2mihdsjcr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jxybrovi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2dxcrsqnl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2htbzdrnr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kxvblovy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2gtvokikh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jbneswgo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2eatcpwnb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zkgmzagi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mcrjgnel.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ozdqysdq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zkwocnez.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2pfusqvaz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2auqgbwhn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bhdckvem.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ppdhyune.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pnnzbyfm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2jpnjijze.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2obmwiupj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bzokkhun.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jpdmlnfw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2hdlsehqg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2flrhnaxl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hmtydafx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2tsugawdu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ofojadzl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cknofzbj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dxcvskku.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fxdttbno.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gtwoibyg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qryjlyxu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2jtugeekr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2derhidds.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qfjtciiy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2momgiajw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xfgwzoen.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qjjuucni.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ufpxehve.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2yxsixiph.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nnkuwizg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zdpjxnyq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oykegtqn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kgyyutzg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bgqkbkzt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2kryckgtr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rexfzdmi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nukmeltb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2cjfmeoiw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2yawvrrrf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ifdbezfv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2pksigtou.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gjeszxbp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2lhahlstd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ggldbwwo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fkykelmr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2detctndh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2becycjfr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2nsmyhvbw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2tyxfvccg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2gvqqvkiw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2fxdbgpne.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2axqxsjad.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2twyasesu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ngquybvv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cizzgfli.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2mqcostap.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2okljkrbn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ufgqadke.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2rwtnvwqr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pkpggehz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wwrnipia.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zgjqbkjo.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2jguozbfi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2imfsywlw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2vykkeqks.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xvxsxmao.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ddvmogma.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2kwysxsxs.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ygvereny.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kusfwons.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2iiooyefj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kecmojsp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yyymiecq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zllbdclu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2szzyyzqw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ybyzrfeu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2amcxyuik.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qgfxforv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2qsekhuwm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cokjvpwe.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mltjjohr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dwwbjbgn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2piqskbwi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2qbxndxij.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2adlqkbee.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2yhamcect.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xruyjrqb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2znqswhyq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wwkaadst.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2viceeljh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jmtcoytc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2tnyrrgwc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xbnyutmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jypmvrsf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2wsvyepcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikjuvdbv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ychurlat.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mssaucxf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2jgouwana.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2iwgdmpfx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2aclkinpj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vitzvfkl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2pwkfrkmj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qpftzebh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2izdqlmxs.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2azjjywuh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ncwhsdoe.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gqxysgxh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ibggkenk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbxomggb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2icfzvqac.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2whlcvhim.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2pasipgsy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ghhdrbbi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kdwtlvbq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mydcjuwk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cefmelkt.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hewvutue.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2tdztlleq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hxaekenx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zgtmpjev.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zgasluik.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2zjngmwww.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2fqgijxir.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2uqsezsir.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2trpxgomx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eegszpox.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tjhurofd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wntnxirg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tjqsqjnz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mnukksek.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2liuhqofa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2otvhfdjt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2gwxjwvst.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2gbcpnqdr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ptavzsep.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gljfhpfz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2adoljvjc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2lelgvnba.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2yetjgkur.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2enpykitl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zqlozyxl.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mqzvqpsb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wmitsoml.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pjepckkl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ifuikkfw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vkjidzhd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2opkixzfe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xrcedbzv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2djbhotvo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2bgrhezrp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qgjthfpt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2htjvwejv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2bmfqltpi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dbbsmwjo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cbvkuvbb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qsvqenxc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cqrdzbuy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jtavuome.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bmmsuwxp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qlznjuhn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ciqwrkbc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ibksnunz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2hbcheryv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jntwgmne.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2tmmicppg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fpkyhytw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dhehnlte.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2swpxwevf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xhctoutj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2mcvajzfw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2uovyoibg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2cfjgafbv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2pkgwozac.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntmmhlbh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2zanmcfya.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xqnjaenw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zicgkulh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2krlxnjty.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2msgdtbkn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qoyibazr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2posnixba.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gmdykttn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hrrlulkv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rlxwzhuh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzjvlqgr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2mnsqjgkt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ojhurzxb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vdwjrlrg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lxsbozzk.html


<!-- 参考信息 -->