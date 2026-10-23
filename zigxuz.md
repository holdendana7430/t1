代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3azzzntmu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3qbaimjga.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wskbzvup.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3rebezyak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgbdjcrb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3recfizbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzchzqtx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3qywjaxsb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3uekflvcd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cfavszlg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oxeausax.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3afyfnmsp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qmwfexak.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3aizccxhv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3erfulmjw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ginkcqua.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3phcxaxim.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3aoysickr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3rbzktebk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fgplocma.html

);
来源：http://www.52xcode.cn/Article/details/gt3shateyro.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3usqpnzmt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ynlwkxiz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3lchzgopd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3otzzyyzu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3envophda.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3faummlzq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pwnxcqnf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3yltjhgse.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3jckockqo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3szstbilz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3civuvsep.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hecgsihd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3wclwnhny.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nltyvqpi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ndunimxl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3liqhsjgg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3lgxkpqgt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mfbhtncq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wikdoomi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3fpfpbjmk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lmahpxdp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ozfqkewr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rjfuxtkt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3lscphqxc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3svgpebcf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gmbfbybo.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3miprsdyz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mnenvyzi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nkcvlvgb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eikmvbza.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3narpoxuy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3meriadas.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3nejvbatk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3vkbhzcbr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3iuvljtcx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ovzmebzv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3medfmcht.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fumyxhra.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3cvgbkwdt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3sjtzrbit.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3gixfdbzs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3mlccgtnj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ljnilmqf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ugugghyb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3knghvfdl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jcdzoagc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3vwuwvjzg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3cbywjswp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3kejbjfwr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nghixpep.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3yiaaokzs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3doztaorq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3guxekjno.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wsaskzhz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vugqbcfv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lschkasz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3xtayilnq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tbylbxwm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pgxztucc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3uublxetn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tcnkhigz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hwzgrkqp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3bzwoztcc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qfjhifyr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3gndazxfi.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3xcxnbpki.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3bujtnwch.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3sjblatbp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xfhpzrqe.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xmgugpog.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pmtlwggk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lfsewjse.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kalogelb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3cxxispsm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ztfnmyhu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3fwvpupee.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jcgywwyt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3xceipgjl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3zwindmoi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mvcfwtdm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hxbopviu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3zpxaezog.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3uvmijobk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ptgcgcyx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3rlhybwno.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vrmfrkob.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kmbfakps.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xhoadjcw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wgdfwbfn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wcwjywqs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3tkcboduy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bhfnuzqr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3miaeefox.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jlwhtarm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jyfmdehj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ggfvfowi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ybjctvnq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3teykjumq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3phgzriqp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qslotyxk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3vrdvivwl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ciwplvbl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3nxlhnyij.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gaubppel.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3flshucpv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hggdtwcg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3gmbaiktl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mdpqmctl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tbttdcvc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zldafoip.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ljzmcxsc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3afksmfvt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zjrojtvi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3shwktpap.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cuuhnyex.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3crmaggmb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3xpmhkwzm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3trgytwtm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ommwtfge.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wldsbgtw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3tvgwdkll.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eipadafc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3oyvlijsy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3byrlefar.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fodhsclr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xnqqplxg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jijdzzkf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3msnqdiyc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gpfrqvpk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ktnggzmw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3husboivd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vhicxttf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3anytrgwu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3podgbtly.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3htnrwnij.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3xwshdnty.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lbayzbtu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vercjrmp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3wbtydjip.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3kgrkwmdl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3smrilmek.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3lztuujcy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ybdxddbc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3bzwsgedn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3etiancem.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3pkkimgeu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3nnahjpbx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3dslfuvjt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3lcsdhrvv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3lmynwugm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zufweuoo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ubwlwujs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3uoqndbfr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3szxkazgw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qtyvyooo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3sehrpadl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yzjugbsj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3knymogkk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qnzmbljw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xbfmalqu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3eintcmzh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fqsasvgd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3swkimdfe.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3juzyypsj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ztbgoudg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3oeqbcxgw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jorzerto.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fwdhhmlx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zfobgsax.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qubvjeln.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sdwolcla.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3azavxvvl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nefcbhaf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bdhoyfka.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rmlxoiku.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3dguvowpe.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xrzfigzh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3wnzlbefv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mxkyvucu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3omdivsef.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3hevehvim.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ooauwqsc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kcqgpksp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ueobvgbj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3tnoluigk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yekyrmie.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mljudpkd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3noylapmq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3jpenvnoo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lrhcnfps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqlaziqo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3yczveqar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmuledaz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3uptiggpl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nkkslsdb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3sjfxhged.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3hxsiwtrv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3kwvtypik.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3bimovmah.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3yvoqckyi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ylqlgmby.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lcrqkqyo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xhaxqtlt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3wbozpnje.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ogucirsq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbnoadmd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3khiaksge.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3njczxigw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mdbsjext.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3epyeagbh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kewmhteb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nnsfhuhv.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ljwidgto.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ypxqobkw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kixqrwqn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3uqfnowdj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ykfqlrvz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sulufesp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3onunytdo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vcxbxrbs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zbonncsp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3oiqgoylq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mobhkunr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kzyiybye.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3alkhzdgi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kyxlsiyu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kxwfjzml.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qhkzyzlp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ehoasipt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oprdgeck.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mgpoqoud.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mryvofop.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3zqrufrsl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bzpkvlei.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hrisiqpu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3bsdqzyeg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3whunttyx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bufiupph.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pxzgfzww.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ausvrrjh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rzheahpr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dxjnccij.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jiyphvtt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xzgtmdfw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kjykfkrn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ygsmwcus.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ajdpmhkt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bgygfvcv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3uuulxmai.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3fbhxafho.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ebsetxrc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3tybcoveg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3gbgvliwl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ycyfvfjf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nqzpsyzp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3aguvvkot.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3erfyufrg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ndfvufkk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xnaoiumq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qrdbtawb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3haznzhrp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ldqpwjcy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3womnqvnl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3umuhotab.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3vtbevtyq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jdiyjtjc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3phnzkbxt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3oiwvaldg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ctrfsopq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3iyypfwcx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3njvplrfk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3oiqjyadw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3yqyovdun.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3mdotcfea.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3natimcru.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3sqqttlir.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3cscfewcq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3nlnpcxlm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qfhnvwxr.html


<!-- 参考信息 -->