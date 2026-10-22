代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rlznotjk.html

);
来源：http://www.52xcode.cn/Article/details/gt2opbtlcma.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2tucuhtpk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2wmjmfweb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ppxbcyit.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2acgthces.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2gihashqr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2kujenjnz.html

);
来源：http://www.52xcode.cn/Article/details/gt2leqqwtmw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qnhyinii.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bhsdefdi.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ehdykfeo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uieqocdc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2delwwpip.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ovcpzeuv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2xnsnofxc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ahuglylb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2temvssbn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lrodehap.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2nrxrmwpj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vtdpftwa.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2hhsnfioh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kmfgfjqy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qfwdkbfa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hkgtsgia.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2fdsupxji.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2godptpeg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2dfxtyohq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2fzhzxzou.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qudcgbhr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zmrxvyha.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uhoqbmio.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2sfurvvhn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2cgtxdddm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2tjkavlsg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2rwzshbzx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fvyzecsx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2joufawbe.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ukqyuaqn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2svslrdya.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2exzygjjq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ukgzmmcq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2cbytdkuk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2yiifhaam.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2eojtbuwh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ymjfokvj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2flfxnszn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2zpxfnanc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hiywtmtf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ylddlprk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zwaywezr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2npalygnh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2cmbwxmbm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lnlssgxw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iblcxmma.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2xdauswxk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wydmadny.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2cugaplvz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lggxgspm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2jsccvykf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2llrlqefd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gwihpnug.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wbnilcoo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pkpryyqr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rifxujgt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ygyxhdsc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2smqaprvk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2sakclhou.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ufufwwsv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fszythsm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pwbxpjui.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2zfifvkqo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2chlponfa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dtjrqydi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2fdmyawfo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jdoteliv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2agcuqxwl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ttzhqewo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dpryally.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vnxvcjvo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zadiaxtn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kdvqhmoz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qprsubjr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ohdawdsl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2doafrlwq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ubxqnhgi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2nuisqkxp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jgovljhs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jcwqqyyo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2sbjkovfy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2nwbubcbi.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2evvvnxnd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yiouffbz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2rrgpzjvr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2lzuqrgps.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cmwmlznp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2mjaswovm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zcquksju.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2govxwfmc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ryulxvco.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2mrgmmffv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ejhlogqx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2bebruueg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cieifasj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jaoiocvi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jftckhyv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jfwdytfo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2atkfjeaq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2malmlnsf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2qjutuzfr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2kswrgdey.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jtupepav.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vjfitrdt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2icokyrmm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wvghsaiq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qujxykiz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qnytjatx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qqoagqhl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2musnyflb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2oxaxxmqr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nndoxlcr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qzqzxvvt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2dhsbwmbo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fnthhrqt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2babcfqtr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cijsbntc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mgubvcvk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2imvxylmg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xdkimfhp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2gjzuzapq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ogimamgi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2syalstzm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gaudfvgx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ebllejwj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qshlxclc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2orxucpsd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2brpkmxtz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rytutjgw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2yzlmlhtn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2upcuqlgi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2acuixbqm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2spooidya.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2buumemnq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2otocgqtd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uzdflkun.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2udonyhco.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ycfxyzlb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mifruxua.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2igkmrurj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hvbqkgep.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2bwcstlir.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fnkwnzse.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2kcwrlzmz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2rogeecii.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2kasrmxws.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2votjqeby.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2pvvohwgy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zqsidgsq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2pnaktwar.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2trfwtzky.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ngifccwp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tpkxpmwi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2fluqjzxu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ssizjrfc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nkbbgqjl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mhasjyhb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sghdfapr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2dwxvvqfd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fededmkp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2srmekogc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2dckxpesl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2hpqgqcia.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yqkpzvjr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2mynwfota.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2barroews.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ylytjdnn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2kygyccfx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pdjlngqg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pwnruhew.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xwbuibgk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2azetrerj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2valgjzmf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zfedacvk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pplketsf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2getujxnb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ybfjlntn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ltgugqhr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2sanholbt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wcynfnoe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2unhqhbvi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bqfqowtq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2cbloqagd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rkiembpt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ipnrzucz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gcooikub.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uetmlrgy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vtqcannc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qhahnyxr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2yeieiglt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmyowdxv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ieqqzwpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psjaznfi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2cblffsah.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2etbzzpzs.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2btttsmmj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qcykmptp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2tzjxmrgi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2tylfkcne.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2mtawrmlq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2sflcrsis.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2hyweolto.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nhkxewle.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2agvnxmjv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2odfvmlce.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfvguwah.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kizbtutv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vcvithti.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cwnwkkju.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nawagiww.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gtmmoicb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ormogxnv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rqjrkunq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pivfsfnp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2svkatdsb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2igerlqza.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dthbcyyr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rhsqkuej.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rddxtowv.html

esac
来源：http://www.52xcode.cn/Article/details/gt2pziqfxbk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2rnxzcbsw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wykhsexf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2staugbdh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jnwkpqlg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2krzxnfiw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qomazayw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vfaytdof.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tbhnlhmt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2pgkrnzmw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uitvzbjw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2keavrirs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mfpwdeiw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pvppdkan.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nnvzlnap.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hugrlqmr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xgfomkhe.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kzobrdrt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2krxoijxq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lwpaqylz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kwfeusjb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gzfbppis.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pbtarsvn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dyfnfqfy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2udfghjqi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nxzepbvh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2hjesvijk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2lwpozxbz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zdbohbow.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2cxsqdfwt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ggrinxrc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2oyzabvrb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2whdrebdz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qjiuaidu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hfkwgreu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ddbpjqzb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vdmgfpci.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uspdsqlq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xybuqseb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rofsdfft.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2uimpdwjy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2cqafcjtu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewbbrdau.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fjsbbhsf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jbawnqej.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2whjlwsns.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hmzqdnrz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2yppqdzoh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rclozjmq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2bamcjjir.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dbyzlhzl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zkxnieak.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsteirod.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xcejslpr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2mlmfyndn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pgzjejwy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xvziugnz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2oojiyami.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2upfdakjn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2uamdghai.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zvqbfyhx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kmxevxyz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tskmcspx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bckgkhzz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zcnspxkx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2qhqorvjz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2amaaatmp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rbhguchs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2yxcylvif.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lvqlhwbb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2wynojidx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2trxyntjf.html


<!-- 参考信息 -->