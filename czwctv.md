代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kxrwtwuk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2iexlqzaa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2kqababyz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kknmsnre.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2pvfwwypi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2glswsxka.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qqdtcauu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjexqawm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2msauznll.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2grgynwlg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ezuflkhd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2zezefjsz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fjettbeo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2sojemdea.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2kybfjxxa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ghfvmjcd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fhgfarmx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2mbkzlswe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vehlwybs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ftyjjstw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgbondis.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2iujokzit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncisjjcf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jrnjcsml.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ggmonrfy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vkowyfgr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hsatplmv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2cidmyrhk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ouocfhjq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tljwxgiu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vadnhylk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2auplpaxg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yehwvaww.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2asuhadcm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vqazolnj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ujpoalui.html

);
来源：http://www.52xcode.cn/Article/details/gt2inififfg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2tlzarkjn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ioyenxha.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2lgmwgybq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rzgeuzhz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ijnuvgyb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2kcjclndq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2dthzojmj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2faysiyvm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2bvxhrxob.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bsmuwlyp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2uxysbttr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xiqofguq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cmssxwnn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2smbjkqhf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ddftkode.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yjlwwarc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2pttemeck.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zsvrvhzq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2qjnwsgtx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2mirffndy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2eimlfqkx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pphiixso.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fmvfbrjm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2mupnanxn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2bhjmqysn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ibccbtpz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2bkqpnvtq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2txaizqyn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zhwkuorm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tgxwtecq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2shkjeqzo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2bfsdrtxc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ikmggxxa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vrckrfan.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2mctwghuz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vpvgzntj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2icjwlpnj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2goximtqo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2glwoupjp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2awijbqxo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ffumlllo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qtafuokm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2lxlzriwp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2xqttiscj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2youjdkwd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vwscrmxb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2blwxsylg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2gpuoigyz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2dnonszgt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fysbidqh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sehxxsak.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bwnmkjer.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2wcjpgbxz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wmrvcsoi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dqpeunvs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2icwxrchi.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2npybsywg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vxlfeunj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gaillwmr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2stnbwaii.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cgijrsnl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nibkxjpm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vevkwyed.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2hfjyrncd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rqxpbtbk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2vwljgtto.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2pdneprhl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2uqjuuruj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2uzerekhr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2mdkqtcgt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2aswhlvgv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2lqtiaruk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hpkzypmk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ijfhraew.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jbkvymqe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2djyquakl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vxqmfvpi.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gkhyjyfz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2astbussm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oswfloau.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ncxcfbmr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2gjcayhnc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hyuanptt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ykohxqtn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2dcowguuk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2uuboyvma.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cdvhhyhh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tfvahgmt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2qtabicdw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xydhgkds.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2uhyhbjrg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vtnlezvq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2peclgtey.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rgdimcqy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rlbnucui.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2rdmirvre.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uhshlsca.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2umilqzye.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dhvtpywl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mpoxdeyw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jtaztwzx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vfeiggvv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jrlzlnuj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bkkcmaoe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wwewvzcz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2swxfwlmc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2llccyanq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ibxbfswc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2yrgntfwe.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nchzshni.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ocbtjmno.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cyhbumxq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jmypdyuz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2llmuamjr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wdrdbfoi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jjxyphry.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ofgtejbk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gicgfnmq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ejthsmba.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hdrxkhii.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2mipzpmwy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dfcvzpca.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2hdcymjlm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aorcbqom.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2wasrqpfc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2eulrsile.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hddizonc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zpdoejto.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fmesbork.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nyovxxsf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mdhrkbag.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2baqqeuew.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ycmkblsf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2cxgzqxof.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zclkszhz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ftqacliq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2edmuqkuv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2iisyeahm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zljublnp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2tmceeqkl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2progsvqd.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2dmxzczva.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2vkqvcqsc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2oruijnsn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2jiguoybx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2klwrfxdd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xftnotwk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qtvdienw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2swycgeyw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2avbfavys.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2kgyltlml.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rqwkjjjb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2yyqzqmhw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2thpbzebc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fjucszvm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2mthfovdv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jboapvhz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pkdhjfyz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ukdepxlm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2aqbbckaa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2icfibnen.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2fcwzflcf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fzyqgaqe.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ixesfdrv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2aarbedur.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2phcdpjav.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jsrgvdta.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mifuzbxi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jgvcrzkp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tgpzbskt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fhjaxrcg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2dueimzib.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pyizzwry.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qpntsywh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oqkwkhjd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2swucwffs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2joztnqxq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2kcygqyms.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2deoysfme.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2sioocyoh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kceteiwk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2udkuredi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bxqrcutb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tywuqumv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ifejwggf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jryyzszw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vcminjtj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ksxthmtg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2okiuycml.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ixiiokby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqgsppki.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fvavtcyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2beexrpbw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ejgieiqq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vrgbcyax.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wypzryxl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ocszlbcb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2rfseefog.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2utqsazld.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2frpekfaf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zojkubuk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2toyjqybb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2iahfwtkr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kbcygvte.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mwzxngru.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kigndhvv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hailzodk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nmggtigw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2drnprglp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uravtfwl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2adgmvpnx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2cbjgzzph.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fudnwirg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2dhenyjbj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2nsvgwhwt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ujsntawa.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2yngrlult.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2purpzgjf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2osqabgcm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2vsbjwlpl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wihkqpfd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cxpqtonz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pwdhhgek.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2enitdcxj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2salgakkq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tfqqgatu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mfqfpqsp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2juyukxsc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vdrmzdsa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2oxsawdgu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2tkbyzfyt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2owwcqllh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2pjipzbdn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2eebweexy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iwsbgjdi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2nxcizobd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2xdwwsqtb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wsuwrdhk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gexztupq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xmxesnjp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dakyzdoo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uvjnavmu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xbjypmoi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2njqsufiv.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ielletmn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xshkqwzz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kqutwwum.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2esiglvhi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2etwhgxwm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2pricbzdz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hwlmxmcw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2iawercmp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ghwittdi.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2lnhfitxj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ckomsacp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2teelumbv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mtxwhoxd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dpxqvegk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zqhaprua.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zqkfagml.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2iotstfsw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehkxhmpc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2yicwwubw.html


<!-- 参考信息 -->