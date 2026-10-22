代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2kgxhxjkm.html

);
来源：http://www.52xcode.cn/Article/details/gt2nunyzayl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ghytoaja.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2cdcmycww.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ufhbjpjo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rchsaxhp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vzlhksov.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2sojfoxjh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dovaqzfu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2uwcouded.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ozmqrfui.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2irunwqse.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ekutxuak.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jqvoxjou.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2tresqivl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2wrtowtnm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2gjdelzpm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2idvqstik.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ootikjqu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2pkcajfab.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mqpqgrcc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gjrtgvoq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2daeociwu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2yivqkwdu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xkfyhjjg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2tiauvaib.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2osbtejwv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vbldtrkv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2oqkcpzpq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2mwlxeedq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2sdybagbi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kuoymwkj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xvmomdlx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2gymrtoes.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2kraiovpb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zuqjkhwp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2casheslk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xvxsdvjq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hnbxsqkb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2cahlrmfu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2pmhwhlbg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2euvbqmfa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2kmqptwbq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2vwxsxozy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vpvugwyv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ujxfmjts.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uzojwyha.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xwsreaca.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2prtrwkri.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ppajjndd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nkcmcwbf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hrwqjpjd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ubadvwxv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rbnpetdh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2psvfvbbm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2eqqdauuq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rcuhvktr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2sepdnssk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yjybfddp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ijjwqljf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uramcqgp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2gylgscsj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mxxzwplj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ftliorpd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kcrganpu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2vmyfdwex.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2myjkuwbb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dnqxhpae.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uiovottn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iombvbpw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kzojjdwu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vqpqatnw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2vuezwtir.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2lqkaafqs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2tkpsroxr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2rwbigldj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cospnxjn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uzqfnkrn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2yxbstcvr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bxkwhiad.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2potzfyaz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ejrqntwe.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2swjgijii.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lztlykln.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2whtiirrt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kznyfcxm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kjltbwbi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2bklroakw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2srahoomz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gfnczkbx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kegovitq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mzdztaku.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vfmlrblh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lzdeexhg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aeeiiejo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zdjctvpl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2yyowxvgl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xggebvxt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vfujtvwh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2snkdogfd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wzxteiew.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lkfamull.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2mznmhyzk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zqdgegjp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2oonuyzry.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mzbeobzq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2huhgcsed.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2nqooaqfj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2edtwiuvp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2eyatneaa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bgwvynhp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jbsuwmms.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wgbozseb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2yqmswnrd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mfkejpsu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2anqbflau.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2esdmhwre.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qmsuscrv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ewschhta.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2afcxjvde.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gopleiqv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2cmiiaiku.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jqesjzkd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hegdyxyw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jcncdkav.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2fvbydkue.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2skxvtuft.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2jxvggawm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2konkvanz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xtfezisw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2whnldeas.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2itolyqjx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xvgzwqiu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2gvhsbfit.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2onjhxeat.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2auquuqcj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2kddzkywp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ifhkmwmx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2krjzmdfp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xvlskidb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jxaofnnx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wkibmlbd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2drmydzlr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2uedphyof.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2nbjoitza.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lduyfhax.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2hasqwnyw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xwdkwofv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2fwirndzf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2cdmlyqoc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2bxkcpswm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vdtcbrci.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dggmfuyz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2hyymexsu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qvcoaknp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ptsawzlm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2bpsvhsbn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xvwwoyja.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2sgmuddno.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vvfwjzth.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rruolslb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vvirbecx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mzbpqdek.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2dnsgcsxk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nrfjfnys.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ggvmupdr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oybpqqjn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zpovlolv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vatdqzke.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2uwthoxzx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2yjssgntd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2vfnhdcxh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2mifmbjdg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2pirkrthg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ommkohlx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2dafczpog.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2iyluqxzl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xjrffatp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lhpssnec.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bsmvsobh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2tbykvagi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gcjdqzyr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hlmeleyi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xfoignyu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fwtwdhoa.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nhcyhqjo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2apuywymj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2wyscdjkb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2gxvswivi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2cjirfrld.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2hsznautj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zmirkgxm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2awrmauhd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2lufgmchi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvdfkdql.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ihesyqpz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2gkhhksgt.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2abyvjicr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2thixnztv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oamozwpd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ndibmpux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctxfpqhy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kohziphm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2tctaazft.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vbaopiex.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ppkkcphm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qkjuwgkq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2efnouyzm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wjphhncq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2qcaxownj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2gqvxaxka.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mdjbyqad.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2kbnxcnkg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xhudgopg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2voliyyfx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2omtazwgr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jujfdbpx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2stwhkjrw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zaizndza.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xfpexzws.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2kugkuphr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2pnqvpzgj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2cvtugzqu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yqunojqs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ephvaomg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nlildyzn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jcuolncq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2dfmcuhnc.html

esac
来源：http://www.52xcode.cn/Article/details/gt2dwqijicz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2gauxhsin.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2eqljocyy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wxhbdwxt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fkctbdof.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2umofaahy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hfdocamt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dbuluiwa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yemybowd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2bsddqccv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cfjjwxpv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cugxdwft.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vwpnfuph.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2bfptdzzq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2watavpyo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wizbvotg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2sngnuiou.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2wjzhscet.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wucbhout.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yjgvgfge.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pwqpfsnh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2noyomtoh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2iorcyufm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ynnbslgy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qknddril.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qnipigfg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2khqptcmt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2feqdkhne.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2krwlwszk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2djvukbjx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2rehylkmw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zvvgwkhr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hflwykbm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2wlvezfvw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ckklrhlz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ruogrfyx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jgtbyefz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2efuyiofi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2abilhjbv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2lrhdhzlv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kxhajatu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gpvhbphv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tjbsqlzt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2uhvmzlxq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dpmlwmtg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2lwqcnrgo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zenxtitp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2egfchppj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2iufcocxd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2czimfoyq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2lzvggujd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2hxtdfpeh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2pylajryc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ttfhssjc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2yxhwgskd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mplqupsb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nlwlixbo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dtudmmne.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qevyswto.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jdnodlou.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zhmsyzni.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ndkqvfvo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2iywpikbx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2eienbfbt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zdzdwtko.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fzrnvwru.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vnlvzacd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2malkohhe.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nscmdfgr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pwnrvkqw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2cjcexgpz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2yevwhrwf.html


<!-- 参考信息 -->