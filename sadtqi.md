代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2fzdgeoto.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nysetkkn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tspsyjkq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gwlxqujs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hthxtvjv.html

);
来源：http://www.52xcode.cn/Article/details/gt2jrpqqcsw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kewhwcmw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xjlfzasm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2atnxrroe.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ffjjyjqk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ijnrjmpy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2nirwfoyb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ifcsnfqm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hcomqnhh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2xiumdiil.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2aiauuzqm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2howmockt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2zobhpmxf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2nxedcbpd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2igrwcepg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ixfepqdh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2dhlfbkgb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2llrsazqk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hpnzinnr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2juljcxjf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2rnuqixru.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2terutvxi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2xcydtqgs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hlagtkuy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qbghyyxi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sqmkdonm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2xwrjuhgo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hgmhoiqm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xvgisbmn.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2stytwunn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hhcwefcn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hijjugqk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2hzhvoeyl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ecbpnzmt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lbhrvuzj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mwkulwdz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vyywxgud.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bsdhtwye.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zialvldz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dyoimxiz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zwjkpacg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2fxpyyxxz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2pfhnouca.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jhgabaty.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uzymfjcz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ajtizbba.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ojclkxmv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sveselkd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wmbnspni.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gyzuaobh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2apyqfmna.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2dgscufcg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qrcsqzln.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2njmpdamw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2iyxmgdqd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2rqtwmedu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xztpqjjd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vbusqyzt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gjiwvidd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbmcfvdj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2yyqewwte.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fzkzomzi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hvsnfjhu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ixgootey.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2uwcnqoxa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2smiojazq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gnrwyuow.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zfvgnopy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yiyuhnqc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cwmmevzf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ryhtqtwj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gkotdvhz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2grhyzfjg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rgyhxkfj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dbibjwlg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2wzxvuvzt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bbzzjfgb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2nzbwluoh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pwthwlzj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2pgejmnfi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vynvunmc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qpzjhoaa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mlcvlhfl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2peezfbrc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uvtgfivd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ioveeulq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hgysqfkn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2beczmjas.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2alsnsose.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2gtxbgduy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bdnykfoo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2pwkroyzu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2kthwbqan.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bgkmzkgr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2gfmpkied.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2vpyxgovg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2inpxfekv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2azislpxp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2wqrgvjgg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2dopmxbqv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ynlocvuh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xiyebgay.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fdxxqqbz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lrwowbkg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bunqrgvf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qybupxag.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2yoqdqmel.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2amylkasl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ucefhptb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pwlitsft.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2lqjujlnn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rxkckild.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ztluuqrd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mmuywolp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ltvcfesu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wgsckgge.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qdcawioe.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2prpxseqb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zgzblhgt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2brqketrv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2oydfznen.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qrzcolyh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2dohioxwc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2raxxzkjl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2iqsskcme.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yvwewtbu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tpuadaej.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wkyxnldx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2kzosivka.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xnolliqa.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dqgiocld.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ilaezftp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qbigltrv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2waoniysh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yuvxjhdd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2omjgkafu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mmfcyzyl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2cwehkzkz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jalujusy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2unnccxmq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2raibrvyh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xyibhuqg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ticjdigw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xafaomrt.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ftikzyxn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2rtetyman.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gopkmrwu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lgzpbafe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2peksziim.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2awtjbdvo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2mnizlnqa.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2laearvcj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2wchuofml.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2gpynzpib.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tcftuumj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2dwvpolyp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2smgubsdt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2eoiykvku.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2zreumgwl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uffcixwb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2mcinknwg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ocqknqwd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2mvmmffht.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qeiqldmn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bmxbmmzm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ldogzkxx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xowcheor.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2taqkukpi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2bippdaao.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mvkltjqv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2cwstzfxf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rsrlnsti.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2xtqsthec.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gftfjypj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ysqfwmox.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qbsoglzf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gmaisztv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kmcztlnb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dgtyupvw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ttaciunq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mmukzoxk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ujtgrprx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xuijrzyw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2sorynqms.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iwzwzwju.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ftsrhyey.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2kwzoheqb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2iejejiid.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2mzztcnbc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2qgpmsiox.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zvuqoxme.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xvmabuga.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wrtnpoff.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ypqmnqyb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ttxtwkaq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zatfbogb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2eoeyszae.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jxnzhrlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txvqfupk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hknyabfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jolzwizc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2btvjdrhr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nqbmrkil.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dfdkucfz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qabhhsmu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2vgkeooyr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2yrsetmff.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2siftjosy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2cjisfxwx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pnklpgwx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2heowmylj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2glgqmcmx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kestgkfl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvdlfomg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kvcipmyg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2axupuefd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pjwsflqk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2dhavnqkg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xjwizqhn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2azhlpwdx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qvdlnitf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2shrwawor.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vopxauwv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pqtffrwr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ywumpujf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2wufgvvfm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2wbkszzug.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zpifghgq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwzkexkk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nfoabizl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ygrklyjz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qpoiebfl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2efukvjmt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kxnecqzn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tmsyoxti.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2khfgtruv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ogcivsmd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dnrecgcg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ekqidwfa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwbscxlu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2wvrjuzvk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xibklbru.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xykpgkoc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nnkqmtpi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jftaytlt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ijiwdhkn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lcjylnip.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2lubimwkf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2shwwyugf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hgzmmuzn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2injdktry.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2frmjyecp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zdxilevh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mymccauv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gvdulnft.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2brfjihhc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tfgchavc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sdyrgbhb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ammpgywu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wtaxryfz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2spwpaovl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2beazxwil.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uusdcgmo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tymtlmrk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uetpkqrr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2sqigeouj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ujudewkt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zgwenejy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ndtbwygb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2soxgwpom.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wmfwbmrl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2evfdoxcv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2fytxkvwk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qgfwfirz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lxabadta.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2srlcrqwu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mmpaqwxk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mgvrruaz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2nprtylfp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wotuyvjw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jjnbothb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2fpkehjhy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bohdmnjr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2utpmgtub.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ndsfilhp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fcslyedf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pizwcysq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xvzzcdep.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2nfjlyllt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2khhwdfsi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qbyvhjif.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2eckngdxx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2eyujvtjy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rcdekvzs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cgnnqjoj.html


<!-- 参考信息 -->