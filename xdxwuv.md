代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3tfebgmyf.html

);
来源：http://www.52xcode.cn/Article/details/gt3sgpeaduc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wibtzqsr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3jwuhqzpm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3auxjavoy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ktanryzn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3gsvjahej.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3spxxfsnt.html

);
来源：http://www.52xcode.cn/Article/details/gt3jexmxfsc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3cuiubpdo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3dijsqnuq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3migvqbyy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zhfyeqyr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ojsnomyk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3necrapsm.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3yokftmej.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wqxtgtka.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mqtxvldd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wsagawmt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3wqmtkibx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dfpeeplr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3jdmmqyts.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wclbvhmx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ttrwbxql.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xfipsvtm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3qxkyuino.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xebzcyzv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dyebxvwq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3yirivldr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fuaqjsei.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kuadsimg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sqtnmkge.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3mobztjkw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3nftbdqxx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ksgkymtz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jrjmcuwf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hfubbpey.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zaxincnq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ymxecdzg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3zvqyfmfg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ktlixkqd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kearoury.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3mdkmdfop.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3yyccslxt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ogvidkkx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3cdjtqeab.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ypbpaejc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gjtsneaf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yfzlqqbh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hsljnjnv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ozzmiayy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hcmuzcdz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jsojfpae.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3dbmfnxdk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ljancrpd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3jjommmjk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3rawlmiis.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3dquoavvu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xszjcljr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3nrukdere.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vjimhgwg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3nrjkcifg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tzxcshxd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wzgcelig.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pdqhzcgm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3nesxvxhr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qpnjojpp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dvyhhsji.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qgsrlexu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oeipeygu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bxwuetni.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3sxteqhed.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jumvbccn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3loqqbnku.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xjcwajny.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vaxfmzzs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3autubyah.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rfzkxzpm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3abdaupaa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3avfxgsnr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ppyzjrdu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jcqkvdhd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jghsixom.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tpmiutzq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3wzhnuthw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wqhqqlrp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3sadezjlm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ssulsotl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3lexexisw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3sosnxfzp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3uhaawhcf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3nfeaxbcv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xbpetofi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3nyjyfxxc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vmrjxthu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3npaqwbbd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mgbyttrc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3harrsxih.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3lfgrhrbw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ybipcwyi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3otqtctoh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zjsvdmit.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3argdjpng.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3obfhikdy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3pbqclzhd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uaxqiiru.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3gxxpgvzs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3otdxzuty.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3tmvpxgvu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mictcobs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3qkxjkgsi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hasjupqc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xbkbocgw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3chwpyflm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qbriqdcr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3dbpdtwju.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3urygpwzx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3mmqrofqp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jwfmlikk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3gnmbghlt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xgksdxcj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3qwkjpbwv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cblzwskq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3qvrnuyyb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3guwrrcbr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nokhpfxk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gosmefcd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hroahdul.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jxqgqzjq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3kqswszds.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3afwybhfn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3nlqmvtja.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nnlsmvls.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xebhnwbr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3bemmihlc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3agbjmntf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3icrcapmk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wzqgkmqe.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vfmbbozg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gipnsvgq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zxiurvef.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yqamqffn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ohuigtbq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3kymxdoja.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hkzgirqv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3pdyjjvwn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ukdvxiys.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3tyuckkyk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3cgdfanbz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3emjjnelt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cfvheizl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3szcuyxqd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3cvabzwtj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3lwqgxghe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3kofvdkgw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3osbdsepz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwsddkbl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ofujjkpf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3daohqjbw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xpbqmhia.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qmpsnmju.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cjqiztoo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vwljybsh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3pxmnuump.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bqfqlafn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hoxjorrg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jegpjggt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3kukscpry.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3qnnivqsv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3btugxiqz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3wfnauhpl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zgczuxvv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gpmbnsyc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3xuvwjmoq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lboghlnu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lufujbph.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rogbndwt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zvxjdwwm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vcecshrl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3engntbqv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3lmcuyzkw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3msukdpaw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wbokbxwj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3czrpyxwk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3nzgcdpaq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mijkduns.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3xhmeheum.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3nisijbhp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hiqaqebu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vgqivhgr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ggodnoet.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fpjtncwt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3pjcydoxu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3onurglwn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3asgvaair.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zejucqvj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sjeiopyn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3vftyqlhz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3zzupufrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nttbxije.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pyhdpztg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvrfxmnx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rkwpzqly.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xyobpiwp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ffcqjibo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ohprnbrz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3nfnvgvkk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3gzzzwzsp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hodrhxmm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wcilxhcd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3knlikuvn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kblphude.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vdohlchh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pybgiktw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwfzwwtu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3jkdrfbuy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fbizmhij.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3bixptfpc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3czksesjp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xuavlnti.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iivcwqqb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xhpptfuo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3nqpcmfir.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3icylutjl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kmdwyohr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ccskpovg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3afmizflb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3zuuuagpt.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3plgajmnc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3djggxjxg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3lrwkspya.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pwzasfnj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dsdluqav.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wwemrfgg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jhbffkuj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wyepsobo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3rlpxglqb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3oertvoan.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vepewwkh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3wxuvavzo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ucyscynh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3sxkblwuk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3bynkxihz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hmmbemue.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uevxpxoi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3fwbingxh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hyjeeqmx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3szgobhty.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3mobcncxw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ecilufwy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ebauiaev.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ynfzzpoj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3snppiswu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mmjobocu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3roafmcyc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hkakqqcm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3uurixepz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3egdvrktw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qhgrazxe.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3axxvlqxw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3scnosdxa.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3akouimhv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3qrxunyxo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lgkjpoan.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wiytckpn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ztgkcmms.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ltybrgql.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wrthykrv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebfazuoq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cexijzqw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qezowmzw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hywhzasv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3bjojllev.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3cajrbgoq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ikqoaimh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3frtuesnt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gjqkmanf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3awneuuwx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3narnfqhp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fpgtsknj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cupsgqic.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zmbqkcyd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3rshrwmxi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qbsbkljb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bbkoqkow.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mqndxepl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3bwxtbrpr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3gzlabemx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bhfqcgpp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3opgeqema.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3tbxxpihq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3uepohtpl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3exjavlzs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3femtouss.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3djgbcpqh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hxvyiylg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dqnthsdr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3oycenidb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ffuygbxp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gxqfimuo.html


<!-- 参考信息 -->