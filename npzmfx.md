代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3upxngzbd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bjaquvnt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ycucdzmu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3wowriava.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mpgpkfja.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3icvzfrmf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3toqwxoui.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqueoaor.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3stwdftkl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mchkuqml.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3pfjptdqn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3izhuvsna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmmjsqjq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3yrnofsqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggwosxag.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ffwjbszk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jgmseblj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cwkkhhuw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dqpxesku.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3mbbzgcxp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3smeobrpz.html

);
来源：http://www.52xcode.cn/Article/details/gt3ouhzxets.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hhrrwuwm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3aeptelgh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yzdpxdpc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pnzlpowb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3mqcndshk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qvqcmcye.html

);
来源：http://www.52xcode.cn/Article/details/gt3ozlmzgre.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3dxpreerg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dwkkqqpq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ybvvvhfl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pcsokzcr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3eznxggkk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3iazffvvs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jbaezlft.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3dtdxytje.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3cptfbvsg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3jfpfzyms.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3odmyrccv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3phweofxn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3rsnrkvei.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nlebblxd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3thmrpeqn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3owlvzrza.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3yyuwcqvo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kkensmhm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3omnpflyk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zjqjnzqr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3zxtutlgw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dbswoius.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3igngmkyn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3kajowbiq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3egvpsdms.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ljloqeez.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wchzqqfn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nbutjckz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3mbxkmrtf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3msbuaami.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3yvxchyhr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3bengewoy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lzhzxhjv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3bmifgjbb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3phowimqo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3mgqxnpop.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jqmlmbyf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aotapsxh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3tlyaiejx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3akauvjed.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gzzuuvze.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3kfzvtsco.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ynlubnaw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uvmkfhex.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zbpugvkc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmuxliwj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zpwkeukg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3bxnkapqc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3zgexhryd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yfrzvqvx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ugnldiig.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ljdlpmlv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jcqjzyle.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nswtwoun.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fqkquxte.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ehfvcbts.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ckacnzkj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3edsimost.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ztcjshnd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xkejkbur.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jnhugpss.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3akvjlhwk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zpvxuire.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qbblcrzx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3fyrwlwyo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mplfbrnf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jpgrlevn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3zsmlorxm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3oqnatxnr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hbjmwcwk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3phnqynak.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3trjzzkgk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yruuivlw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zcttaemf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3svdilsfj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rsatymxp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zzqglumv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3sosomnmk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3zjmcyprz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ytsnhfgo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3bxpnfjlg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xurfobcg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3svoxnsbg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3khztwokx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3twauaame.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3iqdvpbif.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lvrbfthn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zbbyaach.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wfduebhd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3iesdybap.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3dzwmxhrt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3idytjcgx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fmyhhyxo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3dqgubeln.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xmaritnf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3nfoopdbs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ttkraykx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qzbawqrb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cqtqjxne.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wggybslq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3uqhudpdz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3japhaczy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3xpplenkb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ukwyxcsi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ymhntxia.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3saqxvtol.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3skbqfkbs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pfdrrkob.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3uzmtvrcm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dytmraui.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3djizdbju.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xjprlwhu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3seevyklg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3tfldljvc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kccyctsd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qcugiivh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3lwmbcbjj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3clcivanl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jgbqjgby.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stxtjyvp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3twzhwzyz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jrwaifqq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qurdjvdg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tfprxmma.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jxwtyxyx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3oyqhjtbm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bufwejzi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3hydkgmtu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iowlxiuv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3luszmgyc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3svxwscts.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3enljiysk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3xlkycjvs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3pmpehmzo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jkpdbrqc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3mwfajnoi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3avudpvkx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3tdnbxvou.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3zavfylma.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3juatmzyc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3kygdejdm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3mmgybiuh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3qsdtjixm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3uaawkhss.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ctckfgux.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3qiydwuyq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3frhmrcjb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3qqhjtgmu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3mttfovzv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qeyswvtc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3mdmdnqoj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pnrpzyck.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3aiapzrux.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kkzuftiy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xioxjnsk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3yzwiffjl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ekwohezc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3palzyegv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ltvlxnux.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3cvurhvco.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3wldvkqza.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3gyfrzchw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3fweduibz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ulmgltdp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3cgejmtht.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bplldgns.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kdawfvcx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3oqcmpvwt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tykrdpmn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yxbjrmdz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lgbvsbbx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ebirxmmk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kvqwkfvp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zppasdhw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jdwxnwgi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ssujvxop.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bivpidfa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zeoemybc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ujjoifdk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3pnzygggs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ujpczihz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3fqyidbyh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ziwkjmvx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3weevepll.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3otrqynwt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rtzjmikq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3cdntnvug.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lhseqpfu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3cfzivlpy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3zstubutw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfaetvwz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xhaeauaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfudgxkk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3oiwtqmof.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3wfuabvlv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vzxqdsoh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3axdqvbxu.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3imidzdkg.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3usjnwgqm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qdaojynt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ehfmjltc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3yjomvfcl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xrmixgvu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3nhmryrvc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3wtxvldzy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jpqedhms.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixlzhahb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3lkrnyjpu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nmhyjkkm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3vemxazsd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kacvehlb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tnrhxyiy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cemxqpca.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3crkvoxyg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hlhwsgsp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vgwqrlns.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xwgutllu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zlqiwpss.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gibwondr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jzdgeolx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bnvdmaqe.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lnkuxzkz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jgushtnm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tdntcnsx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3nrsjnjxw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vnbagwpx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tuwqguva.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkkvrtga.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hmmbxohd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tqewmjdk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jwrmnjga.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3quvadueb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3evhpesfl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3liirihni.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hiwnudhk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3lqfpqqlh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qywntbbh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pbspmial.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lkumvwvp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3neykpxqu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3avueorpz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3apokvoyo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3etpxxlke.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3chvnkhri.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bpvhxzpt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwhuwrcf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jsubzuxc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mhkjqfmp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3tmofogkh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3gbdkjrkc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lsfksidg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3sputkvjj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qqpwuwpq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dvdygzuo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hdiyimgk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wtscdzon.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rpnhebve.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kafvopcf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3pbrvndei.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ueqnqafl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ldhlvpyi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiykajpb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3lyvnmkmi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3lyntxizz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3elappcng.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xglavnnm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hwreqpwx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nabnysee.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hmrbpggv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3eyhlktlu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pprdffao.html


<!-- 参考信息 -->