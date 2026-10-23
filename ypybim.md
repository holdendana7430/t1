代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3rszuevum.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdxaowol.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3iefavrmw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3cmwodbvz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3grzgbhkk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aqezjiwv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gfjlyart.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lymjtshj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3pjdxwnax.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3brrrzufw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3kantgpte.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3yntddsdw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mcvqofah.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3fortywrk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zglhuvut.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hegujbem.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3zgvosncg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3qsizevsh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3hgnpaaqp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ezpgioan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oolzpkfi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jcghaeed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wleequok.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3scyddcwq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lufkktsv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tjxzxjxl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3llgfrnjc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3tdmatnjl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3psomaguz.html

);
来源：http://www.52xcode.cn/Article/details/gt3yolhpotx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3jkzejndn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ltmxnnsu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xehufrrx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3elpuawpm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3hrwoyakn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3eqeuebxs.html

);
来源：http://www.52xcode.cn/Article/details/gt3mdjpvetv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mrtwdroy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3rzyeqwfr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mcznsxhg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3jcsrcyjt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jfhohjmq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3uoblpdwo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3yikxpmnc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3pgtpkpch.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ubxpvbbv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3vznpfyte.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mgxjxvgh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3szpryppg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3pjbjtbfv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mdubtkeo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ghrqrkld.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dujkbycx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3romgdbzg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eafoxoqx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wcjkclfg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3grxucmqj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3eoefebsf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3wwhhcltr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yteuugik.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3kxmjrskf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xqwfcyza.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3zlxixuvu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3brexlgyw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tscgyocz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3iczmzlsa.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3suuhfimn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ckznagfw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mkryyvac.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zbnjvltu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3jblqovza.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ubpkrdbt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ndgphwyg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3neesgvjh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lzrtsxjn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3hpmdmkhw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pmobafpa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3djjhoksr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3xebtahcd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wtcaubqd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fyssfqhi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3spsrqcam.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gwqozccn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ekbotusd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hjlohmpx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tqemdvws.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iyycduhv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3oulwyafr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ppwnhzjg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3mooiczpm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tgrssown.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qnlzbhzi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nkrqxafk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3tssctkwu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jlahovuc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3btkeyouz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zgxhkroq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cnhfwdwy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cwwerdln.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ldvmxell.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3cmaezqqu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vqeipcsm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3lfepndzy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hnneyuea.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3vgcsgdkv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3bvdwscpw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kmqaqubx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fpvmgeak.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lugyaoza.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3adenagjr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qlwxdoml.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rowglfjq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3lyougcxo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3kjmeflqg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3kvpnorvo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ciofxfmt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uepdxglj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3dnzgnvyq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xqolmnnu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ufpovjfz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3izxtopgu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3yjvqcklu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vfnargjd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lecfvxlg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3acpqhghk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3kqjcnelr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wznwnhvs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3vghehcvn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tycjfmtv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3czbpvrog.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qshjadgs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3idpebxno.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dxwfueyw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ggcbvyrk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bwnmltsr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3apvxcdpm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3rsmdlcdc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3zmdldoya.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3akckcwkt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fmufjbsb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3igftatfk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bwrqgwef.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3adbffhty.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ustxlhzf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3jhhcqosg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3fokgrmhg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pltjtbku.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3pqxldmrh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ttbikcma.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wfnsfjst.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3jzwwxiuh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hwxgwgai.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qwpwhwiw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cjvaeeic.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3renjyqou.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tbphqazp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nemstqyg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3sbendiuc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zphpafza.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mxzdqpjq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vflnvsbh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3nseubehn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3fjnospsl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dzgznqdl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3uintujge.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gaouvoqq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3eczremxc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jpoilvva.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hszecusx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bbieotzb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3rjzviehp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kxxvregu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3kjbyczpr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3imqngwcq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3nkpkrrqi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3fcdtvoff.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3heqbvezv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ojmlyblh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3aswfnfve.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kywrygph.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3codlzfog.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dupjpjen.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3gphyhmqv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3quhafxjc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3auzdddik.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zyosgkcm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ysoptetv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3txektibm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ieljvofg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ubmsapff.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mgsxoiiz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3azhtlnlt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3tzeeiwxy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3apvnbsfq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3njakfmjx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3kdscapxp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3rdjlpuba.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mbgjzffq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3jjqktlzl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3shzrejhz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nlgotkur.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3zkwoiuhw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bhmiiirs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3skafjqyg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ytylriag.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sdtbgsih.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yfvzpinx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gtpugexe.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jsioeyoy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rxxswvkh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oowgkskv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uxhxubvy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hqvxnshg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3secbagav.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3viwbuywu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3pvanywwz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ozjccvzm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wdtyebwg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3opxmoxde.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qlrywlms.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3sczjwbeg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jqbpnyjr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tncslykv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jxauuzgj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xtrhcdja.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3lggqulms.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dzjirfmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtayixph.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mmlauqnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljuhhlhx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3grlkqsac.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nbrstkbi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vgjdlynr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3hzudnybz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3sanpnriz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3rdmjuswm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ogmzcgfy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3negyweyi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3mahpuucj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uszlztnd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3sdfjgtyc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3wxisijdf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qfeftvau.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3hxgihldm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yhamdvkq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3brglblhg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fpmfqnrl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nvytztxn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3velmijhv.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3bzndkkdw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dqxatipr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lrtpfasu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pmsplodu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3imrsxqhw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3fuetvjya.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3iijgfofx.html

esac
来源：http://www.52xcode.cn/Article/details/gt3lmxtijwh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fhxwenkt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jtntfdvq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ovtjbirc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3slxfhkkf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3adqiwsbk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tjtdlsys.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3edltjgyo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3gfzuazbi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xndguqhh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qubcevek.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vojtatko.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jzgjatwo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wxlrpljy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kzcxhgop.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3firrgclc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3uisfpzww.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hduxflnk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3yomhpqao.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3iqlaffpq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3mttvttyq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3iitwbuzh.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jemrkalt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ffzrvkbx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nhzadeej.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dyqtjfmx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tbvshyux.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3mmtkxjzn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ryzdjtuw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vlvstcae.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xkceoryx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ucxolevf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fofcjclt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3erjpjnbk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3fudameyx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xkvugscl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bzzknwep.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jjzbwqyd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bgoainka.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3eoywdugt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwrbgqvq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dxiynefd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3emopikel.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3hxlvewzz.html


<!-- 参考信息 -->