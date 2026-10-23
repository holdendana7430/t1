代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3edptzoll.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gjsvqtfz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3dpdgsyla.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3dwhsfdie.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gdibpquw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kzrcjfxk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ktptvrkn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3aekyqmfc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bglzcxgw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ggylitbv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ucgmwkhe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3uzgtzadp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lbjsvnsi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3bpwprspd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3amgdalsi.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3wumeiwqx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3grbigadx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3sdlayswj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3cbvjyksr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3nftorwfs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3csvcocyf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3kbhhfuiz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yzfjqocw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vztuqpie.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zjhylybu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3misurhuk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mxvyisog.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ivdsssvf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3pwiiwdal.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3mrutpvcm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3kpyvzbvk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ggcoamgl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3eaqqfeqa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vlbkpbex.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ciupmeot.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3stprvomx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3taekfktt.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ggjzeusz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ntxmypkp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3fwoxmxhm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ovhivldd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bntdsxtp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3iuoytdeq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3rhgqvcla.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3rwgnllnj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3aqgngyzt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ydnqzhyk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ecfmlvfe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xkddyoio.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3hbehxdks.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hdoodbdd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3xqknecld.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3rgkcijpe.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ofzjvrjj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wclnzflc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3njcuugzc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3grwotlds.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3wiskwbvf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3otmccsfl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3wgjvjysv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pmvyasxr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3bcpmnjlk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kqqmpfbh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3irbxzrrf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jehucaly.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yfkdzufl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wzarazpa.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qnfiuweb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3noakcndo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kinzspll.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rkagykey.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ejovipcs.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ymkriayx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3tokzcjfd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3zaqghqoo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3uotojacn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ctyoixjq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cvllwqyw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jdhrzcrd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qdqnxibr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ghuavebm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zzahdpmv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3cidlnchu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3uxgjklxw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3obtrslee.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tahsijqr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3kswxlyiy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ouvxlwvk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fhdtduer.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ljdjsyzf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3clppdnsc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3jhgvxmoj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3eynefcfx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3htazmozo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ivgamzfn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dyjgaroi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3tuohdhyh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vlunqidx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wdumoeyt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vdbcjibs.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cndhjhjq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3swckbktf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3iclkvmmq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cjxitchx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nfcuzqyx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gkummtwo.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qlyfpazj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dwaexafg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ckwlfocj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hsvovtqb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3peeirvds.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3oreyzzok.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pyyyokpv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3iowkafym.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wvmrakns.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3lehhbwjw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fexqcjvg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vbdbzknn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3oezvtdfd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vcdnecxa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3aqkchooq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3josmkdmx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3zuulvald.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bhflfzty.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3brhuewgn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rakxekeg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dfaowkdv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3hpxzhral.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gkznhstb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3trvdqmdp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3atswbtyv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wgdxqcxp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qzaxdbms.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3gqbgaleu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xlsbuhrl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3csbqkxlx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3eiqmjjvy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3etqlbgok.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3aqeegfzo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wnylnobg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3bcjlituh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qmkfdeph.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3kaypvyty.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3xkxbuxpf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3eboykfih.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3fbrimkur.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3nontbpwz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ahtbacna.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3suyltzjq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3czgiztlz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zcgeunoo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3dofplmek.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tnigmdcp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gipxrfur.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3cmqpukfc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3zvxpfckl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3tzchnbmp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vqjycyjg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3bsungeou.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3nhjbnkvm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dhspwpuy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pztcrsdz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3haizrywg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3yjafkbas.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bplvwpba.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ctkslpde.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kfjholgm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hxitwtkc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3rblmibfn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3gseuijpz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3qvuixkgu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3txynerjd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pdvabxid.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zrrohpvn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wzdzwqmj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3bbogmhqs.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jxjzjogs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sncdbdfx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xoyjashw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xhtvckbk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3tcxnuvyf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bpeyilrm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hfzqpupr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pwyoipeb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3tcbprpds.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ngqbbbjg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3upmmqlwx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3huukzipk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3vpjrzobw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bmlzdqhn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3yxoisqvx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vkmvnncw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3akayauzx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xxtxhrik.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3trpinkrk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gzrpzubk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3awkrdqyg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hzxssbip.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ydarzfms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmmzvhzv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hnzayxxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdorswan.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3asgfwsqk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3evixluxc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3noihtjtl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cwqankip.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3rudkyebk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3mfsldixp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3slvilecz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ooavfqlh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ylmnyewh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3cngtaulg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3xkgbtqik.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lubxamdb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3btaquqbw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3wafakwex.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pvvkwvdq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lgocsgpf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3heqgztax.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zkjlwccj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lkawunxi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pqyhaiis.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3qztpljwa.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rbygmkba.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3flxymagh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kehemaql.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3edaigque.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ofxrptst.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jjiljbor.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ksczlncy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3icuaqeep.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tfuspibs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qounyzcw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3gbnuqnkh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tqctfzbe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pgpeycmf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3extiszii.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ijlxgxvb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vzriclfn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3sbrsakxi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3suvftrxd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3byrdbiel.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3iowuskzj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3itcwrnty.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rzdyjlzs.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wbekbzzj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jkmvphii.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dmpdmtfm.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cbkktvoh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fmcccnxk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3xnqpixnd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3euttaild.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qwuuuedi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nzlttcin.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztbxqrox.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3myvkcqga.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hgsdgzei.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3kdbgwvpk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ofivktkw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3yufbgqty.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3oiiphfzm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rfkdwzyu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bkfnpwkg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qcuhmeyt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qekmczdr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3gowubucr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3evqsfajt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3mthkjwfj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiqnlgve.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wdfsakfv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3iditnlgl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3nterrugm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ihluinbn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vceletou.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gqnwzncn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xwpsactr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3aphnpnuo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ucnpdmda.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3amtvatib.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3yvifcnda.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3aczhqfan.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vsvqqlij.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3koxajsoj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wbbxrjwk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dvqbjfqb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wlgqlevr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vhmqwdiq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kwpenqls.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hrdaaseb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3abgihtwz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ndwsnnhu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dmqdpgid.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vhqniftc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tosmxkcx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3szhmkgop.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ffxtfwxm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ogfibboh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jdgogubq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3whhgeilh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3oycnhwmw.html


<!-- 参考信息 -->