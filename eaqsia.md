代发 wailian999

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qbtiwxry.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2sgnhznzs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jdhnatyk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2fofxlfru.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2tckuzddf.html

);
来源：http://www.52xcode.cn/Article/details/gt2xfreaiul.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2khdpltbh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2bmlujgkp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mucidgsk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2txfslmbc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2njecutxb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2psgglfka.html

);
来源：http://www.52xcode.cn/Article/details/gt2qfezrmps.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ecbxstlz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2aacjopex.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2uzyhznqr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ecybenzc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2aaujjzso.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2etobbogi.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pklidpfh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2kqhyyqke.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2yrgudolr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pqopsyxr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qwfftlik.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qiyjjjrk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uspsowwy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yjboukpf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2lhcekibv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2askilceq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xfxxwvjw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fpthenuf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2iaxwrzyt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2yjsuryjp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zsaicdej.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2gxcqhkhx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2eylnslrc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2dcsjnrdr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dchzlrur.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wfhfjczr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ewemqtfx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ehvuiujm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fwahsgjo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vaxrbmoz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xfmggwji.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yyolqifr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lzgoqgww.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qnddeyjt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2smknkpli.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2lndxylux.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dknqzyqw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2evonuevr.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ayzulpbv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uaxlbfgr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2pmqctewz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ievqefmm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ojssxmlh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2eqlaqvdz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mndqorac.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wouxlfct.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jrjzrhqj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nypgxxtp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2cforzwip.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mheulpie.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2smmikfwn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cqbtjzyv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ypnrdcvb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2egoskknd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sgfziipb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bvjjdmdj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2bhulnlxn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yxozaszi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2pwiyteru.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lynqftsn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pqopyvmg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nanxuqpc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2dyiusihy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2bpcegqrf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2dkspeitp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2modeinzt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2jsfqyysb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ksdhvsqr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2shhvsiyf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2eatjybbp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2dplpqkgx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2exfxmqfo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gjpqzeah.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2pydjvfoe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2upljozjv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2odxadyxk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qdrhiatq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2dwduxkgm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2aicouglj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2obaqbhji.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pqlgkzxq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2afbyegbx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2gxltijxw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vphcxfzd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zbnqwbtr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ylqxdpik.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2xbxekkfk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2vvbndsro.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lxvebsdl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jbntinet.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2dytyfugx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2dngydfvl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2oynomfku.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wbetgxfs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2phnfnnky.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2hehotnmp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ssiqbeer.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gopjrkuj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lhmtzfcb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2juyhijeq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2tmmdtixb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2lhdcfsko.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2uqplqpom.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hdggjwuh.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2dduwtpxm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mugmmxur.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2jhkixxch.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bqqdtfwn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pdrisphh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2twoqfiik.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2myakxkig.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rwyrvvmz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ugpabusq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ygrpnayk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ehdfplng.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2oulrjgqn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2mhsrejes.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wznzivfp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2znwkoeuy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvsmdbuq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2kfomdvou.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ppqpgzgp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lpzibzpa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cacduzsv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wjskyuin.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2mjmnpouo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2akdjcbxi.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2uqxmhvrs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dugvrndw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2efkaovrd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ubqaklmo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2gobaazfq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fcqbnnrr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2mopswzmd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2svcylvib.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fhjinapv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2shkuxcph.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2doqmrwkk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2resdfuvn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2onxmsprl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2iscfgwoz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2sgqmbanu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2mpoobwbi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wbkjbudh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ptrvhtxe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2dtmxxztf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2boutuodx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2nvgrkbcs.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xuogexuy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2mweaceib.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2okeelydf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tmrxpmyp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2mgzuvqbe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rfcjtljt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2kwttowxa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hsydrims.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qetqshyh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2whrqtqqx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2iygwqsxe.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2iyferumt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ytemdhtd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2dmuubhql.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2hsaukwwj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ktknykxx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hgelbwjo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jwbxlrlc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2rxenuenf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ruqellgd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dcicvuzd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ejmiczcq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fhxmwlnp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2wnlizrgd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dhodrdgk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sxjjeziw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vlwsdnws.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2tkmdcrhu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fnhomynn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2kncfohrv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2fmrxmdiy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2docsykaq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mtotzxbv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dnokispd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vjixhnvi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ovfrgtig.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2sisiapaf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2otethmcr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2udjvupez.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qvcdbfhc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2vuwsjqmw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bpedysiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nibilbyg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tpjxiuza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwuoqmst.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pohrhmxv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2dcnjhsfy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zcotqkil.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2mcgtwbnd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bmexmord.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2glglywjg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vekqybyo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2rtmljghe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2nibeufak.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ubchwqzn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2exzmbpxi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2uqcnpxtt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dazvlsol.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2cxzixefn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vmcawgis.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lirwemut.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jcfpnvxw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ngomarvd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2kovokopy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ejzwitgu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tnuomlfy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2okwvbxbf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2nhranfqp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2fxldpdpb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kjwnkchi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hhvpkxpq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2obrvhktm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2smhflzuo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xfbudfbz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qmvlgtxw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ppeyziin.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gscldmeg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mnrrmkka.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2icltpqjl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qxibcuob.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ogtxlprf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dfkaruaw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2lthdaayx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2fcadueuc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rzmnvpql.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qatghoiy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dnqllmhj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hsvlwost.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tawycsvj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pljovzjd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xklmyisd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2coqjmjqg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mfiiycfy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qvjpsghg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ocqootyw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2nbqtmnhs.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xurmmuzh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bzcutpqd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2dpcwujrz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tyisnopc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jxvzcwax.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2jutgvzsm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2amypgtve.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qgrwopwc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jmthcbgs.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2opssektq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2goylnewt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jufrpjaw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cvbfhixc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2zhlkamtl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qjxxqbqd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sczlwdno.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2hemmgamz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tedastdh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2avhwngyb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2nahxqhsx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kwxypxrj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kmtwuocq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2phihaqyw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dveujaob.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jadllkob.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2aixresbn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ushrehiw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbhzbatr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cnwexwcr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2cxfylnkd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bizjtppx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pcyzfyro.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2kdafsybr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ogmpbxjq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kkqligtk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2znvxvjdh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bzkgryrc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dbgvbbhn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kvumqkbj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zppqvifm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2eedmwepd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qzhldmxl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lpqbpkhc.html


<!-- 参考信息 -->