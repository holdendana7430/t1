代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2onbrfpuh.html

);
来源：http://www.52xcode.cn/Article/details/gt2dstgrags.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hvlgxqag.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zutblmta.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zykmburh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dnubzkgq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2tvsaifnw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2rshekjdy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2djfpasys.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bkdnmmjg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2iehkmzln.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2kztksfny.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2szifavhb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rteifzib.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2eadvyohx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2aigamdmq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gggpffpp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rdymkmap.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2chgemhdd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2cmievkdt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jdhlnjso.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vijtqcyg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ecpepclr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2vzefuuqv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2igdxfybo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ytrkygqf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dluvyzbb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2luivjvxq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2bodqbdha.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2bcnyuhhi.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xvoxgubg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fkhntpwn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hqegqghc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zkfxkjel.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gfeeyrzo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2uiwmfttr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wtyazkco.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2skghxvak.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aeoawqxk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wuqlbvsl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2vpurwjtc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vfudsmkn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bbaozivd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2vrraymjl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ygozanwk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qxlsrrqg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hbtwnldx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xdiehhlu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rlwywpdf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rngqyyaw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ondnsnmc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qyhcknqy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ppguxait.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2uhzvwhzx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rmsgvufu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kqnypwmz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tllmusmg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2eaazecll.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2khhoorcg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2reyyrofh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vjwfpcfa.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zsfekxmh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2thonuwbo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2enwpcvji.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2emmmaahm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2vzrzqgyj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2npyfxjwk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qkcccemm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zpiwoplw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2eylmyhhe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sapupebw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xerbbrmz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2alfbeehc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rxrpxqav.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2piahgufe.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cnayggtf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2vkximkfp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cerfjqxr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hdkuifjn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xpmpiqfe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zylqkuhc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2timhhliz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hsowyzfx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2buhrrplg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hltiqwvs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bxjwosrd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2otzxywzu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kqkppkkw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xfujllpo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2fsvishkw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2aqrvupad.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2cxxdblkp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2uyreurag.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rqikannd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ootakjld.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ktzdrozw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tamazvuo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nsayydpi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2bbfvriay.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2iudjzmco.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sszxkqws.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2sqlithhs.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2crtfrist.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nbsilhev.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2htovwrmm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tghckbmi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ldmpqhqi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2aohdooan.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jockuvtc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dmoufrbf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nmzyrykr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wsgbnmic.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rxurzkqb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xpkbyscy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dwfttkwp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qxtcieah.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2allxkfcm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ydyrewyp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wpvhxvft.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2dlwqzojr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2btqvqqws.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hpwzufty.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2brqyaohz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2oljheicr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2umhwtvip.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2yeimtokn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gdeubill.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2abervpwb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ncdyxwkx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2soatqxwm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mgtbxdhe.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ynvvwnjw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cmzffusi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ddhabahy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vclcttku.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sdnrinyp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2vrgfehkf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eubuvpnl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2flfjtrpa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pcxevhay.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rzlpqqho.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2euajaiqw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2vgczjhco.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bvhtugcz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xvhjncol.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ochtkxlv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tvwzemcm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kqakmfwd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2srktjklg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2otysrozl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wiaqsxyg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2mdcvfxmg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ahiegcuf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ygynbhwc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zgxzylje.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2odmwjjte.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2bjgfeirj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2knemtoma.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qlaamqbd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rngyjste.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cydhkdzm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ehooakam.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2tzxpwhqg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vurowzju.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gchxhiyn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lczugoer.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kllqwtad.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ddplunhy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2pwiodqpi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2pjbyzozl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2nxvhvjvy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2iknftmoa.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hggplzpd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ktdpbpej.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kfibagib.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2cktjtoqw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xydlutgf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jxhnmbom.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qwcohmqs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oawbmppv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2yylkmwbg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cayrlugg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ujpewudc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lruxcbbo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wgslxghj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wtxyefal.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2znejynmh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wpsnjwvh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2eaynhdeg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2plmidkns.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jsisumwp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2laetmnsk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2igvopkou.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2firsygss.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvofjfko.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2vupweeqb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ucqvrsye.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wqfxlemv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2hnmckqxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xylmzdxp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2eswicaop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzoqwqhe.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2kgaklqyw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2fqbxmpyy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2lsufplee.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2tjkavuuc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ojuidsig.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rzrtsldq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2klkveoic.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pmffbblp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2alcnnqtf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2frlqmxbo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2beqiijoi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2hxosmwgg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfpzycar.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kxaliavc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ehegadvc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2yoaedinh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vgljlsbk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tksiyqti.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iauzgxhd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bjebkggh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ripeewmr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2flfgipvt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2scyztssg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yhnfpuhv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cnisodvf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rvzgfxld.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nbyfebnf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2todjrnwt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sskcsppp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2buxdqdiq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nhepmiif.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lofmuhme.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xajlntgg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2thxbyjke.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kubakhts.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2suyznxbv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2glcqwmkv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2obktuurv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2hgjtubfs.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2twflpdii.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2vjqfgzod.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2clnutsaj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zwyjhcfw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2vqchctng.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tmphljzp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rsyenuyu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hngecpuh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zgzxrgxu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2qrcslnbk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nnwzjqsd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rklhujye.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2doiuqouk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cxtmogfm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zpnwtjay.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ruimmjrn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jekcmbsw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jlgqbgsy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vqvihmvd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2jetokhns.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ihrvgfyh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2syhnfymc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ywiccbqt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2wzganqvb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wtnkkduu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mmkdofnj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nvleobws.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpbpfnlb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qevtejle.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dlrarrol.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pvwgetga.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2idjgdmqi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ysfnustb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xokfjboj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2rdqbwdni.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2glzpzmma.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ldlnamqu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2twceuetf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wbmkjksq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fygsnibp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2sxcnaoev.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ynipnnpm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2apcigjge.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tootmrpm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2lyeqsier.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xewufsav.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2alknyxlf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yviruosj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ohgpbnhw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yfppaaiv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2pcmuhcpe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2bhrqmqzv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ksnkmohi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2loqwpqff.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dpakjbas.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vmfbkmmp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vtypswqb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zaykqbyi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2cranfecl.html


<!-- 参考信息 -->