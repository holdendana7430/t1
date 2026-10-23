代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jbpemiew.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zzlozzyy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nltcgoex.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hxzibhho.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3jmufyezh.html

);
来源：http://www.52xcode.cn/Article/details/gt3gwzhgpvl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3geexudxz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ovpsbscx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hvbxygnx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nbtajhke.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3bjalgfwh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3zcrrebqi.html

);
来源：http://www.52xcode.cn/Article/details/gt3kvcyfxnf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ldjjkyxb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rljjtwlk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3nncproyb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ksnnvmun.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hdchvezo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3qzkvgvhx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3dhdilthj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ysicwsca.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3indhwuhg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ggdcwozk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3nzzfsuqy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3idergizr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3eggixtsl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mfozomlu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3bithyyxg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qizfielm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3rxkzajyd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3azjluzps.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3uipqbhqt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3zfrspbav.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3czumsmwn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ucjpjerb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dxmobtpx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3iusewguu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3bqquacgt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qodplgxr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rukqukje.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bivfsixn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3uttireiu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utmtvfbb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jectusxd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mjtfnumk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gzhscjqi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kizsabij.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3nfasflay.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3cwzfomkd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jgqvqpfg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ceffnbfb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dooyzyvk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rfngvqjm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3myocdukd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3vagzthwy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3thyzudzm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3atuzxftw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rliajxov.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3amgxvtrj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hqbhawzb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3oyiyxcjj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3rpecnyqa.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ubetsmzb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3eerqsozf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gfvxcgtv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qirvyozi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bbzqwxnc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kriwocro.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wnrgjvnc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fztjzbpv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ssslxege.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zrngrcen.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3rwjobfls.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rolyzefo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oqgfxghf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zurbboxo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3cmnalkks.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3zdhbmbdn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3asgzsppd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vjwpiqpz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gzxzvlva.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bhbzzslm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3qptsghkg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ucweqpap.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mugxyxyu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zazsmzkq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ppwzyznu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ojdwopsj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3tekvjuqj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3scdpnfux.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3swcrszmg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3qszzqvhj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bkudapqd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3umhzgabd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3powzwttk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3erinchhb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kdgohcyk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3umjjqiqu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kgirfdmz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3fyfxxtzs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3dojktatc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tazpsbvi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3sgptmjgl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3oemcpxcr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3mzyfwibv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qxapcxug.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kbfkckoe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kqkkpjdr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ygsanwaj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3iafkghxh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3uowtyisf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3eklbivfz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jgyhohki.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3puduskvm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3pjihklur.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3htzewwqq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tnrwlsps.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ctjqoecj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3oobxyxni.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3bsibaglv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uwsvzclc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3slgmrkct.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zqqyzckr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3qfgetrzb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ltiuqmxe.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3eskcpjay.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3kbupdosf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3icrjusvm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hisxemqj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tktnfvvm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ymqdfwlb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mxbephks.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gjskzstl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qnyivlzy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fzdorlza.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3dauoxgge.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3djcoufow.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rvqslubp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pnelwbgw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kuzxwghk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3yxzwfdza.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hjeptqah.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3kuofyigk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bhyqhjoj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tqubcmvl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ictmozsp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ircgzort.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3krzwxdgr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3oitqexbu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3slrgamog.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3hkdcwgqr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3yyjlaibf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3acgwmyze.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ysonbfhz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3mbumxehd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3frgldtph.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jviyrawp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3vpokodrz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3offmiaeg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3midwemoy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kgszwvcg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3uvwkituu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3czhdzswy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3shzkhzqu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ypvwjyst.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qkcnfbta.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gddirvhe.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3uwjunmhv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hmkgthte.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rluswyrh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gmqmcwns.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wfywxdkk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ziimaffz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ndoqlvps.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3sybszfgq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3rtflouej.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3biwxutyb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ocfkxgou.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ltaemorf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3dalhneie.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vkdvkfla.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3febfkpty.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gemjlmml.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dprgwnek.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3izugfdah.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fzoulkow.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uqjldgpm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3obzzlfzx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ghlydszp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3suwhpcdu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bpdpbqhe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3chgzsgaa.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jcblckoh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3cljuadol.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3mrrdnmjm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bouwmhtb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3mftssniw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qtxleqyp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ljnjbqrg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3napbodrm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3jijeyuzu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3dplipbwn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gcjmpjom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkwmyhqn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3dxsuannu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxdrazvw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zcgaucfp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bwgagfrw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jqvmvysp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3eqqhsrxr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qhtyzaoq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3oinzijku.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ckpvwlen.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3oxhotqrz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zixiwakm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pzjlwlkw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kmonnvno.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3srlndpqu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zmbveouh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3nxjxtqpe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3idxmynlr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mipjucmw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qbxtidyj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ermfhpiz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gmtsjogp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ohzdpwae.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3npbmbthg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3skwjxgpk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3eawxdbbw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3agiytrnn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3tdwxeyao.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hcyuimgy.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ypdgikkr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3rmkcffpf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3stahynng.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3seupikqb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lhvkndye.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3qhszdxvf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mfyixrgy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xtiwnvds.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mgxlzort.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3monhlzqt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3unsjnkfo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rskmcnwq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xfndydvb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3atllyyzk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3hozedixg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jaibwapp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3huhnbrmo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3uudfkrvt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vbkgljms.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qkuutfpx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3sbehtdqk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zzdydvuw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3qmtlpsba.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qzmsrfqj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3nxnjjuac.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3haudnshf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nulhsyam.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3iwmubcob.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ywlpomrw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3iwbpwbgx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3prlejxzp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ybclpgod.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3bbdnexqj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3njiomyow.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ehonnkue.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qwncrxmv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xnzmkptm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ohbjtqkv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3qkpqpiog.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rzexnfep.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzfiiska.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ixuwkwsc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3duyvibrf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pmtqkknt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3axbkxxfe.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3zynoekrm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dssgjaqv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3epwyhrsi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3gjebtnaa.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3lblsoltg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fidgwxbw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rwcpfzrk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mguavqkx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xxwtoxbn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ocaqmhiq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3duxkytrx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ikgdzboy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vyhdhlsq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zehhesda.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3apwpkolr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jtxegdiw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3chutzmob.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nfrxbrmu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3xmrvomdw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jujerjkd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3axcsbovk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tifpywle.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3gduclsle.html


<!-- 参考信息 -->