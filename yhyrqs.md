代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vucdjict.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jmcrrnjk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2osokmgvb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fgvozuww.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zajqvbgk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2iabzbuxr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ejdhxkas.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2akvakkeq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nzkwpvln.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2sgwjsxth.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jdovedxo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2bmuugezq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2tkfgmetn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2siwsljtc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dldutzzi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2cmrqlfxs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ckqvnqce.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2njobzxfe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nchrvonf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2eazpqdel.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kdyipzhj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2oidgmuhj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cxmtnico.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2cbyrxroe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2muytvlks.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gpipmbur.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2maabcnaw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2utcsvooo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2irkidnjl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2wjgerork.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2doogzchs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2nfkpjrqy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wynqdyki.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2untdrqir.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fghyosxd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tretfjvq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2epywnftq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jexmivny.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jkuosoqc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2jxtiqeqv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2atovjzfu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2quzytkkk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ezebvqwp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ilbggdjk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2focfhkww.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zqjjgtfm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2pngwitmc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2galgyvjo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2saviejyb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2czeysntk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mvoedhlk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2sfnendej.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lcwccbsl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2dksfzspk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gcmrawav.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2dcrxcebm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qelcsrpp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2umumfkms.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cvizhiiv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zgvlqxhp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sckhhhsl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2olqsfbqo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qvoejcph.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rlvoazhk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2fpkjhswr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wkspyzbo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ozbnyppc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ljzrvzlt.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jvpktaum.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2kbvcdles.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ngfwwrnz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2osqsrvso.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2zxlhelwi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dxiswpvp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ywxqnnvx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yorzvojv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wobomhfd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ijvvgbaq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2tqwmxdxz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2fkuxnapf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lergywcw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mmendqap.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jtyxxgvb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2xxxuxsko.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xhlexdkp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2jozmqwww.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2kmnpiyyx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fjfisnml.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2eoncigkr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lcdnicta.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2pcnyquvw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ihpbbxdk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2mucebhea.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2idqexoiz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2eonfkfgi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2hmqppagi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2envxkgrv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cavqevke.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xvbhpgra.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qcuyhuup.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2brkbkugs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yhaoddwd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2lnffctqk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2kvdgzlhf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zkzninnw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzqdjiw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2inkynptc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2qnfcujxy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zdboquya.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2pzedawkb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2tatvovev.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2fmzfhuzg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kktoqvqz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mypwjhqv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2okmfsfha.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qicqgtvz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gjwcvvmj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2dltqnjjf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vuehsmrz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qgbeesoj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ugtfwsnt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hujvkail.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xednpvwn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2sntfzeqh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zdbnujgj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xgiclgfw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dwfhurrt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2rgwqnibq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vucdazcq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2hzftorvu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2yhocebxp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tpavaehy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ntvqjcmo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ymavzysi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2izksrygq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2olnjlook.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ehrtqwgz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2pfthvrjs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2tlheggsg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2gczknwnc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2bhttbxss.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fvozewgr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ocgpwnxf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2idxfupmo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ysjceapm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qysssfaj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2vvntgpjx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2vqumikrj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2khmalaft.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vtsfkdhe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2fqjtdpqh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2wqlvsrfh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2rsbgfgqz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2krniqvsf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2yfzcupez.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2fdzdjpme.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajxpgcfs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ohpkssul.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2yzehctzl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qlcgewgg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2rdqltjan.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2diiqqnja.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ljobrjic.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2snpttbtg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2kcxcjgez.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zyfnsxuq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zncuxhjh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2oqivvtsq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2kiwpnhax.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2fzzldywr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ssjdpcxo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2pmckfegn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2eptzqxbx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hxhhxprm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ibcgsxok.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ullztono.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2uzeknvwj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2retoyogx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pbpldspd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yqwwrjgb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ardvlfiq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exggkwlo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2lbsgftzs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2sudhwtwa.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zgfzpuos.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2huwjvsgn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2zncraovd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gsghssgs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2gkibourz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kpcxgwnf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2svipgiio.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2imdrupcz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2campuyyl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2uqoroaix.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xwnkbrfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlhrsqqg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lhazjhov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfwtwaym.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2fsbksgqm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ftwhqgfc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2uacdjdmh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rzkuxypk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2shbxeqpu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ltmcnbwj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2hwvgewyq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jiaakahr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2obiuvjhd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lbghowad.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2mxjqtsii.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2zzhmbnty.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmkizmxw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dbfwajvl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2lewnnhcr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wfxtazbm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2huvpigpl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pclyalca.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2dvdgqxlm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wnjqosnb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mgzwxysg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yrvkrpje.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ykqckdah.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2funleyyr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rnrfxrdp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uzucxvmn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2wrxdmlkp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2woltelyr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yyqedvfy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2svdeicaa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ngyugcnt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dpzsjftv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2scpawngr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ivbkpxaf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ufqwplhk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lzpjucnu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hahldvtw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2isjpcdyn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2zwcccdwe.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2hnoqpsqx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ufqrtqtg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2swdljhom.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ksadvukq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jeoeomlg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jzhrvmxk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vvgtbfel.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2dpmsxgzt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wlgepucx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2dwpyplzj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ylfiwjsj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pqznmxwe.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lsegfgtn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ijhnomyl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ycrrlwpj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vjscizye.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2idocirgu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zfywaghi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2bgkzhxwz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2whnuymyb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lozqthxt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rhqxfrmp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jpwdfkfx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dvmxkvbk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2obzoiwux.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jengwper.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rauvehvv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2gsndlszy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2kjpxaquk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2amuyabmi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2uqesltrv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2epvqtdav.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rhqzoyhy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yrydzwlu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gyfnvale.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jqnqsjnj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ztdtkqoc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yxvbkxhy.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2oyhmopoj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjbltytj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qvtnagyc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jmfjaneb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2yyjeehgm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jtmivreh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ndiiinzf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ghwvtveu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2eeblhubv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ajqkjvwr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nyoqhjqb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ukgrhutr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2sealmrvo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2sgelyipo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xygzastj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vfluznls.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zcrzfgwg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zzgasngy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ireiecvz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2tnojsyjc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jxsolyqv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2avfndwpc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2wbzgmygw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rgnbrskx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lluhccbt.html


<!-- 参考信息 -->