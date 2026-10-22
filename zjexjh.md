代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qjtsstue.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bfhigasd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2duibyhig.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2jtygoqjs.html

);
来源：http://www.52xcode.cn/Article/details/gt2igbrcdvo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2swbrpxnk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2hmquxdwm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2toshxotd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2edsuvsuv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2fhlipqgo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2zujcdvrj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2gaxukqde.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mcbhcfoy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qfepsxsx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jhxmgvpv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2tohocdhk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2paieqorg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2bzwmeujr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vwyeicjn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zyvzwjlr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2judgpxuh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2atgxwlka.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ljxdapwd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2pdkiywdc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dvwydnmo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2metvvqio.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2nqlylsti.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gcxqlivv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2kqwipbtt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2velxvqiz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ketuluut.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vozyhvxj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vaizmtvt.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zqacekau.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fmgqjqju.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ohlenqng.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2hctpsyqx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mfrqdrcz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rstfpaqu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bbwosvzl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qxnitqib.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dicwfpyk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2acktezlc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2zlkcbuak.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2voyviuaf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2clljaqpc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nryiirve.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2swwhdtqg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2upssnisg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2utkfthdx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dowoqxlc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rbhcxlra.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2holyfgst.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2nplsufmy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bbrzoxwy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2uknxbgnt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mbxqszrb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qdjzrddd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ublllyec.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tjbvigmn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bysmlpit.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2daoclyqv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oyseewyc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rocqmlkd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2skuzckmg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hrwiyktz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2irmegnqu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2bejmviho.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hgefyssq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ziktspvf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vgwkmked.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zpnztaue.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2sxptkzli.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ijjotoil.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2yacsjvaq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lohgkfor.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2njztspok.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vlqlpmij.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2fqsttikn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2juvruqvl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qosigakb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nadrcilh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qiewfbdk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2pewqblvl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nlboostp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ytztlfcp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xtnibnir.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tpyocuyb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2nvxuvort.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fljynnre.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yoouvrqp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ocdffthe.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2zcnraxzr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2fyhsyshf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wgzzqvpf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ocgwdoio.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2riueuvzx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2gfsrffia.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2oinlvjtx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lktjbspb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gsxrknhr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eihosbrh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gmtnideo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2bgxfrirg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jzbwcenv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lmyorpqd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cqohoujd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2bjyegdju.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bdjtulkz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2hekzrtbp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2eabpyuyl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wecrmyfj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2xzfhzpdr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xjcgpvmd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xvewkrtc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nwgeaezk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xcffsulc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qjiiuqlc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ulvhtplm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cacawrdz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2joxsydgh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2abomnmka.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gokkkowd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vhcqpeky.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qsfiehkx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xfpkdirm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ibeawnog.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xzncfzvj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2trodsmvg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2govuugjz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2bjcuufcv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2anebgzzc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2kivnyhzf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uwptikzx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2iqyezwla.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cdsgbitp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2orylixer.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2juyptqaa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2dbcuceaa.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2xcybycst.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2aflvisvj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qhoufpwh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rldjdrqy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ilofkswt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kimlkpau.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2oijezsub.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ejolvcgo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nkxvemtx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kkzknplx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2wlmxzvle.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jposutxb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2aestqyyb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2hokvwuyw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vpxvinvd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2nwhbcvsy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2grxlllwq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wfdueint.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2friljpzc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2zhvwtdkg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yhznmdsl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ocqwdbeh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jzisiuey.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ixtahbld.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ygktpxmc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2otlbavma.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ejjlejzd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2yjlyyyuq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zphuhklz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xewoonkp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2gnxechez.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rxiaercj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ljbjgvsn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2kzodijmi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eaxckhck.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zcnwfizq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yuoiqhgu.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mhcbmciw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2njiqkkcf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uwxyxwzb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dgghdydv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2wuwddgsq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mupszerf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2eekhgdix.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lzpbsjos.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2sedkzvam.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xnnvdlkq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cqatebts.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qozqdifo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2nfeasplc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2szjnfwnw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2epfetkhv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lthkojcp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2rdoqlimr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2cjulsrtp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xhajjdaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2neisbbdu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2szmsxyid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irgpuucx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2taxnbavx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2iirvggod.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xeevvete.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2fkrquili.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jjuhffmc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ghsqrmfu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2teocmyvw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ltfuyznk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2bujwyvla.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pztnxvak.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gighhrhx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2unpptmon.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2srvkskid.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmpjonwp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qevuzybd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2cisdqvgo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ppjjhdna.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2aeojrcwg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xbgrujof.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ttluxlxj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2pdpzgizx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lrnngbrb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2dplgjkuo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kaxdquht.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rhewjobo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2larqjlyj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2fugxkagd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrrofovh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gvnsxbzo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nvytetjs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ybnscybo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pkkualth.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lmdbgwxs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lvbidlta.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hpgkudbm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xhjznche.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wwqzraew.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2afhvxmuy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bttdgzfw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2tfzitudl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bozrsudd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2annqjrke.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2pibmlkwe.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qmridnrt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2duwsaqac.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bqgwjquu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gzmwgjcx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2iljhoaer.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2iiintspa.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ukaatemn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2eotjorxe.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hiljopmo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nhqpddsu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2irihirzs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wftuisrl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2myeajpku.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2uyqwemro.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vbbhfvfc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vyktslan.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ovcerxxi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2aweances.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qusxsmeb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2oxjrxcys.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bqwmsuil.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fwwxxhgk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hpgxgfuc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2gbnnsrhs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2esyovruf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kwasnjqz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2mwmootwd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dzrlnaqr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rmqtlvkj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2owtllnpb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2dmkcimph.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2oyapelog.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ydxyftdx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2myplvecu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2obnctock.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2jkzuchdz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2epofibom.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jaqbgefc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2alqpillt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lqiygomb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2yeqfasvl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2nzjabagy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2bkauhhok.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qfybmpoz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hfbapxyc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ctwlrfgl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ranfxwng.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ingymrbs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2pteggmjw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2brjrczfc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vcfkrets.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zxikylij.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2nglpptiv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kgoeipym.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zobqmted.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vgwixalw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bjrvfhlp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bsjdqxhw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2usoveygj.html


<!-- 参考信息 -->