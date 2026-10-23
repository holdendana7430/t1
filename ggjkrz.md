代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nuilmxuy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wpspkvwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nyplcrqz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3sqyjdkzi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3kqdhrnsx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ewngckzm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dtalntir.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3tyyfltqz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lrcvhvqs.html

);
来源：http://www.52xcode.cn/Article/details/gt3jkjqwaga.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3uiguimxl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3hrippvyv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tnifecvq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3frhnsbpo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3inycuiui.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ujchvdux.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vweabknl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ohohkcqg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ackmjjjk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vwawhuds.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dnumaehg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3leiatzsg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lrfgmqtd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3xehnvwja.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3samuvahz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3viaelvil.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hygnmyjd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ueuwbclo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pmtxcsiq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3rtysixno.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3egxutuxo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3idggfala.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3copxrctq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3rhfvflzw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mohbvscz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3waoesbks.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3giksaygd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fmzgowgo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3epvgxmge.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mwjktfjw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wykhcxkf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qltgvdxz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ggvsxtaz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3bvwzbmle.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bwcihibx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ahjdudba.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3otnanyrn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3uauspnzl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vmfwrgfu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3plzoxbtm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3aecrdgjq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3avhvsnzh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vxavjgym.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3czlxsfby.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3pgqsnnkx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wmomlaie.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3vldhgchm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3pwbukrrp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3iqayphhb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vuvkheli.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3kflkewpg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pywiinot.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ecjuanzc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3iozmcmow.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3fwzouafp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vknyqajt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vmqorchs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vmjcjabf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aijvxsis.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3pagadovy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nssiznmr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hfunydmq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uspszwkl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qnxcbmuf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ooyiafst.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3pavdbqyf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3utnfawvk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fvadytsu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fglvpgoi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3enaleqzj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ryyulnvb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3icpdxvrd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3odwidswa.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3edsnozfu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3uzpghkqi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mpcvsldz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jxzjtgrk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jtycwqfg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3huslhhmj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qxiniqha.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3xzwenmtb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3thkaeerc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3yvzyoxdp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3spaojtvt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3obbqoexl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3izswmfko.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3plubblvz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zrsxplkl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hxaysqas.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3erdvftmu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ikeaydpp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3sxagjius.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3faxhuxzm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3haphqaqu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3oxhlzylc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wsnnoans.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jkaxzfaz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3modnkxyb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zcxpogaw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3xvdwvthz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zxbbyjgh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mwmjsjan.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3cdddmnuc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qsxbbjei.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ysfeutgr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3tbxvkaxl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rrxsejfj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3eaoriktx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tmeziwrf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3liucoigf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mxoezknb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3frptwhja.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3twcxzrjs.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3byufivez.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oddovxma.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3qzeyvqoy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iphcglrf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rwtnbjfe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vxrkxxja.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3jkohkwse.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3uzoqehvj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3mbdcneud.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gklrelfc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rgmqrbsy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3tpyomrsj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3sqvlyfwc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kshwevey.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3dtosasvh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iodbowue.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3cunieanh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cfpccjyd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3hpsmfxcp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3qucuslom.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wpgyausa.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3vggpogfp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ogmqxgbx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nbvtgueu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3etsgmfdn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ncuycjym.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3oletclrr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3nnequbpv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3flrmomvt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3raswtkjp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3lhjnvhjq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3nmsjwlms.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3kxvdjzuw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3fwtmugdh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vlnrzzem.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3smpzmahr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rzxbibix.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uhhcitzp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rcbtgfcg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3cztooszn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3klwqioyj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3bkkvppzt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3uozvciic.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zejpsqym.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3tnlccswh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vkynukpp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3mpleetwr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3asakaqbt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3onygluyd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bgllshea.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aeldruri.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wdqgmikg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3injepqds.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3todglryw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qkmcetvc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3czqdtupx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3pmljyaba.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3yqxblumw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3pbgubkas.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rbanmgkx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3pokyyqwz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rwphtbos.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tyzipixn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gfevxlps.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gkfdavey.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3cuoucqby.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rypybkhy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cdrnkduw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3czcljbcw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3kxmqwtxz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tqashnxz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3mamxtcgx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zlwnbrlq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3skbczjqh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3tmjzbyta.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qcceqhag.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wfsvuygi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3npiwqgbb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bpyfticr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kqsnvkjj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fhfenjmj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3koouajxw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3lncmnlts.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hmvauohq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knnrmqji.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nyytmntu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjszpkoq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3stmokwzq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3bjywpvka.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xvstbjjy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3hvevtkoo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3gghphfst.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ppwpczif.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3msmxwgkw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3jbroqoyp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ocnupxet.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3sxmfohvm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3dtiumrne.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jsnxprcu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymrtqtsu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xajofyoq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3geazpdfm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dddvbbnt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3npbkadtr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gwexextu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3roruwfqh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eufodixx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gqvyflrv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rcrgnqpk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3aiegjomy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rjfvtbhe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jvjwpqnj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vlqnfgon.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vpxjvbyw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hiysckxk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tujvmtnt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zljpdabf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qxztcxzs.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3gwrvswyw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bdfhayph.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3djtneudl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jmxjrzjs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3snusback.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fmbzjuuq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3axzgehcl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3prmmhzxl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vugimrmd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xnsylhly.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dxzbkheh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zhnnbdfe.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3weezafdy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dcxgtpmg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lzynmqyu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3laxvvtdr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fdkmgfnh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3eblhbave.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zrbrgsle.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3uyrraajd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yvnopdsk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xtefrfgu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ooaznqvd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jqyoqzza.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cgqrwpmm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mpatrqhb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3qfikwenz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fnokpyxq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3isljbraq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ovlgeguq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kehcvcbt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3itpyqwsq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kdxvaate.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ggbhokvg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wcxrzgyb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlxstiyg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3jezquanp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rfemlizt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qxwaobsc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3jfqfmxya.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3loyrwhem.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xawvrnpo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mrztygfc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gbqfphaz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3otlzkzjq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fmkcqlbz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ubkngsit.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ndvgelgh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ixyhzins.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3xbmlaaei.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3urdfqdys.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kanshkvi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3siqyyknr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3cdtwkanj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3yiznojmj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wjnkcnes.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3eerdlabt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3rvbuuvcq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vgtdhaav.html


<!-- 参考信息 -->