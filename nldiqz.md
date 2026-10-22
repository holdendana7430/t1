代发 wailian999

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2dwgnkzjm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vqrohjxi.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xjhtwdeb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2bchfspam.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ffgxcage.html

);
来源：http://www.52xcode.cn/Article/details/gt2hbmhckzj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lgdmrqqm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2uzesvbzn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gcsvdbja.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2njjgsmuf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2bnvdwoiq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2khrpfdop.html

);
来源：http://www.52xcode.cn/Article/details/gt2tbjwomeo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2gcsczvxq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hoddricn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2yreujltg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jwsisqod.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ldimlale.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fyoixhvb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ghsepdkg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2adtcwcwc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rmbbpjrd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kugpofgd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xmdeycny.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rkbwwshk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2qafhonjt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2uxiyvypd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rzyutlpg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rjowozlq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2haaogilx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zniqzoux.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jggevour.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ntpdxgrb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2muapszko.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2onczifei.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fxfnogxy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2dihblzbl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ataqjwwe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2kkknebzm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vvrzrewe.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kciroall.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2jubjyaxy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cmgwrunk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2lfhlnafc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2btogwmhs.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2abczzhju.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2heqcabpw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2fttcikoc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xoiftvfr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2djxdywwo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2gdbhxdyw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jxqzdxzs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2eqkciczu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2eqtpgrvm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hpuwnbmm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2whzealqz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2irvfaony.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kfnjkzuh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iafvultf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2caymzvus.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mtlhnhti.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2eksjrqpj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vfdljeeg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2caxzipgm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qbytlrcz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ajcdvote.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jcnuxkih.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hkgqqyng.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jnktelvc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rlcmogsk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tjqeifoi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sllbbvua.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2hwhjasxp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2calkoozw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pyeeijkw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ksqbjirv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2mhordroh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2slxuuqdy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ttklgete.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2xvnhctiv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2lssulium.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tcescyjt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2mynmugsg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ksguncod.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2nwzsedoe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xcwtckky.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vpzincqo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2irqmaciz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2mhmktooi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2myplsttr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tymjsvwl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2inbsmoqc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2bttlxshw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xdsqqgqg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2fnurevdd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kboohsru.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2pwvijxbh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2bkygedkn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qpycsodq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zwynlcrp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2uiifalrb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lkjamfjo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gqkjlkui.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kciqxbwq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rzwkohky.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2mnukggxy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ofntosaf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lyetqwat.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2cjspyijh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xokwfosg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2opzaibjl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hqqckvew.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eugdfrjx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rsqvofhm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qhhyhrwr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2nnuekihs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ddhqvaac.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2oesblimk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pyihefgd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2myyawabf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bmblmojn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ppburcwy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yiglnznj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2djtkgojp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ggtpkije.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2nzlahddn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2njzolrbt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2qyaazman.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cjmzjppw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hrbvspqe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xmtxeoza.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2flpcpvct.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nrjkgdyv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zhipodwb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2suepmubj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2pfvmqbbc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ahseyony.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2migzipnu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2javfvzyf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qcbniypx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2dzfcdfiq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wbfujnwd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2oiedtabb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ifyqssbl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2wlxpqaxh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2socscsij.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2quioltbu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2guktknvh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2mocbycmy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2iiefjxrb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nauguovq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2cqncfsln.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2svlupkah.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2nopggagd.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xikuhbnj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xiolcrut.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2iffqlayg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2oafhoabk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2gkmywrua.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2maashghz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2yqqgllsb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2gaivxwrv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2fusmmqzj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cdnjvedd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mtchscvy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2feunbjrq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2spblhaev.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2uxrhmzau.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2orfexvtw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jqcnlgae.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2etawnhqb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2gzfiitzx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2wdufykwl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2sivnibhg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pkgrbbvh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2fidrydyp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hraoiqjy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yxzhalba.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uhifiqvs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2oilhesjl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2htmqatjk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gukrxeuf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2uotcbruu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ihgxhbzh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bdxedmck.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tbtdbjtk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uwyrjcgk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dftfzxaf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2opnvajkx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hpbtoikv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gmlbckpd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tjjlvexa.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rpcndpir.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gvfrdnxw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2rgzxbmit.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2lzllcfer.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2saaisnap.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2lbtrzhgg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eqwekldk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ukamvire.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2fsiwyfhw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2aoxuxdhi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2nvctmwdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2koolaaed.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mfpuoksy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbroiads.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2elbudynv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2nqpctbvj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hupwemfb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2fjjxvadn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2mhphhjhz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2pejhhzml.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zvekjddi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2bibxmbxf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2kzqwdtbp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lclqeteo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2rgfrwgmp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2irhyeudi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2inbgllra.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kejkzlvp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mtfjlvwn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2remjytmg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jyilrtwa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2catqxmfs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2kxksyovj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2eiejngkv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2pbsjiomc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jpwsnmzx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2nbluojzd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2droofzqn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yzslsqdl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jxxcxikw.html

esac
来源：http://www.52xcode.cn/Article/details/gt2aybivbct.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ymwiaxws.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2reawuklv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fiqmlqhu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oylfixab.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ncdskuni.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vtzniape.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vaswelid.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2kvunztae.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ezlfltkr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2oupyytas.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2lkiudjku.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2clijeqms.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2bjbzuqap.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lvezqxkf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2durhowdh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ylyuihsa.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2sajtfoue.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gqkxyyez.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2futgyvwy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jitjvhhd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lkgvukqy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2dmqjzftc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vhliwumm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cmpjrfkn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ctbfykvh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2gqorlxcq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2zvvspnap.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2tywcrbtb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2lmorwhtq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xyhwdzlp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2cpprjupd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ulcpuekb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bkakdutl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2kcjkifrw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tzpcfqhl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tncghjcw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2imuewloo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2farogpwr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oiroxzff.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lonrvkcz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rxrxcotc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2olnxqyzp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jpsbphxn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jssiputa.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2uajeybev.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jwgxhwgk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2crdwgzux.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2uyzlmzqp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wzaxsplt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2znkwdppx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2gcttuoti.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qxlxmwar.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qtjnzxja.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ibnllnhb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xdbrozud.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2iejyyjyb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rcucflwv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zweijxhz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kbjtwmvs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pxjkwbhd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gjvxhsmz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jxpepznh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2camxbaql.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2icoijclp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jggrpgqb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gwdhacdu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bnhjmpqw.html


<!-- 参考信息 -->