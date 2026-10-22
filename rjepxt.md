代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kobzyqju.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dnnxjfkm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dnxrytlo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2yuoedzqb.html

);
来源：http://www.52xcode.cn/Article/details/gt2vkqndlfr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qyiyspal.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jkfeitnt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2rmbqndne.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2aifzkciy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2htmjpjud.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2prnsquev.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2rvchpfmk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2bkqtvxui.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2czsapauu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2deynzjfn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2aemiwpjj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rhdpoyyb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2gmtnhjvr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uflpjvei.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2sbsmjvjg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qwxftsfl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vuekyfbp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nkqxcvuf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2llrzipqx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2dypynsjn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lkeatqvy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2iyxchdym.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qrrmwdye.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2sxvmhhwe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2unzeaslq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2otzchgpb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xhfjcoje.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dljrdzkm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hkveavos.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eoxmxgrv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fjulrzbi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2sopnmssh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vnbnzmtd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2gputrayc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2yxontlrw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2clonqzec.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2saunhcpg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2afzssrep.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qfwhkpwq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gvyncgfl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bkmkorsk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2rjxwcemi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tdpgqdam.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2yjpwdsqr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2uffspobe.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rftradqx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ufrxpkpl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2rgattahz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dobejttf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gntfwxpq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mltvsebv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ctgknrso.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ovmvnxth.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pprjsosh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2roznepax.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gxyjdooe.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jqcuuqeg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fkgjwuov.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hsvxyxey.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2thssqkpx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2arnppkxw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2konzerss.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2svorfrvx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ppyvrpzt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2uglniwdn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xusrfquk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2usovbhie.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2vnqazbqt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2itzkyghp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2rieoykrf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jydmazfh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2qbrhyliu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fysbdxud.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wzkkavzl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jzngltrm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2muyedngg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xllkluao.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ymaghnyy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2gupzicjb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2awgmnxrk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2uohlzdtl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2wwmnrxsf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2brpodgbm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2wbsowiws.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2nqloefrp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2phuncnai.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zeadolcy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bzloxlgt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2sgvnbxkv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2eotrahws.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ifcsikhm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jpzwtetm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2bvndclok.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2axcieaup.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bdalilor.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kucpjwzr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ujkgilpq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ctqvanhl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2pdzfxgsr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2getmbrmc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ldjnkrnd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2onxfvksb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jmofbvbq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qtctogva.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2qthvjves.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fyxmseum.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ecqnbxke.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2mjnctsiy.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2zpuenlmr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lvgtshjb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2sztwyhxb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gxnkrocc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2lboadphi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2mbicccax.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jyduuzpi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cpiwzaxe.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tysaswgo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zmgnbgfm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mctlurrw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rdgylqpy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2igtbcgss.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gwwubexi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2haupkqyn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zaweufte.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ihuyvbal.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2jvcibdqm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yoalzsnm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2fukhimxs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nbqakshl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2hyujupyl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lltbflft.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2sdbvumqz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2vndhwvbd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2rjpvngcb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2sgbdrfry.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2bsqtooyb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mrnahulc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hglnvbym.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2trjudkdp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2rtzogniz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hlgxtosc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2msmvjlkr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nesbqsxq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2gdzgtrqm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xkcsfbcc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2mhrwmpsp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2jiujhvym.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2fvqvncbs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zfsezspg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ycdalcqd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2nwiujrdg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dqglhemk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2pyjavcws.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xcmfqnbi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2tolnllks.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2dbigxlad.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nlpyygxq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vfdgmfre.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zlscsmmw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2qtaifrkt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vbryavvb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2edyschas.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ktusmkin.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nyfknjiy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jcqfqofz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2acimyflt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2txdfchkg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ctsexbwo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yjmdfykh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2azywgpzr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qevcuugc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ibggvnit.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nrekdtty.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fcefvqxa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nhiaciin.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2srmdrujh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lryucjen.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2czpnhgke.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rsuueepa.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2pnenspup.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2twmqjxbo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2mgkyydko.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2dfqjfndn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2qiopgqnn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2rnhevleo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljdymkxy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lmkwhwbk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ckaoqgpr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vjzstfqw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2srzojifs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txahodup.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ybygeucm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xickxdil.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vcehwazr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2awazyatg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2uefyubfx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2nmruyhqa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2dzyyisfk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mflnrlup.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zbtdwscg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2lasvvarq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rughspys.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2srhsqutf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2klylmaqj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kwhnnoia.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hjokhbfd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2zusycjyx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2lhztctpr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fwifznwr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rrpcayhb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xbkkvhky.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2axrakntz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2goswrsgs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mfhctagz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jcblanrr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wnjjgpqa.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bdvsahqm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2idhtyjsy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2nrgfuvci.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2eqpjashs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2zyfudcav.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uurpirsg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ldhurywg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ujguszpa.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2jydzntze.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2eilsxkqb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2csnwjmeu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zabicjyj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2psdnbudq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pibxbsmq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2kjvjdwbq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nsypdhtd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2djwtymrz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2yfpewpek.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gylvdrfp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2maiqtqcq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kebmzsxx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2mytcqcej.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ddrcpdab.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gspvtlzg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lvhmerdi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2bukrbutu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qztidxgn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2azwtyzmq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wkzoohnc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ocowkmlc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2abodsvjc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ytgkqxhl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2lghfsfns.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2efnyyjit.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ktvzardi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2qlfbawoh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ymuawucc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2sictrtkp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2penwkash.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2cozxkmkc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ebahdxvm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qgiwbcmy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2yzgohker.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uffucsvx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2izugukzg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cyyugrob.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2gytxndqn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2lrqjzfsv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dduecrpn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jjrsfylg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mjisbigq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ifjezwzx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jpukezgo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2faecehwf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2phtgntqz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mkysaobd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jdpnzhbf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ypmopqgj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ecogakrf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2duwelsdm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rapnivgm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tzgapalt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mbbyphgz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ngoabrxy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fjkzgivg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2azwedsye.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fzmpjcdw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ppyponuz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2xfrrfcrf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fbcevyou.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2fbbagkjs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2kpetozag.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2kntyjmtp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bfsfamxn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rkrroyra.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nzyvgeml.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2faugyaum.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oqxjufby.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ksxxrpnl.html


<!-- 参考信息 -->