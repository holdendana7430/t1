代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3feeoafpo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hwcewegp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nmgbezdy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3tlsstene.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bsunnqtu.html

);
来源：http://www.52xcode.cn/Article/details/gt3aiotcgdo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kawlrrka.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ruqpbuem.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tyluzyoa.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pdrcfjne.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3zhxpygof.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qhqnyglj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3covirvhi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3noysazgn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3wokekubg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3dacfugpa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jfvtcpns.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3eyikujcj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xuzauxke.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3osnnjhjs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3zbfeiwzg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3zlyqrqpr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mrpntlnq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jxdpuuht.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yhyjplgz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3isalnlhx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ykjvfdkq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3nymrfnzw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kapvlgwz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mcueywsg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3stoqdrrs.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3scpildhp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3douwlxkt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lcvhmjit.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kgbpmwdx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bhozklle.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qlqjbxzl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3yphswoio.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3nqbjedcg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3hxarvjbv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ttpbqwjr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gtuzspdn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3prmnfzje.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3qvhdbjdy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wrlymdrh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gnzocsvh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nigllyyx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3yivpybds.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3umynjzee.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wcdbxudk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3wieiqcqi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3wxgfkicw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jdjxtwnj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3pupyjemw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3bulxymce.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3aenxtemx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3tyvjrtjb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3qhbovcjb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ksajzvsk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zkmweldj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3cmrhnhzf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ssuwhdnb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jkvtlhzd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3javtxzwm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pdhoolhp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3waskrmyl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dvavsftd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qkekgpxp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cddgzwnr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kkcawfyj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jjbfzoqg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3llulqgex.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3acgkunup.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3shltirlf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xbdqxisd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3pdlwsqwq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fesnfxnf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3dflladnr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3puqwkirz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3csycinny.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3qllffnzl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pnudtwul.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nvgpqrfc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ncmlrspe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3rlbgypxy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nbetcmlz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3optflxmt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3pwsopysa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ikgpmocx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cwxkuolr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3kzccmddx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3xygxllwa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3khxisklr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bkatkfnz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3optcreng.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qssjdjgx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3pygfiles.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3dgxhngwo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3saeeehsh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tsyxkzqz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3aabtoqxo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mtuslmrz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3oxuwwicv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kspgokhx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zvxumtdw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3wpumqxoj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ysesqfzz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tsygjcef.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3sfxcpbqd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ltnxqfip.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tvvbfjti.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hbztqxsw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eprjtoez.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3rwkoglmc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jarxbppb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3tbooschs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3btqczkao.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nrqfvxvj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wifdbwwa.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3unrhciyr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fsbmseez.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3sgdyokmj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wimgbubg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zaucwhdq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3karpkjrd.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3xacsmjuk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bnjpskop.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vscecsbt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hijhzicp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3opvbfxac.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mbfotewo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rzouanpr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kteopyht.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hvcvtafy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zoudadkg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3rfqhvzjg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3loiaxinj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kltbucyj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zbanxqmn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tncdvftr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3uznevenu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jqkfbkpo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xyvaafvm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ntcbuwwp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3snfmdsxe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3afscynzx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3agazhvxs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3bqguyvny.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wuouutbl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3eauyxhvu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3cyqchfel.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3croibihx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3fuykuzmd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3rwzovhxf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3rhsfzswu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kcrecgah.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lqrxapaj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3uvpukdlu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nwaempcc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3txbxhcli.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3igptwxcp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3oqyimfhf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nywsuihj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3lovpxtor.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ivvmbdhk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3bcgdkksm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dsyvhdos.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3zpueefaj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3emljslbl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ipuimuin.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pwsmqjjo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xvrvhzfn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3iqrpzjki.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rsrzulsj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3mjjfmzap.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3umzwrczv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3adwxbhpw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3zphnqlqe.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tkjdeudg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3eoiteksg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3fnbsedzl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bpvvjxfd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fmomnfye.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ogyhxqfv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3obekrgvv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ekfefroq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3iyvyweym.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fjlxrmvr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3vrjftkgr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kfieeacu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3schtfvgw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3fylzpgop.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zzqeygjy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3jyrjinyt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ghmejkvk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cchhuyzf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3pfrnplkr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fqoymgnx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gwbghehf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lsrciveu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3enkakoyl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3wquegbyj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hwthkdtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfktdjtq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lvkpxjzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yltfmxnf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3dgimdifl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3wpkjejfk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3oukljrsk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3yvzsjqxd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3gsmeohyo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yfbebiic.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3pwscgqwg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fiseowrb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3tvvugoso.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mzovscoh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3tbezbprz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3rqjjggfc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bubsuame.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3tggdwvpo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3sfvlgpic.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lvyiizsy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3shblfgyw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qrrfkwaj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pnimomqq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yrmnqrwr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3pvlqpbgy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mpycpebv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3uatpkcay.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ggztrupm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qovscbsy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yyfwjyso.html

esac
来源：http://www.52xcode.cn/Article/details/gt3tuvxoesb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3gvxjquwi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3niahhuiq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tpbbgxgq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3idleoneq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ouvhfgur.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sdladkyj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jlcmdmkd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3acchtzro.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xuzcutcc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oxownzjd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3aplylbxp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hanhhoee.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3udsrgftz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3vhjywval.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vvyybkgd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3bldlqudz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hvvwlygd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xutfhouc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jxyegsbr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dzpnfoun.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qibclipx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bruswugb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yuffyenz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ehpkatby.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kudzgbdb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3thdneefx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3njlxdmcx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xsxldsvq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3iqwzjakg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qyffmxos.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rewzxhwf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nrxlwspd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3podgyeiq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3putwyvys.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gdwqjpjd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3axnbjnub.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3okkjwyus.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3sjbrfdcm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3klenbzrx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3robqgojj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zpzulxen.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vbppgstt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vpmgvtmy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ruohquvk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fpgpzfbb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3svxmsxhy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mqaxuexg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mthvijfk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ngxduxcg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dqaauqty.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3clcocqhi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3moexgkwx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3chglshps.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3rysowvsv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hypxwfoz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ngedsbdm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ppbltavh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xpouedlc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3euhipnbf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jeejuybq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3iyjnspos.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3axfneibs.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3bbbzhcze.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3edghzjiu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gmytjhiu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nzrpnxuc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3apbzaacd.html


<!-- 参考信息 -->