代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3pfflhbcr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mubihybb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tcexjdmo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jbjymqli.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3veskeeju.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3trpkcunj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3oijibybt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3glvkfwch.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wxswymxg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jmlpxvuc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3kzbamaom.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vmnelycl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3troqefdi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3brfyazxx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ddhhyrhw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3efwgwefj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ddfewzki.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3lqlhlbhe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3xjffcgzi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zhvwfdag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnojqohg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3sfcjssdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exbncqyh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ovmqbkcg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3agiiokao.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ewozbcic.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bqminbos.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ucddzppu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3sfbeaqou.html

);
来源：http://www.52xcode.cn/Article/details/gt3mrnwzljv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ekxdjzbr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3exsqxtsc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uksvmybj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3oaylxibz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3igqpbnaw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qktukncd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kyvzkfmq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3npenuoaz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3orufvxsl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bnuzqwlg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gvbmlapy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3peggvlen.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vckhdazy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ugchvxam.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3elkfxtqe.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3alfbvhvd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zrbllhge.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3hwawiyrr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gehfoabo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wgvrcvat.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3uzdackmk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3bydyawkj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3recwzwuk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vmsoayea.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dcildwma.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3gchgfgwp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3usatoymi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3dgjhnfrz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3rccpnthu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sxrznozn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3htefjxtg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3afnbbpni.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qvwqcrzh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rhzsipuq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lebyxltq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3fwjzixkx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ajgvajsa.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hkxpswjy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dccrujoa.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ybbtzdcx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3cjesorzb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3mibewdrw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3nlcylkvk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eunvydgt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3flziddky.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3untlqosd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3stefjadn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vdhrvqnc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3yxoknasy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3zfwtaoqk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3vvevqcny.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3wghzkwqv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvajqfzn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3demovydf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vvwplxqs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3rnjarhzj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vjdfrhjx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3brrchrzs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hzqgczmj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zmhqhmfr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xakggpso.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zikpxapp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aodqbjez.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3uldnixfr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3czljxdkh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3xhygtjrh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ldzonoov.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jfucbveh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3suwplpat.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3anrnwjov.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fbjsylht.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qrldtbba.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3mlxqkjch.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rabdbwkh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3pmwxmzos.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jqgyaivx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3qxtlisyw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pdqgulud.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3zhcagdoh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zqcpetzb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fqsugjrk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3picxdxwr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gyeramno.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3erctkxsx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3nfwzmdhb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3uvponrwp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rwkmthjr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wsaledun.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3srvvfbwv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qtnmevug.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zedjepna.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pjgkbmaf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kbmjsvqr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ealuotyf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3nemppljj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ruussmyr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tsgfpggh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3edshhlvl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bpeuuvuq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3jxvfrgzl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3waacfqyn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zojmpeej.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3luempiae.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uugqpmbc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kmuwxcvu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xhlnrknm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3udsmolpc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qilswkva.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vqwslsdm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qaiderhb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3acypztmm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wpntuald.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wmsdkcyc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3lrrubkjj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kxvlipvh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3skvrzuag.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tfciezwb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3pjdeabor.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mntxzlho.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3azpmdvcv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3wxnqeajo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jjuokcti.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xlzckgrd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kgsdoyfn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3eflbvhle.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3lynrzetl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kpbmwago.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3gucuchtz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bbkgkdeb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3utxgfvvt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qbwdvwwi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3yxqlpihk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3slhptrvy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uzlezndm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ttllbagq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iulncqse.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3bujhzpng.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zovqopxa.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jufrtmnq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3phivlqjd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mrdhjifu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3pkqsqush.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3trowvsxv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ozzuoloe.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3tfplhbgf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3fbpsxqel.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yjpbuiwf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3qerlnrks.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xtxwtgug.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3fvktnqsl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3xupesubt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3tomzgtal.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3zxzmnwpd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3zkgojzka.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3lbpdgemz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3njiklttl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3guffykar.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3izlrmeit.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zixauwpl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xyxcnjpe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jitpljcb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gjpeyshd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hvjngzlt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3eyhfygcj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zpohmurx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nqhvrpah.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3nqiuqtje.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vljfjkdq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3toehnwtj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mqtwudbc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wvrqegzm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3bicpwhft.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3trsapunj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3azerdcsl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3obnuhksc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lfzekuzq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xfrqpckb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ltqeyski.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rrwemsws.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ckkktctg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mgomyefa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qdzbyylp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wrrsteen.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tlvrtrtc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ficjyefx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3lgqfiblr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3kqpjgdrp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3rxcukeeo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hivdveei.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ibyhblag.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3aeycxvuy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3rjqlgvan.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pwfjqntg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gihqlgyp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ncikdfyq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3xxjmjhlz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ezutptud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqrdxgrj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lnnowxul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fewsocof.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zsdajfed.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xvqleglm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3xeonmrgd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3getdfwwi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3cyxjrsch.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3sraoiyat.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kcnykosu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3hcvqxjbj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3rchunexo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hhhqxvro.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3nvwgyxrh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3plrimkoz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxoxseas.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rnzvuena.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xgigtxjs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ausnykwc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gfmespeg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3orlvbumz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3dmwwjilo.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3iisvmmew.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3oemuytne.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3bgomweki.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gomxicoq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3tlusteco.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lzchwgzu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jxisgxgu.html

esac
来源：http://www.52xcode.cn/Article/details/gt3rncbsgkk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3inkluscx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3idvcsqns.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3njfwocoy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bxqztxcg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bqzbcjvp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3npeqxotu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ymapsuoc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ztgnkidn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xuzdduxb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gqwetzwu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hznxmgzc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jdmmkuik.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3mwrfqocv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3btgvmngg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mrmrcysn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3twwwjauj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3txrjqnuk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wtlvgdoz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gumqursc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rgifpymn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mlbtoplt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hhtvodyo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rxxlzvow.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vzwwyklx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dzvberzo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mquacjlg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rhtltbsc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3cywhupkl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3svkzkcgn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fdmjnfkj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jlzohhsv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3tuvbmzin.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3tgoehmhn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xqelbkrj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ndojzuez.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3excuxmka.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3welaqggb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kepiygwq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gmaehgsl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvymqfoh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dbqyzgam.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljatfdhf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vfilyhde.html


<!-- 参考信息 -->