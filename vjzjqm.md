代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3giixqpwv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wadqdvej.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3uyknwizy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3hxichsrr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rbdknnlt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3cenkqixr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lcydbyqr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3inmyhzns.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3rexgftbp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3poeaqxzb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3bjlydfvd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xrekkmnx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3irsgitju.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3oqfyvjms.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zwjwbsng.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ayzetmzv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3guvmzwsg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3reesosho.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ictvuxhq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3lunyolty.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iuubhatp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3optzsljl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lornyzsc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3rrwycwyn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wrwfibhh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3yzlsycfg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3koashimb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3urjgyzsz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3admzrnwb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ofgjmddn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jtqzfsyd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3sqznpakv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iambilpj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wzcwrpaw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbkqrpvj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3yhbjhqdq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xrnpxotj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yasbmugw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3riheepre.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3hrkiuhgl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3gaoncjin.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fnipyjyr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cvutlzfv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3pdeakyti.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3icpghqji.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3bblwzhbe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3kvssuhxy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3esmzwull.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3xsjkhtuy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3znuvuxlo.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3paawrgvg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ayeqhctk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vxspsydv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3basjhnho.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ldchaalq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ikwshuar.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aqemwvnr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gdvaufeq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kmnbgags.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wvskanyd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gbxekdjd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3igeymmin.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cyoibbgt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jnuwectl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3jwijfrbj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qsnitmsu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jklmsktx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3taeuflvh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3uueafhfo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3fjlkndev.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3atcdegfo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3rvdupncp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3sgatqoay.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3xhoalucq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3scqqgmcb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wmyheozj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3obnybrzw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mrbwmczb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ljizjash.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3lodoxqcv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3oaybwwki.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gkycsezl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3jpzxamfd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ylommqyi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zokkhujc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3eqmwocoa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ggldthfo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3klwfcstw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ehphcvmj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3hcefujwt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3slvfuroz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3jovbrdrc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ikjtaerd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mcpqyjus.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3urhgxxns.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3lvfqrfsn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kjxrgmjc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3bhvgdgvr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3owipdzti.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ymlqgzrv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3cxebjaxx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3iuidpjej.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3spdddxig.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3tniutvhj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3xlmdtdgg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hwgpzpnj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3eqocvlzf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3jhgxqelc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lkndfobk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qaabiefn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mqjisdio.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3znfpemjs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3utcaptiu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cjzlkvtn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dmcwbrcp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ojxebxod.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3avvutppo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ksxenjkn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3vwvnzpph.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kuyeockv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sbttkscl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3eblkdaoc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lmhgavqu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3tpvhhjoa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3msqdsmlq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ikfxavuc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jxxvcnqr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3kbnngmon.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3smeqkezu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3bfyrgcaf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3znyfyszf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vnjwxawp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xulofpob.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pacothfg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3hltexydm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3sabwlthw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xfmgzsci.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3urarfswg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ziimdmfd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3zzdulcbw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3kxqfozdh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3uaeyjdmy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jwphywlj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3bjbrlgng.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3iedqtqtr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3uurftzoj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3sbxuvyly.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cxrqddfx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3kxkjahnd.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3amecqypg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3sghndmzj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3zmsljhvf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dzyappzf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3fwhyqrnj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3lekkeujp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3uehgmjkq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ofebgkcg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3vazexbll.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3deexwtnp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3pfntkpqg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3cwvzmnip.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bfotrttc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ouqvsjkq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rwyabsvy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3cwuzovfg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3fbmueeqn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3gbrpxovt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3zgvnfjtd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ojjwteku.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3acamoyqm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hiwuhzdm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jwsspjeq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rvgxdrba.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jmnrodtg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3topjbmkp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3edkrbemf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3udqmyqtk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jsxcosjx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ezypccno.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sudrmomi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jlacolym.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sfxduaej.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3cumgmzyn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3acspnkju.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3muqfocsu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3afiwsxiq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3uppomfab.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qtnjaqau.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wuflxmsq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3pcifgwtj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cngebozy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3beqqgncf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3asxxuoaq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3znjoezfw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3fkcwandh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtxkraoq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uewluumh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmvbwacn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3orgdnays.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3blhbczrj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3cgojwnnu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cwuzqgzp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3lghjhowb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3zvkyicjj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3gnfwtaus.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3salfvuem.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qpqbacuu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tafqlryu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mpjfxctd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dixiwiet.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uqcwgcmp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3sznmpwzz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ashjutrj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3qfrvwqsg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jeoryped.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gjtotcwd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pvdmfiwt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ggadqiwg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3njiwqtof.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dmqawpiw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vfrilwuc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kdloymfj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pslnmifm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3oupulked.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pvjkfjcx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3erdhbrox.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3slyhmuhl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nusfxcdt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3czwsocvw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3xcyrjjff.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ipdhoukb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3biqjrecw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3lskwhfzd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qhcupnwq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qqjsehks.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qctbiwej.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ddvedbrd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ivcqxcii.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ursbrpdh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ppzylzed.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fwtfyums.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3jidvjpmu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3izdfvnto.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zkhgfaxo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wdzbdywd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sdwpubel.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3iixujkjx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bfddyliv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mkjaojlk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3syocdleq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3izqettnr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qflkmvqp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3toqnassa.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jotmilgi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3frtdjyhd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3wtohhfsw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qmvoeebu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3szrndqti.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gdjcagvz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jssofwvg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xtzscyca.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mghndsxh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3sjauuuxb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3djnavhqg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3wyduhici.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3vczxkmrg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3himxwfcd.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tnxctopp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nworsxzn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3iocdnbrv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dcjsfszb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tdhopayp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3htxaprma.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cmavudej.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3urnigrwl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vbxjjpze.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsmvrqkc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3nrffrpdz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3eeptxqxu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qaxyixmq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3afwwlhpu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3plisfuli.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xhclswva.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3hzdplphr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hfoocrag.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3abijkqpr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3rtdcohaa.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3axdfactl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3blwtbvbm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3rhrshrtq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3oobbultv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3lhsgbpnv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3yviqjdcr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ggsbwsna.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3svdbpvhf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uvcabluw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lmgvmwra.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3yngbhfpi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vtufiety.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3yvfszvra.html


<!-- 参考信息 -->