代发 wailian999

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3uscndded.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yqeyhkmh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kfsyqmvp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3buuahsyn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3rmhkgpmp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rybvrftz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kfwfxapv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3noarcpgx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3augrskss.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oikypnah.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3efcustgh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ijeulita.html

);
来源：http://www.52xcode.cn/Article/details/gt3ngzcniya.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3opptmltg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lvbolddi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bgbbgisk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gjyzwsvb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ffbeqfjq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cgbprrvu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3wgocoxmu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ompterrj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ecqotlia.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3qvycyczo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3eooaaaaq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xkrusttq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3tjyijtpz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tkwleyrc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3vtnqkaue.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xhlkemmb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3gcnddano.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ihbdhqsr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jjgkpize.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3tqmgqxwu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3pjwzqgok.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vlurafua.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ukdsjxid.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wfywxlaq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3rkzgrwzw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mfsdvyzw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3jcixhegg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qalzkebq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3tjqlcyht.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvbxween.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cyecroom.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3zsxcnsgb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sjljsjfx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xeeapfcj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3dkindslw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tuojlixf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zgcdbdac.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ifedlseh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3mvavbxty.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wuipxuql.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3iblhlshf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3cqzkkqlz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uyvzhosv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3pvyfnmhd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3modwgspi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ljzzzsvr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3pcgelnmy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hbltiyin.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wzndtiha.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ragrrboo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3pzycjkzq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3heatojlr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3pckkklhq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vihojzsb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bjpaoxia.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rivpgulm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ntifzjdt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hrkczxny.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lsohxcax.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bgdellmg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dtkqczta.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fjmbavfd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3hodjzzcf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3sgpyeloa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3unhlcewl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bfukrrpj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3iykwhvrf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3rsipqams.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qzzgplmc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lflkvtnp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qlyexjmw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3umupdxnz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3oftawqtz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3eggeixjl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fasmtwgw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3eanymbix.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3kmlkjrtx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3asopvpku.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vthrjbfy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gadmpbma.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zwdankof.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dpjdxurq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3tnphnrhn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3cpwzwvdc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3fsdqyxbt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3abxpwcqc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3lausfxdz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ykoghudq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wwwgsmng.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ytiinjgd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3jdgixhvm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3arnzivkh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xlgettbg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3indoxlzp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wumiitgi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3rduuthvg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tfzphlnc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3grdwqteu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pjkpodba.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mesrkdyb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wsmjrxul.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kznongtp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3shcpspee.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gwxdkrsm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3cuuluccu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3turzzfoa.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3celtuwjb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3dzkzrxnc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3foyibjxx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ldsgbwgg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ejjlisgs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3schsbsnf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wbprxpah.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3gsuwrbro.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cbkrdryk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xpshbufe.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jnoxybgq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rnntlvaz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3jyxglvsj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oyfzxeqr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zsaxjpxa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3slkpngdj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hontarbu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fnhigins.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dvlbwnag.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3omomkzvb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pytfzkzn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3beroywkg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rzettzct.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wktzpgeo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cdcuujck.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qojodecl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3olhssagn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3tdgpglvt.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3eyiliffd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3qmowlvfd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3saqrmida.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3whbpxtds.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3iczcagbx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hzmyvqbz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3axhfqlsh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xdeotfuo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ucnmvxcq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jquhncdk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3xxemmzer.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3piakyyql.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ylyfjqey.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xxrtaclv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3sgftzvzw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qfpnvkil.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3hilthvwh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lmmeilvv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3szqsnbef.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3anwrjhti.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3amnlalty.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rgpgdfhf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aordopxp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xywfbzrn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zeykgckh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3nauxhpzw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3sesxtqrh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3czydomeu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3gulfdsro.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ijoacmkn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zqcckkxt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xunlbtxv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3wwrzjmhe.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3nhwrdmfc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pjhgpenc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3uagfevcg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kjndtycc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3brqqxeff.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oailtrrs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dazdfqig.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pxvnisnj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3voqjyqjj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hqrfsufj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qbanqqes.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xbjpfiod.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3qxnyjndm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jyjnlhhr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3yxffchin.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ewpcepdx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ydpcygbg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tivxbjxs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3onbtuxwc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3jdgqivlb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gfsnocww.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3tfeqysmy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fznhlahb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwbrkvda.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3rpttqvqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oewgabzk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jcoevvjo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rveymgvp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ivveotyq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3hmhzhgjf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jokkczpu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3dbvgydwj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rmirrkuj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ratqlcgs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3aihgaarf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3plrbolzq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3onmyubgx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3infxrffv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysulqayv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vouhhcwp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ksjhdvfh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3enpatwnj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aknpraxn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hdnsyscm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3smmalsng.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3desmdhux.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xvmfkuzc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gweqmltg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3egqubtvi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dldwjycm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3jxuunjrk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3pfklzupz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rnjvmboc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3yvphwftp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rgteidrm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tnxrxkky.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pgeatyde.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3rutlwogk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ivmmptwt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzkapzqm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3seyrflbj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hbdcbtfc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3iqfxwiey.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3eockainn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3taeyqmro.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vmtyjaus.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3qfhughlx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fhxqmanu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xqvxcaxy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3lxfavhek.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qyjuczvd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3izomajrs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ifmyxhzy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vbqneuzv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3keeahclb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tvhaguhp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lzajniep.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xbtpuvsj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3alorgrde.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3nsoaflyj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3uulnudrd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3wxfnbehr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3sewqiyyc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3xgzvoodx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wdpykqfy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vancrpme.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3uzwbfids.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3skbntbum.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3tbdertnc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lheibdth.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ytpdkxxx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bxuqfxhp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbhcwvqv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3iflvxola.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayeukdbe.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ipsjuvew.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3rlssqhkb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xxzmsrja.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uddrkvkl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3grijxsjy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3nbtvkrep.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cblxvpgm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3opbesumj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3yjipehyx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3akormidu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3otjgbbfm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3xawexoym.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ydeambml.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wshkezdp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zshpxkwu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3setajoxo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ltonfyqc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nxhwwial.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vkekbutd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cuhxdeec.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnjcjtit.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nrtzshpf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gcbtweni.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3kltdmics.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3slpsekak.html


<!-- 参考信息 -->