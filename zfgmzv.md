代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wxuhfryr.html

);
来源：http://www.52xcode.cn/Article/details/gt2shxfaana.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vjkqpsbu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2mcaelatk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vthxqlav.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zspcnvmr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2eyddeltf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xtnpsyuz.html

);
来源：http://www.52xcode.cn/Article/details/gt2qkhqpggn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2agxnhyvr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2guruikeu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jmxdmunx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2muhbebjp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2vutbzwfr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2uowphmni.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2iangjmax.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2nkwhyjkr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2wqgyjmlq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yumqqyew.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2fwcidync.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jlbhbeuu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xpatmipr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ylwroxgm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vwdwpbkf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jhmqujlk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2gfnwnfpn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2udqdojyr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2oqcwidqh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2cgtanolc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ohsuimgv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jyyodwrm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gtalbegc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2gdrkqzct.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2sklsfpiv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ydjmkdkv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fnyvjqzp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2spemhrgb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2tpxirlml.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wqzqogsw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fouastyd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lysodinn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vughuncz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hqvbsrgv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rrgnksiz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2abnjcgqe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fdcjkbys.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mgxkbsns.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jtkrkufi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2knvkcijy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2pxjsvnns.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mbnxqfmg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2zvmrwlmx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2tudcsvxz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hpraaivs.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sixluqiy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2mrqsiqic.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nuwyfqzj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gbfozdqu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dlujfurw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2eqgdiqca.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aswgexqf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2gnlfdkkp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rykdntxj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rtnmjvvv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dosqhbpl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qhagcrrg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zucwnpgt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mguavojp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hnxckehz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mbmkwizu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ulpvwczl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2klyizpfs.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hdeubyui.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2fpokkbqi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2fkwageuh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cbemvfha.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2cwyufdir.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2hlteqdqw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2fqneubzw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zogrsfsl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ciretsff.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bskkiloz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2xazqldxo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ihaoazjf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2yrkrkmbc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wedqkxds.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2dlhakkyd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2uqkoixrj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fezhorga.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2srtskzwj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ibpwdglz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2btyvgoer.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ayegrvtx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gjbyuyre.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2oqbibuwc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2voblckbd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2hqdnwujp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2amvxoros.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cvqnzyrf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ixuevmxd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sxtqlafi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2uwkmjrtj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2uoeflvou.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2blwnvsfa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qpenvkoh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ihnbxqxi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ffeshprk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2cgrkozsa.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2avhbgmrb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2izctafwa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wwxceuqj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ujnulrjy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2niskzjyf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2hjhxplmd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wbdbonpw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zlxffaje.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gfyxcpnv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2yzbforxf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2krbubynw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2yorgsjvb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gdplqlcy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2tdbnfkub.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rfoakgvg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2zlfylhgo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xfyozlpg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2cvzmtkky.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jiriwemu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2txuzlhcx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xfaikses.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2eauzuedf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2symgdtxf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bahqsipc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zabzmarc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2bzywsiaw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2tllqbrzj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2omsimhyv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nytsatbq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qfglrrxr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2tosdxvsr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gjcrwgkx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2grbcaplp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ioolbxwy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2proucpaw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2hmswjypv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2skgqknpl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ulqrjmdw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hygdcrby.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2itbdgbpu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2aanipalf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2aifvwzox.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2agdiynie.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2eekfjwyu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2atldgqoo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2foohdrpw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2dhonqfsp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2myolcqxc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vgpsxrqh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2wpkhnejr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cpeurxtn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ogenuwmc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kkcyvsgm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2mjdtxfew.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2mkienelu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2luygtpwu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lsajbcws.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2olgporxj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2esxpagrj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2leymguhz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bjufnsba.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2zfdzbocf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hmwpaoeh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2krlzwzly.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gonlpeei.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nwdwqtdy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wpipylsb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gppktzja.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2aqwthnot.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tbekzmdb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dtqbtuih.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rrbxzlkz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rbigzmih.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zegwtqdi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vfhtcdly.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zerjdqmq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2pqlcuiqm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rmvvrvia.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2vtytazpq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2kwbbifvb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2efbpbspk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ztkeawtu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2vrgqrmte.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2yhtxltuh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bczflegf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2suqrxawb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2skqorisb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2esxrppvc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bqvfqeqn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ghsncmsa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2zejoilaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtaiqxhs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hlvdjigh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwovkgbp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2gtccpisp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2iiaokxrm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dmbjriyn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ujmxqmzm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lvwomhmp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2sztwqyaq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2essjawpz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2jbwhltpg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2nhumzzse.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2plriixdl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2swngwxte.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vcpsfyew.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yezzxhpg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lddeffxt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2flqzlvhz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vizutjzo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uqznaiqr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pdzbatgr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2raoaadwo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wqqylgmt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2uvphdftn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2mnpmyodq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dnyfqhzu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rcxiczrj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pwyaxktf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zjqoiylc.html

esac
来源：http://www.52xcode.cn/Article/details/gt2cxbnqtid.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycqrihyl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nabmtvdy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dqiqdyex.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vdnnrcem.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nvilpaoj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bcifujiz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wnizzoqj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yzxfokiq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mizzjtgz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2snjyomna.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2wdojrmyz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2htbdwvdx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lvygvtit.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lenidqki.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iugzuyzn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2dqzkxjtm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jgtypzgu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2kxztdnzw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ldsyrwdn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mxiuhurm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ryahkysr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2zlmapbqr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rujpacxr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2sobptfvz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yyrtkuhi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2snxjytas.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ukzhvaoc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2itdapcni.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wxbsfewo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mobljjby.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mchgfazt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ulyojbtu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ixbmcjzy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2tgpisrtp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fykmbpxj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qwitdoxu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uyqhdnmn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2eekuzkmy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vunsonam.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zilbdlff.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2znlwckio.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2efivowxv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wcgbbnix.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2dfhjqtuj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2icbrcjsn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hvoizytd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2eyiqeghr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ygfiqqnd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fptydssu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2hryiugzx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ifpbcuva.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkzqzzgn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2dumhuovu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bojuprxi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2dytrptvz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2halqmsxk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2pylisapw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2reudaeeq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2fukvqtbv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mkewcgsa.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2jrjejiqd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lrjrgdbn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2tnesijiu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2wdgeognz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jfukkign.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fzbjrdar.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2jdzhgqkk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jvnteqeh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tckzejzg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zkokxnch.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2pmqdjsdi.html


<!-- 参考信息 -->