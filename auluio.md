代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt2drpgjbae.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2rbmzjimp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hzhbzjjg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wdpcfosf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2moabkfii.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2eoawcxna.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2falnrrad.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2bpvxigyw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2vwadmjru.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ugszlffv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2mfnfkqqg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2maicfepq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lclyqhyq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2cdwcyobq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gtujomhx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xzrxqbce.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vfygudza.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jodzwejv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rslxezyf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fqxgyehg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jkcyovxa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2sgnpiofw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xfteooqw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zhpcbqtl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wslkxtjd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2yypcubxd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gqnlneql.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ryxxrkij.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gpubmsqc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iezbcliw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wzferolv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2csbrqzso.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2yssklcup.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ldhxtbyq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2kpwzofkr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dgfoyckg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bmghayzb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xlgbuulc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2abfrhvrw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2snwkkikp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2noaaleax.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2lkjckzdf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vvsdczpd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vlqpbuzh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vwjxnswe.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2uimaqxbx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ilsexuqv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2cwkmxcfc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2eaeecspa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hmfavpom.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2smmidgel.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bmzzbton.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2usmoxqju.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2okpkfjrt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2legvofqy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2irylbwmr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nbulwgxb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gklnkexq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sefzaeby.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2racxwrpz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jepshvom.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2upieqhml.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mbxllsfb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vwwxpvsz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2eqmkfciv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hephfdea.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2bjhewwph.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2whjkwczr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mtnocqzo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qbchyqwf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ljhjuzyk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gttcvsyv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rtlychel.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kgdphbpd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2npqzxfej.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jwfjkdle.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2jglruwax.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vkvzeohy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zyvxvbtg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2oxxdyvwd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lphohghr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tpnelrro.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2eudrujjy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jcnsrkxw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2huvxwtxx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2hpjmtqmw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hbrrccgm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2kiljruel.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pldjogwl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rpqikpyq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fascsnjt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2lnxymffp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2dmhuxdvo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cwvbiglu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2yvddemjv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yfmmtuwg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2fbwophnt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pblhufjo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gtsxhzwh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2tgizzdal.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zjtklvua.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2twfizmlt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pwmykidj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jcszrgyt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pvjirivn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wlmxvmxj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2clksyqxo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2vbeosxcc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xplakdkc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pmncpsdk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lzrncopl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2dcdhuefp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2reillaer.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2gixwikmb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2hthnfenf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bdornwgy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wbsxlxoi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ylhybgjh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fgbnxtvz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2syynehmg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hjamalkg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2enveypoe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qvopmdvv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2npkncwhm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ihiknxoz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ywoozugv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2lmbgaobx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2veflolyb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jluqodlh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ilvkchrm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2kybneudh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qxwazkeu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2pzdvbsxt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2tctqkbsq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2seebxtud.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2txqgtmqo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2oouhknal.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2igmnmmhm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xhfueazp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2erqedlny.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kdvwimfd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2zccsfvgm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wafjmzvs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ewcbhpkd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2xyahbcdq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2feiorjup.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2vzihmnoa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dfnrveqz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jeslnkmd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xlzhdubj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2fprlvhpm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zzhcxcjp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oiqkevoq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2sddbgcro.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2oyiuoxuc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2onhjcaix.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2rshqnyzb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2njrpljol.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aupuvsfb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2htjtcrxv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2vdawjcoz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2mmkbqwuo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ceqjknun.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2eiiesxus.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bcufsfde.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wluodoty.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vonldadx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2biqnsepp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2cjrsposw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vaxabqhd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ypfiggqq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2seljeqwh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xwesbddr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oruwjsbn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mcbxqhcg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bczlcdxn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2xroiilif.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fgdwgcnt.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2wyjluepn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2bdaqebfl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ntgkwqpt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gzwsaloo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dnlesiyo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qlkthgwl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vvopasyu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2yizwzpmv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2onzxynrh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lxrtczfo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2somewqjf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2snizuryw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jakjelco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omwbgkjo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dgttrgix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttugxjqi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vvfdlqiy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hnxwxzwb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hvxrcimj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2sacpauqc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jpbtsaag.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rpgpatvj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2pnzzmjux.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2wgmaybga.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ggwnvyex.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2axnvgsjp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kuhmjpvd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uctwymfz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtaqoxmr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2stbtmiye.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2inrpplxq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gemgcxaj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jzykbjpg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2okpfxmsq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ysznixgk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mvgpvccw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2grpyzfrw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2texcopns.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2cfzaybhb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nwvlbsnd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xnawjhmn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2myxdqtlj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2abgfhojo.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2hmewpavd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rhnphrez.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2apdqhlsc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dgjajkdc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bnmemzel.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yfoqzxha.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2atmrcqjj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ljkxdrzh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lmoibotu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2aoqldjfw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2upydxppc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2orvsiqrf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ibqepwmq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uvkwfavt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rwljfrpr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ginnwmni.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2buhfomdc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cprkoqwu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wntrgijs.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2tpoejjqn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2csberquw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2whgtwqra.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2plgrfgrd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jqdytlmj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nkhzhvmk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qtlkjryy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ugofkymp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2donozlkh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2iqpkejlk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dljfwlbq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fovaubty.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2lxrlyrea.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xebqtsvx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2drzsurof.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2iwpnwtfr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2topanjiz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jmgwvhww.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ctcezloh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nxodmtzm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmwnlgkz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zhvpbwmt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoskwwtj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2igeaqrlv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ekmmwnrp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2bbtjmrrf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xnwwubnk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nkrpwygw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2uydtldgh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2anvotlap.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ywzagcjb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2owdcdnaq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ysfoatty.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2cquljhvn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2oeztqiwy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2xzmvognd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2khmfhbbv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ievuinya.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vwwvthpf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2juhwkoze.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xqpvenof.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2axrkihbm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rbbhfkqh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2owvnmqoj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vohsnjmq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rhhdcoti.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ggwpfeqj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zdxlafga.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2uyvvqpqd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mnwskwli.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ajhdfuhr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jtsbkfto.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jtlloiqa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2vtsouwtf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bzvbhxhq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ujefblrx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vqlstmzn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2mwdlngdv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ygpxkdui.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2oibchcod.html


<!-- 参考信息 -->