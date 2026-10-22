代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phftiocq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2sowezkzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atslqmpf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2twcqnwbd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ncrkmxvd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bjbvfvst.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2taigocqo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2xdrgivkc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2xhzonxuy.html

);
来源：http://www.52xcode.cn/Article/details/gt2pawkhjrz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xlulmufv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ewbtcciu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pxeeobey.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nzzcswcl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2isgojooo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gsfcafkp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wefwvlhp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hyrjfpxr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ggjesahq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2fotekyxs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2jsfrilkz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2laovotti.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qfwiefzy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ebqonrkf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kqpsfacx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2zhdvtywi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ahuhqltd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zsszvqiy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2npegipiq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ebrepnrs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nncahkrk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2rgxkanug.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fuplbtyk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2rxnbzymq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uojrorlf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2othkoaop.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2khxqgjqc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2pahlgrqg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ldifrrlf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nkmojike.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2dmykocqc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2kkzohqng.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2fdnjuaku.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2sdbudmvn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2scyvpwbw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ayxoxkyc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2baiygriv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xjobitnz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cgrpbimu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2utyajyhm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rjajjnyr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2zmfclkpv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2rrgcjkri.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2gcfsbobb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mzjbgmtp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2jzdvzkyh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2krqvxsyn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2setiohdb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2bwjevmsk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2btzvbmzq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pgznhkhs.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xktspuyu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yiugedct.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2eolhcnyw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2aqslfaxn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xtuutbpi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mqasdbpp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ycfwbdak.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qpphghkl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2apwnqxce.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bewhtsvp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mmpqklez.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kxldppte.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2jdncolkd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dhibgscg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2evjekqpk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cdvkpaht.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gbxvkisx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tbrmvqed.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kawhjjhg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2mvavwuzp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hwqkdfwx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ououlnjf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2bdtehfhs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2yiwvmghe.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kxwlfhaw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ifnbckau.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jwugodws.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2wvnogezj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2sryokrsk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ztremomd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hzrrvvbc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hribldqc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hoiwkpuw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zwmywwxv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2dymnausg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2acriruha.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2myvwbglj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jaymfgiv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tvokbdcs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2axxhufjx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gsvktyrd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2vyfombxp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2yvfgosar.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bxqvilgz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2melbzbrc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zinqqpco.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kjwvptro.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wpmcyezp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2bvheymmm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2hsvemosd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2iyvndiio.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dfiovtjy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2awocrqlf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2banlvgpr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2duhxkgvi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tkuzslvp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2mpjbrwcs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2vfhjgjsn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ctfduibz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yqijpowr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2fgziypxq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zefauasu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zfjpksdx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2chjgzbbl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2klpcjgql.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2epfsnqyj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2hhmscyew.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2sqtrqoxb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rekoguej.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2gfijvulf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2etnmztej.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dayjimka.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tdhefyid.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wmdeocsg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2jmtrhbuf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gdlynklm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2offedyfz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rooagrjw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ovxjisjx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wjfntjru.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2gpdrusfl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2lwkvyedi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zcvtnmwq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nnhegmiz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nvyrgxao.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dzyiltwu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yzifklxz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2qqkbdbpw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2prsxrbhd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gifttfff.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2joniapva.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2pkgvgpcd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ucbwpzvg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2pbidylef.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2cpvqligb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2beytgyze.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2fofpuklm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ylgcdyaq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wtvtrrvx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2knkzmazw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2cxzkewzl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kqgzswvp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kyfrquby.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zejmadnj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yrunifvn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ptmkkgkd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qxsenbbt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uezdnjai.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ieobeifa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ooukbhhp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2tvlqbuox.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zsoqokzp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rojyqjwi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vpygowdw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xbssoxvt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2jmvouekh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yifgjunc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2crxahxyx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2necvkxrn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cmbxmdwp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ypuhcomc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2omanueez.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jgihihbk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dkwkkrtp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tkynqfjo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jtxrxgsm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hcsinxrv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2jcjdciqy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjekxppp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ayvwhhmp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vwbxqzio.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2tvetlahh.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fdtijntc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2qxtnrgsi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qtpythlv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2bfjpzljk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ewoawyex.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2fbgvcdzr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2sljdttsf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2yxrinhgr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2zmvdpmqh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fnryqozh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2hrohcsvl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ivfpsgzx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dfebvtpd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2phyilped.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwlufvke.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rcyktdbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsknvaip.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jrcfozot.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pjwykhjq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2yassjyvo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ojrerdtp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gzdhjkpl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2inswrlue.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2dxtawhbv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2edpaocpr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2blrbdwin.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2waptjsna.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bpwnwsiq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2emwcfmoj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kvnlrgmc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2cavslnls.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hkoufzzc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2iosmwdcq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uxqllnay.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jozrhdxt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tupxyrht.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vgeipush.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2evzofwgl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jetijuhq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qfqegnvu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2dwfmpieu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2qttuhhlj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vpqkfbkk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2knrevvph.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2pfuihamw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2tfwpfwyj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nobzrkeu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ukgejvps.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bcduufut.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rierkftd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2entcelhl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hakcvzdi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2dqjyzkhc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fimdjtiz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2jiyghtuv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lcprkuun.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2numgsxge.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ytxakwgb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2axfbxzny.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yowypnsv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wlcmpept.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zxnposjr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2doubbfwd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2njpceaqf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2avkjschg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2crgjecaz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jgfrccty.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2znnvzmbt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kcizgggp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2fjblhyeu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kzffqgaa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ijwqwzfu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2obkdkqkg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xzhgkphc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2yteoorat.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ihlleryi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2yhzmaawo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2shxfhuyl.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mwmugusj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2cyhbjkra.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2fxjvjvaz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cewaycdh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qysljqth.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2fdvtskzw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2fjiqetul.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2egkdnfug.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2tcxzduwg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ygcjtvww.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2saqrqjzf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tajivxbh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2imjejvud.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qqtmfkvb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2eoytijhm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hdcudsxs.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2yvytcmru.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tinukads.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vqhzrget.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2dhswflvn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lzbbirlu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2meoqsljw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2kyftdiur.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ktmdpnrk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mkcwzztg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qbohrbht.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2gawtnwxb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ivyiicyq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2pwvqwpqu.html


<!-- 参考信息 -->