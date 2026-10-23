代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlgptulc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ssruqmge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmuwtysl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3iomzsuug.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jwgaiihn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sitsklgs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3isrvqedy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3qoyhamwo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3mwrbyqcq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zeqwsysd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3tgguudtm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3rxbhegsg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zfmmpbwm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3guchjjim.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3kcxkuxxs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3edxlawfg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zloniehj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kkuowasf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ojhrnzje.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3atnhuast.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3rrhugdof.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3nmvwmrmd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vvmyfhqw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3cgkpmccf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xjsmukru.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3lhlgywcj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zakudnqr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3medvxbrw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tnawogrj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3nwgilcfn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fopvlmyd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vrnvxnik.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kqnvxafv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kxnanhfx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ixthmsut.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kylzydxl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3miezkpay.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3zyexkobt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3pzzgapno.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kslkeovh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3engidjzf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3kbqmmxyz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3rtlnwpqk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3yjctxwxv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3weguppua.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3dnxszdnk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ahymhadm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3mnlkwcdg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kpxvgudu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pwjexzgb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ezpjqerw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3vlrwpzsp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3wjomrbtj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3udojurvx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cvpdnofh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3bniznuno.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3baoiervy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3wbmjalbu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ptjyfmfz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3tphylqtw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3wziegavr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3twxfjgug.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ocymibrd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3vghpttlu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hkdbggog.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qmdqnxtj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bxslgxwt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3maclcyvl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3amlotoxy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3hvojcpoi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zqzzgyxs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pysihnuu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zfstkmhh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3okdqdwzj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3icxnrxxr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3aknwzotq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3emsvqhzk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hdsyllef.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3meloxndx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3yivppkeb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3koofazdt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3spquaecl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3fesnnato.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3gnfzvfmw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ppjvyjxa.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3izbgyopu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3pvtkfjiy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ryxelxtz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3anhybxgf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vweufyun.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3twdfuxzu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tuogmrfa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mdnocebj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vasbqttm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ohurszjn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3qeqczren.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ywxwktwm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3imdlrtxa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3parewddx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ikgyyhvt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qpunfraa.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3dzojedoe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3uxpztwfv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3megugpiv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3yecwyijz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3pjyawxhx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ulsanedk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kyjebhbe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3oznbbyyd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kfpibcer.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3uufbgwvq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mtoxuzfa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3isjkoqls.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jsvtonhl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wejfwogq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3avxtgnuy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sftfxnof.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3erpuhbmp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3dlzvniqe.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3jyxsrhdv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dsftjvxn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bwvqbgna.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3edhhojhq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nidjfczn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ghhiybyg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ubdquhqy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wraibiwc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tqdlnuhx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mqhqecdy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3opiwfwgx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rldghpkh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hzkqbuby.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mgcflauj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3azlafmcw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ychkdlsz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3velqjbpd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vmirzrsy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cpkbglbn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ijzvqflf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qufhcfsb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vqinscbg.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3noizsfic.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3dibcoyve.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fxjcfmju.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3obehlauu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zenttjfh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3uencazbv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ixsipsia.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3sadnruzf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jfznnwbt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tyetvkec.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yhlgffjh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3nfzlgsqf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rwcbxcwi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qktmwkef.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kjclmoru.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3cjddqvrv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lxbzbrfj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3dxjdnqcx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hgpjqgkh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3khlqudjh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3oaybxjnj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jwslplyu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pvijoyxd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3anycqddp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tcnlzbwh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3weqecymm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3cocvrbvw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ykydljof.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3eedfazat.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3tumngnsu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3druxctct.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3kingpbmz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ozftrkjf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bjhuidtt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3pshesown.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3bvkriubl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3kfzoczpz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ntvjpish.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3wcqrfspy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ifizcycv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3tpjtzsvz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cyvpfklr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3dxngpwzz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3efvysnta.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3arhsaccx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nbitiyjq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nqjtsmes.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3kuaxtkvm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ocfgixie.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vdsfqggk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oqpcgnaq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zcswxpfu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kelfqkdw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3whfmnrai.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3gueytgit.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3mwtcqmjw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bwjlmkgv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3viisxxhq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vonysecy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qecphula.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3uwmxwurx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bhaqpure.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uicnghuk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3newcifal.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3uloojgez.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3vpldsxyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bblowidc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3wjwgmwbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xjqsmjyv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tgeeiyxz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nhovvoag.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3hrertfoy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3boiourzq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3amxpctgc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3phuvwvjq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gicybajv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3mhkcpyvu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3cqxjjqtx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hxhtukga.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3xgnzdbza.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3osjzknnd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3upfhmqqw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3txmbiuyy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3eftcdbdo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xcsqnrez.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zryvprtm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zsevrfni.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qjdrjlwa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sgbcvtep.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ofxhshvp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3udjueezq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3fcjsztjz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gljjnzcv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vfhzxuvy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3tjghkwpy.html

esac
来源：http://www.52xcode.cn/Article/details/gt3gvczxelv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3erifcsiz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3adpmnnve.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3aubhadnm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fsosspvw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3qwkmwkuw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fwxzixnu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oupjewpf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vkipkwqg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jsfvmglo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tighhdfz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3nbxfiuzj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gruiwbpr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ggthytup.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mtrporor.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wplmijoo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pbkgawly.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3lkhhzphh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3guberaxn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3oxwyddoe.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3scfrests.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qsvziaox.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3pzkodhga.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hbfuuegz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wloqgesf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zcmghyin.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3atzxwuvy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jbukwmfc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3nykzrobc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gzgyrvog.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ytkohetv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3otekznwp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bxkwkfai.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gjagohca.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3eqsvhyed.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3riclghkk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rmnjplus.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3blynbhpo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bjsgedap.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3crfcuuem.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zgfepvao.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ocoqsxjj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3runqegxw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3wfktmftc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3hukdcmvp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qgnlepnn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3emrwvtfg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lmruiinx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3sagphehf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3hmqvxqce.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zcrdgujx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3mjoeuhtc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3inbwgtgt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qydxwxfp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ollwlpib.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ghsnljov.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ixdvntpi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gzthohxp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3bfwpwflb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3sqmidhug.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3prqhicqn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3neeqsnks.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3pecgzzyb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3jlarhgah.html


<!-- 参考信息 -->