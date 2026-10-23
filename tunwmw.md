代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt3vlhdltuh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3iemnoixt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3izuudbtp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3pvkuhxwo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tnsoysxc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3dkdaajmo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3yohnlytu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ydldebmt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bfdllqsj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jwinizhs.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3auztgstd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3srkaznpn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hvuqkzec.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ljogveim.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3iarlpvhw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qnhmeoxj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iqdaiwff.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zulirfrv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wyulwblx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3styaecxt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3gpkfruho.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gpnullcg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3senhrjdw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yijuvogk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3byqgcjfu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3izamteie.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3lredlmzz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3nmlepwcx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yyknwmuj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lbdqrbds.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gybaclfk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3fgwvxaui.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cojvnbhd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zziwxztv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xtuywemq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3alnlxyoy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ccaaqlbe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wekairrn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3hgzgoxmk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3aryqwtdq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jqajgqdd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3kswbawti.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3rnmhxfet.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qajadbhy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rwwzrlmb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3abwfmryh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tguxdsyp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3kseagxaq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3gpdxesdq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3nixhgglo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yyekxeri.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3wpetgbpe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qcdtpdxs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3okpepppt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xydzshyl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ebnavdyw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tfnpbbzk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3gegfkkgg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pxwiqrjk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ccdouajq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ydljhmim.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lckyerxt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ksezpino.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3aovhghfz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3bdjpsvzj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3kneblmok.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3itrmjjfb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mlkcvchq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ipsduqya.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3faqrfqiw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rfypzbwg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ylriuqzs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3sduxvzlj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yniylwuz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3pymfdhrb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zmbdonlv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3irzdhyrl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3dwynudow.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3mesoscuj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3irhwdzep.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3aoztbpsn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3wkbmlekr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3psexgitu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dwovjird.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3liriyogu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ijnedmqq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yfeyssla.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dbfkjryd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gdroymox.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gmhyfusq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jiinuvry.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3wjthsmbf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3tyeqyeei.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3pdfpqida.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ngsnmnho.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uenaslgz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3qeedgrpj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3aroowwdu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tcxikebn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xuqkxuzx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3opqbosxf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3eybqbrdi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ccuvlcwp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3biukrjuo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mueigyfs.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3cvnbtoum.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wvhjjfjh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3giexxgwi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zpjzadnq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3sxevwktb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fbwxtuzw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tmvjsszr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3shuguomu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hngnjcby.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ouarbmtb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3upzwadxw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kvxujkdg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3apamxuwf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pcupemcr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3wwlxwusr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3thptcwqa.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3itzvmocs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uajlmemd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3hevfgrax.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ahrjwvmp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wbyblcrk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dhyhyimp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qdloqevj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3zdmviqja.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rauiugom.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ptxcuzae.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3veajfhim.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3drqiddsb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3itpyxsbx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ebclituw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jpzddrta.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bfjsjcld.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3scereluj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ejhdqrwn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3owsubzhw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ceuygxrd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lpokuxpw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3umeevkpf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3fspupgfi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ecqzngnl.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gqxmgsui.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3acewrvfh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3kuscffyp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xwyhomps.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3eksqwttt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nzybtczy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3czqaixqa.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jyqqnnbf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pderohvx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ajbkxexu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3uyhjlqiv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3fzzhxsrk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tcnclryn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sxryqwpy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hgkcdnat.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3htfhsvcx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3uglzszin.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3kjqlfbyz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3pjwbhklo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qmkpkync.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3jxilytyy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ypuaoflx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3sbiehxak.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3wzxblrat.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fowvhlie.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rbxiwyjp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dkqonatr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ttirpchl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3disdtkiy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sobtxndv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dtzqaksi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ybwwrgfu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jyyquafq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3dggetefp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3jerbfqbn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ptynvahq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3skeinbyf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3nxfpnyvl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3imgtthye.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wdhedetu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ihelrpnr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3etnqnooi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3njwxgdyb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zncfjndb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dghxctfw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3fvkccwmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igqvrjcj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ezlkdztk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnqscyih.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tnvdgfot.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3hhduariw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ptvysjjh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3godbpmxc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3svvscwdm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3vyvkepff.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ocuwlolu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ojzxpppl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3klzgmdxe.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3celocwbb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3zfyllyvn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3gpygwubb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3imuxuhvs.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3kmbxqhev.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jfxbdsoi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jcluxcad.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3vvjrgntk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3toyeympd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tidjxdxb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hxmwiozf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3cixpbnnq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tcgghhip.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3lqffdizk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3eqlhqdtt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ffqalerh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nmmggsar.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rnkcgftm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojagjtpi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3idttmqdg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dopmchmv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jkwqxasa.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zmprwswi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3yugmlzmg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fxwgabvi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3arzlsqej.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3eswtceif.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wmonmnhg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3yvujuxcz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3lypbgggj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3uumxcxcu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jrhzzgqe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xvexgvwp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tjabnzjv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3aqmbyzqb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3huefmfsd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dbpkeswv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dxdruprd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kpxqblbs.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ufgongvx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zkkutlpf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vfvrodkb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nuojgali.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3sldqrgdh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3nxupzofb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ucdzuosa.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3zdleqtjo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3enoqhyfo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3maabordq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vxfjpcif.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vctsqhie.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3qseehzeg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nocbgjmu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xmvjuqym.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3veixwqbk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3izqcqwdg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mxledacd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rbmilbjq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zbkoavxe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqcdhkwc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qmraqjkj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hvkrzxxq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3iwbwzmfh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3inpzerbx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yltuqtot.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3rtasdahf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ajqxqcte.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3hmrgwbdf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3wadwbvuy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3gpkqiyxo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bncjhfvo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zkpbekwx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ippwozhe.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3epzupemy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nvrnuuli.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3gtystjnp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nsyyduxs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3efjvuinr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ycmqjsqg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3jcbjivdx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fmxduylg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zcgjsnfr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3rxsmomtf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gqnffivq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zsampjed.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bkcdbkkb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3fddoqyns.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kmmeopkn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ftjgnwnt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uyfosmhn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zsacjfpm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pfvejcio.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3evptnhkf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3mnccrrrz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qbjztcrd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fvkstbcx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tpmdshks.html


<!-- 参考信息 -->