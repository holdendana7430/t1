代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xjshyios.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qyuzabsi.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bnusvykx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lpgvzbur.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3rfpbfrlz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3byyjvrnc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vohmzrbw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3focanssv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ddjvacmc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wuwqboat.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ibnbcwor.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3dxkrlclk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3acsdoqub.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3qvdnadep.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nvpqqajz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bkzclztt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ykdsuwtb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3etajljvu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3khjpvgsv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vnlfkjko.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bgvkxzsl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wntxxymk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vppclpnx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3zxecooln.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3imavcqpd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ulbxblhw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xpimaque.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vgvaoxkv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zrdvcfbd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3kohosexw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rknifgry.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ysuehzos.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3pezkcpbi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gxgijdim.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3mvbxtqcl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vgyverdm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3iaoiyhdx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3lsolisnc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zvycerrn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qrtfvtun.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ublotgac.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3homznank.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hpilcsnp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bpmrxykl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ssgyqcga.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ulyctpoo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3focicfnw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3yvrlivtw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3dfgkjlii.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3kkudszlv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iqgpwdbw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3upymlnpj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3knrvceqt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qvdjehea.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gmzdputf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3atbwessg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3awghplog.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ywcqgxmy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uyeytjhw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pcimbkrx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nbvtzwtl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3eusovbrs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hwlqvmsr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3zksblbkw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lcmclrkt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3mmugunbg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vvlwkxvx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ycwposso.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kesgpquq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3bdmxesll.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3guyuwhuh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hmllythq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rsnnityd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ggacbdno.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zjdypjvg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3hiojpjyi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ddsprsix.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3uowntyqf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jxjihljd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3bjahqfiw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nwfvjsln.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vthdtaey.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3tdebbqja.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3weqqiszb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ddgrclnr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qsmmbcmy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3iiaclsqq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3iqewizdy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mzjtpcpp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zkbhifrq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3mmptplfa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3aijeseli.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cpuzopau.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3kifdiqtl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3nrjvjvis.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zgbhbqaj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jzsefjgt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3hdjayoxa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jyxxdgql.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qowdcayl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3yhrtpnot.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nuttsrmw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nselxgvz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3wcoxuvvp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iwruvczc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3bnowvpcm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3dzowgxmm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dflltufn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3hmohsupz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rnnvewht.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3snbbjedc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3nttqisdx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3whnpjleb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3opxenbgy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jmvzbgbn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ndpowvry.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3murvhkac.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bqtoxdyv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jtnpfilk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3tyqnsxrw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lvlfiqmq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3kzitkuha.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3maeoaava.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nshfiosm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ohaoamne.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fhruhdhx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ozuaqfkc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3affgcauh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3bputawhx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zwkhhqsv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3otygirkv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3drlvtytk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hqkkhsuu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ejuyclpi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ocnuuykk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3yrlnanbm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vlqnisut.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wydihlni.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vyocvvyj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kpmfqmci.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3olkwewnp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ipblylgb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ymyynpvv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tksrlhxm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3plqkdqod.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3hkcfhbpy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vrphqddr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3cnmmwirj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3slnhyspk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rwdjrqds.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fwkvjblk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3zggvkogt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ouufeqby.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3nqxonhip.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qezsnxdt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bwecyvni.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pejvzyno.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mddmidsr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3flmespig.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3uzqgkruu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rjzusgie.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lcdxxllk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3awfzkxkm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jlquijwh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fwhwnnxn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3dtcxgsuj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tawripbp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ajjddldf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ztqgizpd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cufsqdnn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3imoeitch.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3sornvylj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3apyfgysy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3xqdgxtbv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3yysdomsg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3cjmblhch.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3eclnvflq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jydgbhtl.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wblcxguk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ezyvkask.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xsizrnbg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tqeuwsgo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fpsjmgnb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kjdopynw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3oywmdnvk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mnopwxdm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3flozpfwq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3movngnnr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3davnsdwj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wqmxmnqi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3sssnoclv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3idwaecbh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3veuypnek.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ezxisnvh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3afnmchmf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tpluvgwy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3gyyzzvxt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ldqmcwes.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aotptsym.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wsbuaifc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3drjelxum.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zyescnui.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3atjhtumr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvhglqgt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mutxolpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uixrfsnr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3puejzbac.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3cnhdqyjv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hwlcquhz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3uhuxvdzb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qaqjrqrx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yxwaysrw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dhjisoko.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ruiwedwu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gxdgfwwl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ozuygfqq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3njqpuglg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jtkzqaki.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cuacloza.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rbilzpig.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3hofoshct.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ogqsasve.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lozxugcw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ktpwwxkv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3zzrsmheo.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rbogcmoh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bzznlbrj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xfoykyfv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ijcjjvun.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3truqmczd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3yptwfiwl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3eqiyyrji.html

esac
来源：http://www.52xcode.cn/Article/details/gt3raytbboe.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3lhehrzwu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tbsfmrch.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3djzojtca.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qbjymlvg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3htlbekgs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xryvxxww.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uhoazore.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3krzkzttw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3rpelxddg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ktvilvlu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3iglgyjty.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rmjzgufm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3dndgnmlf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ddoakmsh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zbzzulxk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3cqjgoknt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gbsbetty.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hhzxcwnn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fluzgclv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3occblzvh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rtmvixlm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wgccgccf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fevmkvxn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lntnschp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cesguefg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3duweakul.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fgztxifl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3voaqzazn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3siljiial.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3qylbpotp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ajmxbjil.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3mvaltiue.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ptjgcfxv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3cthecxhc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ieeyzorn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dvnyzdwm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ybuuchoq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qawyyppl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rnsajvab.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nrflodjb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3sfynualy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yjkdgcyz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kavjcjqm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gfwbmjhd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3flozwnef.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nrzjpdfn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ohhpoubb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fxsjrbps.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ciaedvim.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3sorvnzff.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3yufqhnlh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3drzztjpg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3aasbocgh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fcsmybgt.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3yhtcxjta.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pzomsmpg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vnysziwy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xzxrfozh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3yugvrhqr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nrgryemr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wfvqlpdt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ejrwyvkf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vjmfyhcy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3tqmkmzaq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3quofzijy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pbgvsxms.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3biopuhtm.html


<!-- 参考信息 -->