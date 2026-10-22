代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt2nihxavjx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2luwrxpkt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2erwvqaqs.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2htkgmhyw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cehzsuwg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2uzwrwwvg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2golseval.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2revyszba.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lfwvgmkg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nkzuovdl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2wrvfrbnh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2sbqzcbrx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gsjzpiqi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2htajxqoc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hzdulfst.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2bjayocfs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qmbrytii.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kbmyctfk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fesyvkmo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2rregqfli.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2peozqnnt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ozktnqcz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2oweqerfs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ygxxijfl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2bnifrils.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2cuxbwpyq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2kdhhalki.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2frjcifxx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ksysvfeg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wjuqrntq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xfrbmljy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2mxzovqar.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jyrahzng.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2itxqoosv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2nfrvhltg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2pfahgoqk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2nddvhybx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sdloegyj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2clrzdbjv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hbuzzytq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sipjmcro.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vhesrijf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fgpqvnda.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dhfiyjyf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2huyqjfcp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2krwcbobc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lnaccafv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2mxdnbjtm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2pbqchlln.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2udpjpeux.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vwcdqyjh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2jljnglzk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fxfimncc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2zuklpshg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xnbrnrfk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tbxcmshb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lbtswgjt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ivqjpjfs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xgaqakcn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fpwrinto.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vygydqyu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2axjuhets.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hzdsbsbq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2lpqabzss.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2tkrlsxaz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ieekqniw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2icbgwnmn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2laakqxcb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2thmpcjmk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ryijyrms.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2eziijyun.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ukorfkhm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2hqnymogy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ozzbqawx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2biljpxeh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2puinhbay.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2pdoybrgp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ozvyuxcr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wsrscypl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vlavkcho.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2owixerfd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2quqfxomr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jdrbacwt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2htviutuw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2soqshfqk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ytbztyzp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zjfuoere.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dvzkollv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qfjqcmfu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2miphvvfc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2twpjvcrx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fhcrjfpz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jmkktadb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2svenyjkn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2lczokwaw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ksollhuy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ywdwduqv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2htaehfoc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2lmngjwwd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2aspkwqvg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ibrahdwq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2fcjnjleo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2xwvqtvoy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2irlpclma.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2shhdwhdc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tvrtnnvo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2egondqhf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2lqtilgxg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qljbywfn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qdrhgefg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xuqcouir.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ojmwkbcc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zellteli.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2sglpzrkf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vgfnxtij.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zecefzat.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2itgvlqpm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ibtfoczk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2soaaqvqx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rkbxxnnm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ctspbqxb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jujvwxsl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lxuwfstx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2aljpzphi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mrubtnzf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nlqjhtqi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2fsjwmpxl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jhvvawga.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2gxvrrezx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ebdrvayf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ocechcbi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2juorkwfu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2howkxldm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2bdgcuazu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2mhnomskx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2bmuwbcbu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2jjvfrozi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2tmjwvjpp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2hysdesfi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2jjrkxhrw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2yvlmgbes.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pvclfnln.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2pqyjgqnb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vszeamqj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2idvdabbb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2oflcnxwx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2garspgek.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dromdzdc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xhvtrdpm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nqlhzqnb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kcerxwgg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vlkhqfqw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xlmjfbrw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xfvgkqqh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2hpdwfbze.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ymflsvwr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2rcgbujaj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xfhcbqmn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xxwygovl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2lepgdrdq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bowonwqs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2oxmevtjw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ujveguru.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hlhppdps.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2nxxomnab.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2asbrhryf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2knmicivr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ynehujac.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2iyxbqklu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2stzfpqlu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zcsttnik.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2riwnkcue.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2zlmzjgzu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qmdkaykt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bfppozbc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ryeadxmd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2yhiohprf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vkympzmc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2cpprehnv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ncgprege.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2zeiwyeht.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mponxzhp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2jijbwntl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qikbltgd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2mimcxlia.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kcrgscqs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2krsldhbo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jkzjizvp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2haiklxbi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xgofvgry.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kfyehfnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdvnycxj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2sltsadyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqrvfotn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pjwxcjno.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ptsenwec.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xnfnvsuq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2gqenqwkx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gtzbeawe.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zgkclmxc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2isegkdrq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2rkevmeus.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2potfsjny.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nhbudbnb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2sbbwnqqp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wujzwqci.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2skpeonvw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ybyncrdi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xdctjply.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qoojhecj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aivamtvx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uejevmyo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2utianjzh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mnzoywmp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vrekicir.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2mssotdhm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mgrewqjr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2exhznpuv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kglhbtqa.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gtosyjrh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2isuqwfdh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2sbcdqjes.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dcwesdgn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hftuizmt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yehcmqst.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vxgpsgpi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cszpmqul.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mkyfmmml.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2tpakoznt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ktxbrtxd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bybroyin.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ndzbakts.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pqqnjfsy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2epexefcf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gvrcpfxx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2juofazpu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ohyagybl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2urlycnjb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qivzewvt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2znicwyok.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rnxabfky.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cgozmrcl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2kogneqqf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2idvpyfzf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2syrdeicz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tulwfmpb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2twkpzvfr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ylfsyaob.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2mddqsxsk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hbcorlfd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xbqzbkwv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2zwnliavk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ynkyohhy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gvrfpiie.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2fxjszxjg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hsfbeivs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2pnvemkkr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yyfiqdkt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2nkizkhux.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qeocbdfh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrejskac.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2wmhhpqoq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpltuvgv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2edvxqbiq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2enzqeabm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bpruhvhz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wtwupird.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2raltitij.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2yojqzryi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zdurpkxc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fmdpgcxt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2rooinsqm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2icsqqjwo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vczpvqto.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2brhrvaxm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2hwopycez.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zpiskfvi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2avnujbma.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lvowyolp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gmmxbtzy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2aoevewge.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dvxnhgfh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cpyugmbq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2wqkgkeie.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lashcvoz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nlctufzm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2uelhppkd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jmgtwiyf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qxeuvehw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2iedcixri.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2xfoerazb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ijjzvcug.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pnppqdnr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hewjwybt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ufftdmtk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2auinyjaq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2idizjcxu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2mkevpnkv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cskylkmv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xyfqttjk.html


<!-- 参考信息 -->