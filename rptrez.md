代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gfvtorvm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lrvrmtgy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2byomjouz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2qpeyjwjf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mlqbzfwt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2eaaicdzi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2gctgpnvl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2jynyuzuz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vhlbzibk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2sbkmizdz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ygrbqjti.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2txmjqaqi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2hjzclehz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rhfytytu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ftnfjwmf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2cwockcxx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ozdhgqlb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ntgzzlaw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cvkrsbmy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ictbssba.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2eziqltnx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jazeocsz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fuhhlehn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rjtkuxbq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2afjfvswj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qrrauvna.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vskjnvhe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qmungkgr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2tijdkpsa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mdujmwky.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2zztmwass.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vruldkgf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pmkqvneb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xyhfknbq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gcbxyjzg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2zvlautdg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xpfdprbm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2wlldnfmw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2wrykrghr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2aqyezebt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jhduksvy.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dtmxlbpg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2igloyefq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jzurqgpp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cgqnumkv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ttboutcb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2wbjcwigm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ehjjlhxe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2lglgvkgu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rabqcoeq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bdahrsax.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2vvemfkif.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2pctddwvn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2zlqurazf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kquocfht.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ibbhjdgi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xeqqivrv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2inpniozd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qxgbyimq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qsuqbgoh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pssvoinm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gudtvjeb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rnufghbh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2evuqbdot.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rbllqzcf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qhazxbyl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ygcccciv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wfumbsob.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zfveqkdc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ygyamone.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qcynflbt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2higpnjgc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2aoehrmlm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kkmolcpe.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2utrfsjbx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mutgoufu.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2uegpvshr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rcqhkild.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dljhroat.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rivajlam.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2tjssnqes.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mhuamedd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2anmvuqwo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2yjoegmqb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dpxudkue.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2zrtobtdi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2lqvgqgqw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qqbwbsai.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ifbgezdq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2nlskcyua.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ncpoapij.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cnlkhotd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2iypnxwfh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2erymuohm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vryjxthn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2lqqctxjw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2takgthtq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jmxxdfls.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2cnxrxlkn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2arrejwbg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2gfymomzk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pcvelliz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pmhsqyrz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jydmunhd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2padjpgnu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2vevzhgrl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nolxiyil.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2tjmpksqm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bsgoaqwb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2pbmqgwss.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2upfworim.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rsznghmx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iznzglue.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2edvjiizj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cqtdxbia.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2yzvcwukk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xrzxxrtv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2mvjjdrur.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2fomkyjjr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gciqmynh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xsbmjhnb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2wambwwgg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hvtaperk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2npxaofao.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wsjxllkd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zkdsurex.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bmxevfzv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ndgqmhqz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sibrirak.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2oelsaulr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ehqfskzb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2flmrlzfk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jaymtjbp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tbspqjnu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2tsmhsuqo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2aaglvpcm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2wtjdeqtd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2yqgxabrh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wgvwkvfs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hxrgmdbz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vexjkfcv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2anyofevm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2wfseyxrf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qjrthjvq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2fqckwuvx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2htynomaq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2isplstrl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jzvknkpx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2debjfdoj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2raadgwhf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gqwpygov.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ywdxevdz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fiurcsbm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2svtdqptk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wzqwfshc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2hzxgnffm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jodtauvs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2iralqrbj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vytaiyvn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2xpyqvqmc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bvflnddm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2spvppkcm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cqiplasl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xnpqpoal.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2edgbuloo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2bxhqckpu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2tdkubmrf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fqgwvmgs.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pskmvqmz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2lrytoxdk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ryatdbci.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qfjyuvpm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vjooqeit.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aqpmjhos.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yieyzacv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bwwfqeun.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2wxdyzemo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zpsfajog.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uilmwezg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwtczidb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hwyrlvmn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cbmxajva.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2oqasvqpz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ohiavutc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2onrmfcnv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xdyhpwdg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2oyuzzvul.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2yolpbwls.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ohxmlghi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zrkeybww.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dlfaxyvd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lvasegrf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2nvkfpime.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2arvrtexk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2etvzdrea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpkowspw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2htrglhmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awyzuhiu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ligbfiem.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lugeetnd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qzjaecxs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2spogpynq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2odbzesvd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2tombiwmz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2swykgpyc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2kblqmvzy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jaeqcvzu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zrekqkwa.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fivitdxa.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2uvcuzzwy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwzvfyku.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2cjbazplq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2dnxiyced.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jtyvfkcv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wvsjdgha.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bijqzxot.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sjpktrst.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2anhlmvgc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tmjpxeze.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fzdpxxze.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mzdzasme.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ucqleemt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pswgktxt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2svpgmnww.html

esac
来源：http://www.52xcode.cn/Article/details/gt2nelhgutc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wskbobdh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eslxvmwf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ywwwfimj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gihkgelc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2salecyct.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gwwexnfb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lnwxwbsk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ewoohmpn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2azcfyvkr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2woctvrxq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2tjqdqiiq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vkvdxjun.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2irsexubg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2rtoiwvxq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wpzuziiv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2pnkrdhba.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2dypwvqxm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2uoqpluia.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oaeqnvxy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xizrxdee.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fyvwpbcl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uapjktvs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dzmivtiz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2lzflooci.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2skdmzfhg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bpeomphv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vsnfiyxt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2juvzzkaz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2iydbgvhj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2oabehczu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2mvrgohhj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2hbxcckak.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ccrspyeh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2khzfwzef.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bckvrodq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2fgtwozko.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bbxipwcu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mnfdqwtg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ybhmkkiy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jgkxeesh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2mkjdlbfh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ylgvygii.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pitsurwi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2mxanactp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tuozcfoq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gamgdwop.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2otmiuwko.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qmcwwitt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mnqbttad.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2iizyhnac.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2upfqinog.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbzsoui.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ldpshkhc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2diipihtr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2jflfwtiu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rjhnzdby.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2pvtdoryf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hrognbcs.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2mjpybnea.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rtgvctik.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2agqazowf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ptjvuhlp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2tlnzjehz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jpsvbddy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2dhbeukqg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fxodohmv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ltegftsu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xxbevwph.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2zscuykzv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2msntpisk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2cxcuasim.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rjexrtgy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qzadxdjh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2agyxuvvc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zrjjhkbk.html


<!-- 参考信息 -->