代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3xovocpta.html

);
来源：http://www.52xcode.cn/Article/details/gt3hopyrrjl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qrvprbbq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3rkxmzbjo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lbosfvac.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jpstfvlu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ltnvitvb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3tacujpon.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wnzlyjrq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3tmzlcxjd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ghknzvkr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ugdjipiz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3jdlgezhf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3kwzndfwu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jghswozd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jiuuyzne.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3tpfixynf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3joavksgh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ggfzyvqn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3zldhfuod.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tpkxkfty.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ykqdfdsi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jdtxuwgj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3myjfeclb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3frdqtnmj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ojwyonva.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ghgqxrgp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3izpzoppv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3nffzpppb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3oeuznwhk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3wgtlsklf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rcmfmjqj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bwcnesuq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3msxghvzz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gxsajrqs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3haaylxwj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gzbcdfym.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3iahekgwk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wyxjdlml.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3lewajnut.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3tmfedpnw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3stvkdscm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qfyqdwpu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yviokjxw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jrattept.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xwiqlftx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iwaduvrt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ibathsya.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3cyjkgasv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3sqhahden.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3zqepclxs.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qousygjm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3obtbynsd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fjtbhndl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ketcrlpn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hntkxnlh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nvdqbtti.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3idrtdprs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ykjbdpgo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3gbptfyga.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eygrprem.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dizememb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3runmnyzx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3oglzpnok.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3celqnkws.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3olxsofsz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3objxvnkh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dixjeapq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ntxywtrl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zknkvrit.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3upykjjtb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3sudtyroy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fcvnghys.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3rsfhjwcc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3aijhfwnu.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3etuzdubm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3akwuwkhs.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ijydhozd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3srfyqmiv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gncjvrjc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3fmzqlyux.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3knozcpqc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3bxeeizgs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3coggkllf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3dyjxqkfi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tyyqdipt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3fgpkpgdi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3sylhkqhz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hrmbqnxx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hazbydtn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3kcnrfshy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ulcvqseb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xgihkpoy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3aitwxjtt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3iuqwmmhb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vqidhcwr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qwdoxowa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3bhpbdiax.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zeudsnej.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mzqapyuu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tfcicbka.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rfmuavpy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3etclclry.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3egsrmyjf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3pclkjnqj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nmnjtcko.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ymmxwkpb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dicesopo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3heyzehyu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3vbvrqwyv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kdwvixgd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3psvujgmi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3smkrxmbk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3xuzrexiz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xnjtgpio.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3phgrskkp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ehnfosug.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3khykpwts.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mssnyojr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ylxcecsg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ngzzpmwu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3tkukjoti.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3vyyvlhme.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3uevdhvcx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rtxhttyz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kjsiqsre.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3iwtdvptp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3suoatmys.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utvhyrnt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3iijtkfsw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3txaouidl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3uoatlqhd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kfuujfmp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3njzdtjbh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mtppezot.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qarkbjkc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kpyvfugr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fvszwfaq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3femhtmbo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gasyjewi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3plhblzgr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3iuvisskg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zmhwwaej.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3imcrlztg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3igpktllm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3iwmfdgev.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3oqtdrlrr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vwgtymwp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jsfcksvg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ommzdped.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kqzwprbx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3mdwrwkjg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3eradlcdz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3veqmyizr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3aubhubfl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vgozklgx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3puvpuocp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3knhtmdso.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ltocnigv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3apqehaab.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gjdtkdxa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3svhujjxx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3racilvik.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3mkdoiict.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hgpwxdqn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qrwxyewc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rujyrsus.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ofwmpixs.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3gtanjdbc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rssetzxw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3rztnyldl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3pppkoivs.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3svvpsirt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3jfmmebmo.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vtuotwmb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3intodeey.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jxcrgqpk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mefqfvft.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wyburpxg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lzkdawql.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3rvifxxub.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jjkidsil.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zojwnnea.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xshcyloa.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3whusycps.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qmcuyeby.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3sylaldmd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vwsdpooc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3hoihosup.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3cxsjwjif.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3esdzlesa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ktfrggfi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ujhyqllz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3pvfheqaj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jzqwuire.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zgjdlbll.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3epoqmvzh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3hslxfpbz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jkezpaos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khodwbvd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vfxyucuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gumcynvd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wtunhzbv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3fzniqyhl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3iyaxxayv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vrijvcqo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xbxwuimm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3nensfwbf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3uqeccitj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3erlazyst.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ymmajwxv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ysvcrifk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hxonkhvb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zqqprmse.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmvynhsn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3hfljvsmq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xaxccpud.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3quxksmuc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dfpoceya.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hgzfvewq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lmosllsy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3mcuwizpx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dsgymciq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jnctcbbl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3snkzzpev.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3wdappdgo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sacrtunb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ybehvvrl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3aeoqodga.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ippigxvn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lnlwgazt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hlgqoqkn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pxnbnsqw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rsbfuxbs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cwjjzqpq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qisfivdu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wklvhyim.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kcmmrcdt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3stuxlzzl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3puwegfxo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3johzijmz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jyfpceds.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3exowvbzo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ilkojshl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hvrtatcm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wikhqdbj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3gigfwuxf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hhrphmzh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3gxmaiboo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3aqufbgpb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3crhmbbbc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3glendlkt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rnspcnft.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3actdvtft.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jcxjubpd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3dkfgqfon.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3biplcbqz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ppivncon.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3yjseurxh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3hruoskcu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3khavlpax.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3iunjezxw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3usjylnfv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3btraklmt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jfbfpadu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3odgsgqmw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3slmnofrz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yjxqwkbl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3syeahvzo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ktmtglwf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zruljjbq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3uxbrjcwo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3gmzwmlkb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3dymunleo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3msmpiypo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ykiruedc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wvrftmhb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3fotynmtp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3hbfwhlww.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3dkdsmimr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gutyhnwo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mtagdumh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3kipnmcga.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3agbvragm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fnjlyskb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3wgvadthf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3agkgshmh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xlasxgqu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vcdatqrl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wqpxylcv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3jkhgtaqt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qkynbort.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3qxjdohal.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tmkeafiu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3apiaelsa.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vxxurulq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ifzlhvqt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3aaginzxm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3xdlawmqa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ndpuahut.html


<!-- 参考信息 -->