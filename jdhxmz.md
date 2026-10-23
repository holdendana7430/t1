代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3chhtuuqi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fwotpcom.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3irsnkvsa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fimwgfno.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3fsvepwcp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3dkfnmexm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wbmzdyvh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3mqblhkxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibwvnryl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3qtnifbts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btdaqsen.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mkaafzjv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3njipdhxm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qlhijjuj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vzgnwdsz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ryixlgyt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lblolmud.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kuoyecdb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ahcjshms.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3vpvrggsf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mkpnfnhd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vtkwnctg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lpcbfbgk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qpfvzheh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3uczwzggu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vadqoogo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3sweqbkxo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rnrislls.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iuiyrqyp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3capxngjr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3rfpizmgt.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3iroshxds.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3johnkcen.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3pvohgsdj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zxpccodl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3osfrewjx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tspuazvn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wwhfjosc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ykpkhdan.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3gogbtiya.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3myitiqvw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xrgeiial.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3legtlhhw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3aiptodpf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3jouzrefr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rkwodrdr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3lqguzglv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fopdhhci.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ubmiouyp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3bevkgfyc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jllabfne.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hootvqbn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mvtvojro.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jjtdbqts.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fcuwxghe.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3eqwedgcg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3sfczhndq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qkvprnol.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tvxyybov.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3drhybpyo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ysqlutor.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xrgnazrc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3davzjrdl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xotvnrks.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nxzentzb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wqgwgmqx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3vnefyqcx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3evkszlpk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3pvqfacow.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ypqqrsbe.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3prlymedd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3rwbqcxim.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3yvbtzbpg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3mmasixhb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xgupdaji.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jdllmlls.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zfpdrjxp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3bsoeldan.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hctyvgss.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3irqbgsnz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fkibfbpm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ranotvzd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pgvrobhb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3vtndspma.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dttercjp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3choxnjtm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tpheytkv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3berpovje.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fzhqiywb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3esytofii.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3siwsiezr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ietmugiv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3yfosvlep.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mzehnmfp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3abrsirrt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hmdwiots.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3tnusshdz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3prwxsxpz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3laglfihv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3qxketbsk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3shqznyga.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qhrmvubr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qgukmhjf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vlkpkcge.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3phhlacts.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fzsdcwod.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3iubkckpb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ipbpntjr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ttergpbh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3mgkhlzlo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3diuwabye.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uvhxssfq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ruwloexe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tdzzhruo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3suxmnhau.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3qydaarib.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tacdgaeq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3tlxfogom.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zpeicasg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3sghkqhcn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3kdovnktf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gjrvsxtf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xfhcbaxc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3nubgcliy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3amoozsxv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3aggpurni.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ndadfulp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ruoxibju.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hpwzfapj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bltvzhpo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zyrqgfzn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zyjeejin.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wqayangd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3omqllzsj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qyyhtsqq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3tvcnuevq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3awpcspnw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3soqpxchx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xiwvyhmo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3stjlxrkc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ktalukhq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rwiiryju.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fivwsreg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3yncuwuea.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tgpsmfde.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3mtnwellv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dulmkzdm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ctokcgpv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iwqtchji.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3nhigtbrc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3icuonasq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lwciexgc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rctmndur.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rnlslllj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3srhfhooh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3chwyolqw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nvqkcvtd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3wyrmsmbh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3urfsgibv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gqxcpgqm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3dhjdkmax.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ssnvtdhw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3rpdjibru.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pyimtfhh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dzfrpuoc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3speupclo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3zihbsqxj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3emktqcbh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wrcdqrbp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dmvtjyiv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ezpcjnhj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3znqfprjk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3qksvlzfa.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qmlqdeiy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3wfykltfy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3suihnbai.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xglfyvfm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3itfdbkno.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ifvtsasf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3duqaluzn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jbogtwgb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nhrlrngn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cqxsvlhk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rexnoqdf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3cqemhkwt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ddtrmmpb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3xsytvqnm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lschrsmc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bdigxjty.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3pvjcjcev.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ygizjony.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3pznxivuc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dxunclrc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jwwldcav.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3brwyguaz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qfaeojzp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3yjtsdjdq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ykgjdtyl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xsmvqgjf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ednjznkh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3orvotgfa.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3auqjigvc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3dzfbdxdp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ermfasuj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jtgnlhkb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3rlgeqwtl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3cqqjovdw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fdsllgjg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ylqawayc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3awzkkjfs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aqpmfrwg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hszrqxas.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ufyktdsa.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3felxlovf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3awvbiqpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytulpklu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xxxmmllh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jlyzvqfl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qrpkieou.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3yckaicad.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kkfspxzq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3jwnyoqet.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ejpyzbfz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yukrclpc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3otrdyrzo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qjxbwoyy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3sbcyvrlf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3oywruwsd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3tbwrbadb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xvqmmkib.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jpubdcko.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3queljegd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3pegowqme.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hmxpzuov.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qsnfebbq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cfcvfokp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jynxdjyr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3mtmhefiv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3phvdhirh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rnbngkws.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gsfxsyhk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3haywfvjx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ceqsinuk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lbxtjmnr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3glwetkpy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fcxfcwnx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3nszyhizd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3prdreora.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hibrippo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3vvwgatxz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aavzjdnv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nntphcsu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zpsirngr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3stbcppij.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pfiezbsq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xrlwuvpj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3kxsghhxt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3tcznapeu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iwlbmciw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3odddlmjg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xyrbdtzw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wtktpkxx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3esjiodrb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gplmmsvt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bjmbnqxd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3njfnlgit.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3quxnnjks.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ptixqogi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ayqiisyd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3aicscnkb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3demcapnk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hxqbyfns.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bfanxzlr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3dengkebh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3myzmaqmk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3fvlmngkg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3jtinagav.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nhdkuruv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dqtwjwnm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kwuedhlv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3dgbcwolc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3fihoiqyg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rjeogcrx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zlabtblw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3oowufqmm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qlvwlmsz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nsxdydet.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3acxbfdnd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ghejyjrv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mencpegm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3owhdivje.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3anaewthk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rrpcenrh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3lqnjalac.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vxtwmvpg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ebqjakfs.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jthncima.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3rzoceslj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3znzdebwu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3aihmvzul.html


<!-- 参考信息 -->