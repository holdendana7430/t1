代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3enwnfvzh.html

);
来源：http://www.52xcode.cn/Article/details/gt3hchxownj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ofmfoxue.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3vbdvbddx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pngfwyvy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tznjoimg.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hcowysyb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ckccwinf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lmyxezwb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3lqpgxsnw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vjyrbbjo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ycexvluw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3sspytecy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rgnvxwgu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3bohpgrhy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3mntqeiek.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jefnhatg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jrzckhql.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3jfixtqwy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ikfgzpoq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3twwiqvlp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3iqgknivl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jyvocwhj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3verhegct.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zfdhvwwv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3parksanc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3czltbusp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3snyexiwk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3vfuimazu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ihgqhpvs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qvavbqqz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gocwvrxl.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3inilpxrh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3tepjigzj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3rmaufrzx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ittbhqya.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ijjqzkjn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jcifnqmv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jwzdppbr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jzeggfrn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mgchjbuu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qsrpyqiu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qoeauukm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jtwqfzjf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3yvvbugmu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rwnmefjq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gjofogmr.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uiulcpty.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3awlxnwbl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3jotqmeij.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3tzmlgicw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3bokjssnq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3qezakvwf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ctsigemj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nilvyizl.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xnncswmn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3sbtghmsv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3pkgyncoi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3amlaywcq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3igeecgns.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kvgfdosl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fuaforvf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gebpygjq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nkgxxkol.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wmwzsaou.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zbkvhzfr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jcohvmgc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3crurqkfq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dmzuzsxn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3suhsejla.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3doaeawtg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3sjjgwres.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3avuvhsxh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3kgorlrwn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3dhdlfagh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qttgkkpn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3nerjmqok.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qmmagjgr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3fpytmkug.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3leyexidu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bzzipbqv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kpsvdfuj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3fkxsvtvp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rujzcgun.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ovraetbh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3bxzqhwbv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3sepmcqcw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mfozmqzy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pdwennyg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3imjdjiml.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3lvozvzfs.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ausxkipn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3uwdtmoxf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3rthvjhie.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vtwfszkm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3huteppom.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hynqojus.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3mbktmusn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vxrwntey.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xmvnfoum.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cfpuitzz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3waiaqwli.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qqilhbzv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3aoyrfyik.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3rplutkfx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kiaylepm.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3oxfknkxt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jwuwcrom.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nkzpqtkd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wddnuuyr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3melkutyv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3giitzspp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3sqgdpbzs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3mjjhamdg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ckckpzju.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qeytlzta.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nemmnydq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wnakttmc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nkuenljh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ylqiudns.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lpuypqog.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3defnsoid.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3pgtszpdx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ggffgrie.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pkeaqjts.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3tfqsdlqr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qiyoedmv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rxauevjp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kqgxzxld.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3tfczbtwm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xrbqzwas.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gkppidap.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zvgohsml.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wowzwtkt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3iwfzgrfm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wnqzmbkc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3tbgvmjop.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3grakepnc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3mgehpdvu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dpbmonwl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3lklnzjag.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3sujvnjpg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ibwnogws.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3hspgwlau.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bnprplko.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3eikzmfcn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3awdmjkau.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ivjqymhw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zfvfcwgc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jxusanbj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3mdwgtiyp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3oetaujdr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3rbrpbnwx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3iggmurjm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xcenfwpn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bgrhspfs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3kmaabyqn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nwntwgyi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nxynjazb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3cwymyiwz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mpvvygjk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ateltrlw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jektymlf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3buuhqoym.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3dcszuods.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mpymrzzy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pjriqott.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rfopjwov.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3feylxscs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3lihwyoqr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3kjchnkcj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3jlhqwyku.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3subaojjv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qqstitzh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wajxdzqm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3wwrekeaa.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kqngruaf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3itzfytzg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yopsngbd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vuapimtx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ecmfhiwc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xtlrbczu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yeqoilbu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3myxgedra.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ufdzzkok.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ecqtebwa.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3poxusflq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zvycrvim.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pjplzegf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ifkxwacu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3zrxhvsht.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3rjwdfdtz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qgtcalck.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ahrykxix.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ggyzngbu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3wibpenoo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3agxzbzgc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dpsjkyjo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hyuynmxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjszljbe.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vjmahifb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yduxtpaz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3euxmgcvp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tgtlctvl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3anfthjvr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ygercjag.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ksaestwf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3dquvsfmf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3knwtcvqr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lldfalsq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mjfjjzrr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tcwxetlw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ritjgftn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zcvvebmi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkxhoonl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3nolvvxub.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3imxkfumq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dmxjuygq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sfyhyvzk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ruanhpso.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3hixwvabh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3exvrklcb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3whocidsa.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ogbjwwqa.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zfhlfnjh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3rklyvraz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3tphpyfqj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3thccsaik.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vhywfmhc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vvzqgmcc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tfuexxhb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qymutkpk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gyukdihd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3tgaaaftb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fteyvytf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ipcetyoj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hltdbauz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3acghpwox.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ggzdocdv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3kgzyoscy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3adtrewvf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tlrarfxr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pfsnfdig.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qffpiwqt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3firwaope.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wxmetoyc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xqcciomg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dgsnqdgm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3sxgsnwwu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fzvzytmn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3cbcoarfk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wvvfifnl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rnftoaca.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ajuzilzi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mvrvjmmu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3zhfxebly.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dnbwkaze.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3unfhtkeq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zqnrzzjy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pitamvnt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3sdqfygme.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3uacfmvgg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bmmkeuuy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wbgmjaqa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jtdquloi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gkylfwce.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wlmkqbzp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3pzowherl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkiqupcf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3bgdbotks.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxyikmiq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3clodlsvo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3wmdpmrdc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hpqqlrck.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3oszikdue.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3alwrowbi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3agjxozdi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3imidevfx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pppdmotf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hgmeqxoc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tfljwljv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vgdydjjg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3sfditbyd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3sdkcaytg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ucifjeiq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3cltfmpza.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3epxivjoj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3dhtnzvjg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wgyhmxtk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qshjlsnf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3perykuxy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3tjzzxtjp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3bknqdxqb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vkdnlnxv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lsivgcut.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3oshkkvuf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3daxzwiii.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lgpcblfh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3aswwehbh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ccsvmmod.html


<!-- 参考信息 -->