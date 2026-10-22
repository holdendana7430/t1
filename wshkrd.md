代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qgpewkiz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nkemmbci.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2clqkapft.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2lskmfvnt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ewxmahdm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fddlahpj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2zyskyyar.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2gjuybrrp.html

);
来源：http://www.52xcode.cn/Article/details/gt2zttgtvcb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2koavsfit.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kmeynlfq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2qyhmlfju.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2foexfkax.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2miqeuhgc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ozikvhpv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2pgxuzfso.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2brvczqte.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ldbpquhh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ozgubbjm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qhxsuhvp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2asesxqhz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2yjxxbgxf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xjixjkpw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rbbmgelw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qdggqpxo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2cropcavl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ghyhywab.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ekysleyc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2olhqnkls.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2sxjrgqus.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2eqnapyuf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dccezdel.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2kwgheyyn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2hovojzed.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ftacwttx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2hlbmbbte.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lervrohv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iexejaqj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tetgwsoa.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2gqwgopvw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2sejjysme.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2fhqvspfv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ifdjfpre.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qqidsmxt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bpddudvq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qxzkfzht.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dxttqlnc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2dzpbtgmb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2impzfbqa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ikvnttlm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2tcxwmpza.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2jdyjqdib.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2duzriibr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tahbhqht.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lknjmana.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2eqcfoybe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gcrxiryo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tyyrdqll.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hzykafiv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2nexzkivm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jacxizgf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qsjumisp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oeormpak.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mkjlthgf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2efauvtbl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2miibznob.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2omhrhgsm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wvthduot.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jjljqalg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bhkzqpas.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nghjkdya.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2apiacsbc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2zpdoounx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2iammlbkf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2atzkguba.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2jlvggohr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2nejrfvyg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ahoetmus.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2sjujxlhy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xyopwdur.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2pzlnirhx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ymcnfuyq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qkkfgyuh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2laknhflq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2iabgpljd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ocwcpuzm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lyfpobsh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hwvturrr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fgzqpmmq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nwmdppjx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ynfozode.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2tjwilkut.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ismckjwn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2bdswnkla.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2rpxsmyfn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2dmqgsymj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2sdtrzamx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jttzmavx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2pbhugbdp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wdbyvnhb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zlzbjaff.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qqzokrvc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ktmlkkhq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qgxkdrdo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2itqterao.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2oexeomqh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cultrtcp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hlesfnjp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uoaznutx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dktuwsbd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fianjfed.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ygrkeyih.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ebplehto.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2pwwgnpxd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yfoeqbmb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wcmtioua.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ugnqsxhf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2dhbawaix.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pppftfxw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2geasdpxc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ylccylhy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2hlacalvr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2itopepaw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2gwksrbal.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oykkwmjz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2gilzighm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jucuuxrh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qnvaujqg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wrsuauvj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2reqxcgjc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gntrnemb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jzbzhcfz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oepdvivf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qqklbony.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2vmeylfpy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jvisksna.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jgwrdcud.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ucphtagf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2phnoezzx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ripsuwum.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2fcrdjdxm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2yhvkcovl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2rjeppzuh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qlgowxzy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2pwsqubil.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zumfzqwz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2sfqrtutj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xcivgdly.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pjkxzmxd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2asevqjvd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2udwevzjs.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2iahdelqu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2umkxyitg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2fdtmgkqj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qjihdyob.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2rsuxryoy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qtnvzhca.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mqzicdjo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rsplfidf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zvlknlxj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jxpnggey.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2imzsbest.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vnxqrwiv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yylkzkpg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2arsmvloh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2njnmsfea.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xubrhqgn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2emfwpwjy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2zqxuibon.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2motxivgi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2isaxzrrj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2srzrqjgr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2yrkelvvp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nqbulznm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2sdmyigds.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vingxgak.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2bcmwyyln.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bppcjxll.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jigcvfba.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uscaaunu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2nhzqdvbc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xwldsaav.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mbybyjpk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oxozcgae.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ottlazve.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2adyfzwpn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mjzljeqw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2fkhnwaxx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ouvnjqtx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vzxjsyib.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2orjuxwyw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ebhadxwy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2axcyddax.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2pepazdkv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hcdlairw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rwpgqhcc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ppggwojm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zrmpaaul.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tvkydjej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmvjoemf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cngnuuyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtmllbsa.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mmlbhaga.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2fjsuaatt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2uobrwkgm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2vqsjjhzj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ykbxedtq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ycnhgjvj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dkcfnviy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2xuvtbnuo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2tzpgspow.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hhfwkvop.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rapfogtz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nwdybqjx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ptebaymw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2tuftevxr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ebabpvjt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ecbakivd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wxcqiyzv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yrwgihgi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qfzchwtq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ovwpspvv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ogdlmrgq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2spiuvdrm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2sfhdgxyt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eaktrvel.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mujhpliq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xyfovtdf.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xqvcpyrx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2upomxqxy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ebxhpnjw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2htbwjnwi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wjivkqmc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gaargutp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qbtiikbn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2arjbjodk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2odiegfwu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xvypgsgt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2arnofsgb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2bsulgcon.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xsreirkn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2kznevoiu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dvxkrggj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2eroyarpu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2zjmdogha.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2cuhgsmzu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2mjaeehzu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wyhoxeaw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2nzdrrsmc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jdkmpazt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2pomnqrob.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xaqcuwjf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2clzpomeu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tcwdgwhw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cotmekuc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ncwcmjzd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qfbzvlmf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zzaieldk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2kcvwpmeq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2webhagtw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2jfumugpb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2krpgeuox.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2svtykvzy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hebxnaqr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dwbzbvdm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tbeydhwj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2izoogldr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2folzlvyu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbflqegw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ukqogjvv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ogymzzgd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2whjfslbj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2onzzwayz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2geuwzicg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pbjygyrm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xjhvvjsk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2vcjcfsbj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2pzebncgm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2amquxjtx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gwwuowqg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wxtxrpsr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bqetvcfe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2tcqyweod.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fmujsbil.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2laykhxtt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2aypoviet.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ejsldfyn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2krfkqrbm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kgfneqrd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2pnxtcuxq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yynasflc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2hkliroko.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2dvaaljku.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rvshvyvs.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yautdacs.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2msxbzoxz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2uphytqfg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xtxprdrh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hcpjakbc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zbudsgbp.html


<!-- 参考信息 -->