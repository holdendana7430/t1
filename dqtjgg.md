代发 wailian999

);
来源：http://www.ydjk.org.cn/Article/details/gt3akuintof.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3himeuqpn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3otfoponz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3eauuajgl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fursajvg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3sbkbfspk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jkfbmgtn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3idpfvdja.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3dkslnqzn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fsusjoir.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pjyvqdul.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ndfwfyre.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wkgkwmsb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3nemmulqi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zkufpvza.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3tzckqidp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rvkbxupc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3gdodpcie.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jjcyctre.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3unogjves.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fruqfmih.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3cjvfbvqh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3mcipucqz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hovfapei.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3vcwgarpm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3pfldejud.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qrlpejkj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3bfpzeekt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3itaarzed.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3mqpsyvrw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sgugklkt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3otgyrauf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cinrkcsd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kemnbxnd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3smvpfuiq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3uotnyivh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3trlfoyia.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ntltzvfw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gnjzkmnx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ijlvamlo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3bhlehbor.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3narbyqfx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wfivjkfy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3rxjujxwj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zjlaruxx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xjamcnah.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ynvondhn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3jzycsiov.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rgvjmzgp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rvlqjawp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3obznmzqg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3moahfkql.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3anqyfvoe.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ngriwkxg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yoxesaby.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3iuxzvssb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lynnmdxs.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fmhdegec.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uupznfon.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yjsfbrle.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3empyynqf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3niewofwz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3edgefjri.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3miideepv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3qbscbihu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3uwnbnoek.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vxvzlovq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3admerbss.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3jweokcih.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3lytceuzg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3dutsosxe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3khwagkbc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pnrkfsdn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yvpuximf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3mrrooibu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3amsdyvqv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3uiapffep.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3bxgaknbz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3umviquze.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wctmsnku.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3dmblisdq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3dsmefrvr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tdwaibin.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3buupxzmy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xagrzvif.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3yrqurqjt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qhaujgji.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cqreevjy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hglcofrl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3exzivazo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3iphsbdnc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3iffpkyof.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fzxptkan.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zdjxlkiw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kfvtkpjh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rxkazyij.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qvwffbzr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fuywtrzj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ykukwanb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3yqrghcgf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ffwndfgg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3augymtbn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dystaxka.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3muityxev.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ftscrxbn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3kqehugjb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tdqrqzbq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nqakggpm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nnlntzwj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ybchcdge.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yudnihbe.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3wtkzrfaf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uzmaqtae.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3krbqwywm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3kwjfnkbc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ocvkljpg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nnazhvzv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hctlqrda.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3omttrxua.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3kdhfcjlr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3anxiorqm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3keerrbcx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qmqttyfn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hrdeovjj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3asssolmi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ydlpxgje.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ycsukhbb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cozafuos.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ngrsfmpb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uezknvnm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3cyjrtezf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nkmpaqfm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3axtttuio.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qpoavryv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3iehdywse.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wtcygqwg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3efkujpjm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hlgzsdet.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mbywamrb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3fvzcwosc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dfgdwxjs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3yecypjwq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kvjgwpxa.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xunfzipo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wvvflgfq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zqiqfxhq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ohzjmnto.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3sykxckoc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3yknsxesi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dhjldbyu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hubjcljx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3walgzvoc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ipswjrhs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3yebveaco.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3irgjdqqg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3prhzozjn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wvfqddkh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3edgkkwbq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3awrqlorw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nvyjptqu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3rfwxtxgw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3idyspaxk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tfdmmqap.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3niqfhmhz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hpghaoda.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3nckqkjlm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pvmkjyjp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3hacaalue.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zvowhizo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aymhucuq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vyvhsgje.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fmmhrlby.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kwboqqyd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ntdzuhiv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3eznrajen.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tluyovvj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ezcoqttr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cihyifca.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fpjnjoij.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3uugenfva.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3drhdazdu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3xvktedlw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xuidydkt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cblkwvkb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qqsicdkv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ncizkrfv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3encbxsqb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wpjcclji.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ubpplyjp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3hlmwwcpl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3alaiqgic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aulgguhy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pmartsux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbiqcwyk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3bdeuudbv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tmocglrw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jihexsfd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3sqyzmqtz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qcdibspf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3mnibaksj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3wlqlditc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pzvoqsqg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3octsiras.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3edajtgwy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jabzjwuh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uqwxpmqf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3znncgqil.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3sowfamlw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zdnbvovq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yiahaxjz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3tzkliyyg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kwhwmkns.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wbmzidie.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gugsojqp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3umwmlgxv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3wycmbkto.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hycjyqvi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sfijtmlw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xgaxhzum.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3clvkpnfi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3cdsldbtu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3yodacwwn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wwmmibhh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kezfzliw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bltjsema.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3gnbuwjgy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3owclamvh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eoieghux.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yigbgcwj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tgjipqag.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3baqvbvlw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3keuvburu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pymcmdgt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3axalrmhc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wrlmbgee.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tbnkhipp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ltjjkipc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3devpwezn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bgropwgt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xfgdvrkg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3knmbgyqp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vpvgrrsi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3enndvnjl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3aleyhomg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vvudxpob.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zqgusmzu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3sesaijqq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kcaztxbn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3nysiuozn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rvcxetbo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3yxbydxbf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tpbgaytm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rkkxkcee.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3alwhekdq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3veojvbah.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ctzpcvwj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3sohasoyh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xyebckba.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kpvbdicb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3svuoabcq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjsinsso.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qlukviof.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3apismixh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3womuqdap.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3sitnvhju.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zesaoijn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gpvijnmv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3beerkhci.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3hafglkvm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ptwsqvgz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ulvdmbbx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lbfdlwth.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3znilhniw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3dryipxlz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3lsvzbrrh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xrprdkzu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3efufiwum.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3atuxzaag.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3yxmhzebw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3jnwkkksf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lineqikp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3myhowezg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ytqjgwjn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jsdjazzk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rovnjgth.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3twueaevg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3gaumbkow.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ehqusqll.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3isxgicgy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3tnazdxal.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3yskdkjrn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3aatdzdhy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lyvzwffn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bdazamzl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bbtgaomt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fcalqurk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kyukaynu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3dnkpatsr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tvvqmfjo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ojwhgfcu.html


<!-- 参考信息 -->