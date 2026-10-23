代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtrrvskm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3higexccp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uscncvys.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mpsxhnwe.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hiqbdmxn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3kejgkqld.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qbjovhku.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ablusdyx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3rakzshyg.html

);
来源：http://www.52xcode.cn/Article/details/gt3xcoabqic.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3bmeoapux.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jniodjxk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nobysrum.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uxilhaqx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3abbrbxpi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ynhttszt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3uatftuox.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3cmsqukoc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3clnyxoos.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3rrkvvsle.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3sfkinyxl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3mohezzdy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3mhyjztvv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3rmwmsjty.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3fjrackvo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3uobukzyp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xqkxlhlk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3jjkiyllf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gsvgwewo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3cyypuudc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ghzsnwnd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3rrvlgldo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qpcnpawb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3svmhisqb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3upvdtfpy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3snazoziu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xemttgpj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gbnnuucc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3jfzwpdob.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qdgtxbko.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3szisvtut.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3loauezjh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xzsevjwr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3mimozxqf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rwcddsmy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3wuirgmns.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bnzanmme.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3mvrsnryp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fcwazozy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iaddwktr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3eswntvku.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3irdhqwpq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3myxyirwu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fjyndezt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wnfmlqeq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gkyzonoq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gumpxjvk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3yohmvgdq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3atydmzxd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3eyttaatl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3axgvpwco.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bfgasexx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fhfuwhii.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3nkirvzsj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3fjyckrtm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ogpkympl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yswwqqpy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3rtsmsidk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nncoqaug.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3zhlmwoai.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3anmilogr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uxqqmmcy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oplfnkqq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3swwosbdy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pqsxmydp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3burtozra.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qtnxzjjf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uqpmmyne.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aqhgadfy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qmvcljsv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3dnfirece.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3juxehjue.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3prxtsslo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3djqbmjhw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xygsnatl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fprqwlwt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3junpvdcf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qoumsrdz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ymistxgd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fegwflhz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3lnibxnde.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cvcsmdjb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3lhrejjpu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gaiubwwh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3apvfzepp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3abycqsby.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wcimfefa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3byfvfnns.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tbkmxbzw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3pkzcptap.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qqfwavga.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3zefvraxo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3udbjvfff.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ggfdaudo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3skzdbmot.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wovhajof.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pjjqdwwi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zrjtuifw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qbnqotvq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fmailvvb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3whponwao.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xiqgtfjs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3egeaccby.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xhxqrbfy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3nsfaenmz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3prxzvlsy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qypfqjbs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dlgfuydb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jnfpgeqr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bdeavouh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iwqrrwts.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3yefporde.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ucwupnep.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3syrouvpn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3joowmhfy.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3zjfuqzsj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gnnubdxi.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ofkesvzy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hzwjyktt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cssmmsnt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3bfvpkjji.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3laamrmcl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xxbwnoja.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3pdwgeeqv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wtipxavv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ffyypijt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jwjtjinh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ujrfnahf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3paonfhvq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3erweoknj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qircqpje.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3yragnfwz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3swptaatc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3txnusxew.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fisgmfmk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dljlhvid.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3unlhyejp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3icpadprj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qcwiiiix.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3owuhmwpq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3dsgzuywp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3rpubtldg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3woglwfwp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3bemsygiv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vtipyqzg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3vojlakfh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3szwkguzo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3bksrjjdw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ixndkdga.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3cfjlboed.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fjelaysu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3xqwofxzk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3myghkjrk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jcbdkuaf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ggeatkhx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hufwajkb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dzxxylle.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3jexxbhwz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3psmnxqyv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xphcsitt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3wauruoeh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3kamfuxxn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3cmtxpolj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fbvdojas.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zwqebsfk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3lthngkqe.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3bjdqpyow.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3omoipnpc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ojwgccjt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3rbohiusr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3jkwsilus.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vxynlrym.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jsbfrfxi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3zimoyvxj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vzpebrfb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dwdztyks.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jqzikkio.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zzudwrqa.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3waandlnd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gsisedrx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3czihhmfu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lzshybnm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3hjgrbkrz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rcboeixq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3vosppndo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fgyfssbv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3utnwrxoe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3iagvnoet.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3khnmitig.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hyaftonj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3mzvnerti.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ggruucwp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hotyzpoh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wyzjfjah.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cecryxot.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3uzvsvemc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3cahkbwfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atdxherl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3fgoamvpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohggxpfg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3mlzhedzw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3edhywfbq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3grrmrbza.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nvhweprw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3wjxhzdva.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cewdlcis.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3qecaymhb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3euwbasjs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hqifcenx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ghutevwq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ymyfyfuj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jtqbbktv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixpolokn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3liaovtku.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3eqdpzggg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lghesjjq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wxalbesa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3upzkfleu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3kpcfeahs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3maokvsgp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ewvgxhhz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zlclqbus.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3toxqbrfz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3palzrvfq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mrfsetit.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hptxlfgr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zshrsfor.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3pepgzrxh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jfqdfypq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bclwkxvy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jfxwxtre.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3qqvtljvv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kavjsjff.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzvubalj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qatacqom.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tkexawvb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hegnfasi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3arfynldw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3chnnjgih.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fxfthzod.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3xjoauvkm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tlzsolle.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tepyfgyl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qgnwftsu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rdowaago.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fwattfat.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3srvzfhxd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yywnpxyc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3phgquvcz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yugnzfbl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bknglqzh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nzcehgpi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlrijjtt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rcruthou.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ltjufzcz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qrupoerz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gfsloujf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lwtjrbkl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3retcdxlv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3irnmgbsp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bazyzvzv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rwbzdidx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3aunuabbd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ngvjgclo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kybtjdpo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kjlytioo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwmcggwm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ockuxoef.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3sqwguzhw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qstfxxes.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lyhyufpk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ranilpmd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ytngdtqp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ookhkrjb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3bikbxnna.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zuzcqjis.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3aesveeqf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3sbwxpkau.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3uynpkwab.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3iocautrs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ihuaubdi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3icenohyd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ukbsiibb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3yqwszoky.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3bbgcjwsd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3gllwhupg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rzlbveua.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3tjzpxhyy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3opwpdccv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3aspimefk.html


<!-- 参考信息 -->