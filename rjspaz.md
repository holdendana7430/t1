代发 wailian999

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ydknnlnh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2yclyprsi.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nszonseo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2naiyabjx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2savlkgfq.html

);
来源：http://www.52xcode.cn/Article/details/gt2xscfypyj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hpkgljhz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2fepieofl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2adnjcqca.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gtgfiyvx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ewsttqvy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2aakjkalc.html

);
来源：http://www.52xcode.cn/Article/details/gt2jsxdeaqr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2oukqzcpg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gppzvxaf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2wwdlddnj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bfpapdfn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2frluwqgk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qrxxnnnr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fluwbqaa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2vithgosp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2cuqycikf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pnqhobih.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2pgmyupmy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bkccnxnd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2yqgpbnri.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xyioylcz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hhcigidq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ruxvnutd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wzrixejx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wsqkwimj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vpwdmqya.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tgpffxtm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2retayzjx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2phfpvuje.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ebgwcnjv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2purgezvf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2cpmmxaxh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2cdrijole.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2cbjikkfl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tyuqgztx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2csgpfqka.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kguxuhga.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2hpgllcyl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ybfazuxy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uhlqrxgd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2olkikgyn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2evmybkma.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2fhohhfpz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qrecovqd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tqrlliep.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2fjjewbqn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2htaxyysk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2yzesyrtm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ukwvuskr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fiwnxckb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ndvsemyl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2haobhdzq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yjgqelxx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ndhsuibj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2gidcekuw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ltellcep.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nbvmgyxq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hemlqsxc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nraelpmf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2emdygckt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jlcfzlfc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vmrajxdm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mpebeuka.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2pazmzjht.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ohjwvsnz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2gacnzrrt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wposorbk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jqlixhce.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tybaxqte.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2hzdbogkk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2suzeadoq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hflgxsvb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2mwxbmhqj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2kotgjztm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2riywqmlq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ntzgxwsp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ouqjntrm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2glktsvco.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2uoloabaj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2faodsvlq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qeulciey.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2zbnaaluj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vpucwbqk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2eqjnalav.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ndcxqpll.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2khvhyiwg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fhozwrgg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2woizlbod.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2qwfuhrpc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gmzqcmkk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2nhstpdwe.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lgdhxlln.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ewhdpcwd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ycueqtvc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2nmnwswat.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mbbaazjk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2aawkoxfi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ijndwqhg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kwjimnvz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2kodrdvyv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2pnwwxzqv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2msmsuzqv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2yqixwwav.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cqrevfzq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2olbaidmd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zdfghedy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2plmulqot.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lxunnqvb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wpwwzsse.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2tcdlxnrq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rvmqlfqc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2dqqvevbj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gcjyvqhn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rpqhysuy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2cekkxdrg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2cbwhbxkc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pdbvwurc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fpakuhct.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hjqtrjri.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2goghtbef.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2hquvsbth.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2odnnhqya.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2crlrvqva.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2muazgxtu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yhdrstjy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rabxwvup.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lqzckfbz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2uaqnunlg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2anefzrdp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2yzztkpyz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2elavcntu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2hmmfyont.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vlieswew.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zirscwnc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ekcchdsi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pdshkcoq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2evkugxwx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nmpbjbod.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xfvnmszz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2pbnaoojt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gbimkacb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2skeodefm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dzbbftpa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ifkvthsy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bizzsokt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2cmikxcrn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2auukawlx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qzgyadlc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2gffserln.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nbdywuyh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dctcuykm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vglxtvzd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wexrmfii.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2irlgalox.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zdsynlha.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ytvlwkhw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2artwotui.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2dwiiquuu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2juhxsnia.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2glfejaok.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lknmrpgk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qzkikotj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2frdzcstu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iedvpyya.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zjuwulli.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wtaquvig.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2isgbxfvw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2icrjtakl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qqjwhacz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2avbdpzgk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pwadqaxr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rpjwwmss.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yxjienfm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2dhxuquzg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2tgjhqunk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sebnvqno.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2juzelhsx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hobvifmd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2pzwdddcf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2shawvgbw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mutxfzeg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2acbgqbos.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zesjfwkp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gzuseqjc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2afmdggil.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ortrcjoz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2axjcingo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xfxzabcx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2adyuwkde.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2eflluufh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vivzjxbu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2tilliyky.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sqntckfw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2nkwmbrdh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qbbuihyu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dtatfvsz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vposijxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clsnfqlg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mlmhyjdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jedzzzzy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zuigsjay.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2tnnrbxkk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2jhlwczdp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lrmdhflt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fdadwzpx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nsyxkbzx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ftpcmfrn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2rwefyegd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ayikqjyi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mendmhlq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hcphaamf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2oweinosv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zvwyvuwx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2naiiokvr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xefzqdvc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ivferisq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2flmneuyq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2akypoljh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2spucipqx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2pkdonlri.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2suzxdbac.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ztiptsif.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2juygocdf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dofvkwug.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vpmklttr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2blkdsksp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yypalxqm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2npopypxm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vpmifrhj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qzlwhoww.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gzlfgyep.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2mngxmbhz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lwhnstqr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ironeyqk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ddtozalf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xkuufpyz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ffycymcr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2mipldsim.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ffrimbuv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lmktmqmy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xrlcyhqa.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ehiqxybj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2afltuzta.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2euzwqowr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2emgkzuqq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pqxoaugj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gytulzvk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tpowaarv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jhtkbeqj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cbyrlsdp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tpsrxelh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bcommyff.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2upeditln.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2aigaokwl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ahjqjjil.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2hfrjoilt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vionmlxi.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jjyuthgt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2jscbgmqq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2eqooztte.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nnuoppwr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ohljenau.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ogvmpbnx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tewricla.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xsndaewt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2gwbpixuu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2erknsqse.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cznabcei.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgebrbct.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2gpceoyhj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2efullzvl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2swzwcaub.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kydhexlm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2avqiogoj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2uoyrnkmk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2suuuzbja.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qdtzejkb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2menniqqf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfykboff.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2goykupeb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jywrjtcw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pwuklwqd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vmaewywt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2thqggbpl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lcksamgi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2nyekinzp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2frmwhgxd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qrecqkeh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wsbadcag.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2cyngebfw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qxwgsudo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2aetfozkx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uebxhnob.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2feosfmlp.html


<!-- 参考信息 -->