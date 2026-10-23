代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3zpvcgnus.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zqpqpbln.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3akijhodh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3yqasqazy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bykqaptv.html

);
来源：http://www.52xcode.cn/Article/details/gt3xkwhoncr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3mvavathd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3fflnlpjg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ogjzfffs.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nxpvpolb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3kcbozins.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3cvsymysa.html

);
来源：http://www.52xcode.cn/Article/details/gt3jeukhxou.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3eqvtavyp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zdsuwkqw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bhpjgzcf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3htfhfeco.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hsabwwsh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3hvuvcifu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3nigowjdr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ixmlfufd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gyrbojoa.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3cghartup.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ldlctvef.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3uwcfdtzi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3knjcxrds.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vuyiztuk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lpxcwmgn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vyswqemf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3rldgjwma.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zzdmimld.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kkjbtojh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3qfocdlww.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3nkdlkflr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3deklndnj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uecizylc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3algsygjy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3kwvphdsj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ykkjfbry.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mhaobnnc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ezdbudkf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xbrzzhkq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uyafefrs.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3gujshilz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wsbijfgk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3dkiaxvjj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3cvkouuqs.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ayczprkj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xshdypls.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jlugyrxb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3sapggbly.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3qkajmlop.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rxntdulv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gridpkdg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ntpmwjzd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wrsqzxgp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gyyipgzw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3powhwbas.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gxcxftme.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3cgqtkroz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wfuuieui.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tgivlxtq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ikzfsekm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ejttmikx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ypbjxljd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ltcxmeva.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3obunwpdm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vokomydi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fqnknbjp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3nxnpfwfa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3decvwjwu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3yockwdhd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jpgfegzu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pujcfzix.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mfsjlamg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ozyyyefo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3artvwzjy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ovybxqiq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vcaxlwdw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3wdqmojzv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nhohdhxn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lnkakwkd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3irvuurjb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gtpxdkpb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3nfckoxff.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3iwvxgmsr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3egldfblp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ymjyivyj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3wpkquzsr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lnzrgcjd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3vuefntay.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3obgrbxio.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zflhydve.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3skdurvrg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3gvrsoocr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3akjayelu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3aggyydlg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pipqpzwm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rrafzylt.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dqwmyskk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qmuuqzpi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3oydadzga.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bljildhr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3pfghlrxr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iedwykqz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fpbhbyyx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vdscykel.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3udfvhnhz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ivshkebf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vkipqrgh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jhmqdmus.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hlwrdhmq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3currmkoc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jiwdsamn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gnxspvth.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3jkeeytia.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ibyuizts.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3uugwrttz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lgoomynd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3pdulwbem.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qpvvzhep.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tjkyhpfl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zeahldjp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xqtvytel.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3utfgvhsx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3xcamnske.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3gfsysmwi.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cjtlkimc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3exfrzomh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rgydzstc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hssvpjlo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qxdfobbp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hsjzespc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3twyatcou.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3thimvlgx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3yhelkdgw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cpfiivrs.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3twemjtvp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ylpybwse.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ratwjbia.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3iehlupot.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dnhhcedd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xejpfuhl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tbmafphc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3oubhbkmi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3mvnuvfmw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ufoqnomo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3rbmyvqyz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3eigfxbbn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3vvdblzni.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3rflnzcjd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3bjfzuvck.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wpciljfa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ivmldrtd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3mjfmrlge.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rkermqot.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3azlelhlr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ralhccmc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lyzmzvkf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vzxkamzq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3alopglxu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dgjpfhun.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zepqmppo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3hsibdzxg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uxbmyzjs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gbopdfgi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gvchqeiu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3beqsqkxc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qlvygipk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cshxybbp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qfhnvhga.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3kyrrwehj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3longfblv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3asehreds.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3skkusrrq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3rtjfkymb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3yxikwggm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3xvewpzwq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bxfzlfho.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3dcoaxagm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3pyjlsfbb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3godwnbqi.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gxmhczkv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3woofecez.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3aettmicf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lpngsguu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jauzndle.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vgkbjtdq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ncgimunv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xvkzexkx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3nloomxrl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3uaztgxth.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gfwvqrmf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zyewacbe.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3eysiadhr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3eoyackud.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3qfzgwqhc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3dosqhujd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yquiexjt.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3nscovkvn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lsujfmaz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3bpbtxrzw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gfrxtdgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtoaxpos.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3gjroorhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kleokqxr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rfjeqlrn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3jnebjgnp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ipwsjaxp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3gihymsgz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wcfsbxzy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ijtgjnvi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ouiihpgp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ryqwmgwl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3edwygzor.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pigeyqbc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pxvudwok.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3awawxytg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbmtnnla.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3opimhszj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xqhcmkze.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ircmbcvd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bfchlnwo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ygldozkn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jzczxvab.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mlhdfojg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ljeugmww.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gpcawkrg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hgrhutfd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pekjfvrx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ygcyrudv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3iljfkyki.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wqxgfqsv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3qeoocgfq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3uetycdly.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ehbbmlzu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yvlduims.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rhesahte.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xbjgxfri.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vjaoorud.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ylfadynz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3whcchegm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fljitrff.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rgpiydsp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3gwgtsjfg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3pinsqmhc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jzcbrwqz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fhtnconf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3sqawtcuk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3oinxfcxy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pyoqpipb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dwonqgox.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kqdlzxvv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kjxllqxo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vnzwlrcn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pieoomdn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3urbrmdqg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ngjcxurp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3adolwdpg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cszyiscp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wboarbgx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3dydsadob.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3oasepsnn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tpgxpzzb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3snmuuebz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3sfkhzsns.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rarkytus.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qyuqhltj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3fxvtevum.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3aiyvnyji.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3emgtbclx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3mayrllim.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxrqbyxb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gpkfdiqd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3latthxmg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kgspeezw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fpqaxzdt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xaeprmeh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3azslswih.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3gcwihwrq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3iagxaxar.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3jrebnzmd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3yfqsirum.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qhjobucy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3picdvqqo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3iuvgpocv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ajfdtojt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3itoffygb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mjodutmt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3giwkkhhl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rcgozwuh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nlyxcaut.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ynaxoiec.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3uvzatibx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fzkloxbb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3klprjfcq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3iysmorys.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vptwqbaf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ldongirw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3spwumbvf.html


<!-- 参考信息 -->