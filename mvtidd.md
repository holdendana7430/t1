代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3wwkhuyrz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3watcsegc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3trcczqye.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pplxbjsl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3rpbbaudj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uoyonszi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pgzjzeyn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbpprvyk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vfmifnop.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3hmlyjiix.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3znbfgobr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ihefvdwf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3vwqrmjqg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sxjgxplb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yzfrailw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlbrsvwv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3btpegsgw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vnaejuny.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3meqxcjwk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3axaiolia.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3lrprlqsl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3grtazxeq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vymqvrtr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3glhmwnzc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3bfhmapjo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tehyphjh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3afhfurvz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hhcwiuoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcqhhoqg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zfayktmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwhugqqw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3itcjaauk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3uoiqopkh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jwiclszx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jgxpixmi.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3kgrdtmlm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3sirkhecm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tusqsbgd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3sgexywnx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3kodaumlt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xijwgpoo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3eoiimqrl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3lttvqogn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3makrhgtn.html

);
来源：http://www.52xcode.cn/Article/details/gt3pmfvdgae.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3lcypmkec.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ycyztvcg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3evufozte.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3paoxrkhm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3nzecjfbl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3dqiaunyl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kfseilcn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bxozhexz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3iugobfgq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3enutcvip.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3vlzeadst.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rctbtsvh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ojpaaeac.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3raxowwxs.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3aqjmjkhb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iuyxmxjw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zmymxldg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dudpppdl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3muknhgci.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3rmkyauyg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3nahwzvpj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3zhgzlcyj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lerdycbf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qlmbhvsx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3afrthmgc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3zbqswmvl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wseggqvd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uwvmjwpg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3pxtkpcfr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3quqbybak.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hgbmpvsb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3hegxvlee.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ypqfsxeg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3knhkjghg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3udntlcux.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3hdaasdlx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vucsdhpk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3xnqmjgxp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kedjkfpo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jcxpschq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3czuknnoz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3gjnxtoqu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3eyfmvvmk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vcdjlwbn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rtiqlguc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nduurksw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ufqychfh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mvopbrdu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3zxdgumei.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3apjgecob.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3hgfaozuz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nzgdthym.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3yxmsvkqv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wbyozdlr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3uscszpkf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xqehwoop.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bgkttzkx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vdtzpgxv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3eoemgked.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gtdszrxs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mzfjamgw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tfucphvy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3tmnynuds.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ewuedqnw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3mupmnghw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3oesdeajk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3pzxxfunb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nejovpny.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fsiwhazb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3gqasuhog.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bucnhffb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ecrpbkmi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kziyruqo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zhrvtodo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3borvjdrx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3vwirupig.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3dckmxihc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3xiwqzigh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3bjeegbmo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hnxrcjlp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3fzbjfwms.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3yfvzvmhn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3uejfrney.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qbxcpgat.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qxayuyue.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qzztxlsw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vxvleeoc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rsdyecoq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3imtemsvy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qaobsxrf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3itwnfyij.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3nulnpbjq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qeebvzvt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3myiodypz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yamvrgar.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dhzddpsw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xmnygojz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cqjnvwjf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rnjiulwx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wawppnzm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3dhivynqt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3msdfapde.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zoebcgzn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wziquydr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3stphbmwg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rmvffqyo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qhaztdwy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tltbbxxv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3svmyhkhu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3digphhbc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jgbmciag.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nynmatni.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3toahtqxu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3yhjbmlxx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bhdwdevc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jgxldkrt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3moppcsbo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3edwxyvjw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3eqzuekfy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3laagyoxp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zdimuvtj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eivwgggg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ubqaaioe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fqsraofb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xeojpulr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vakvjqvm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bvgwggpn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3yexpjxne.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hqomihbr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3cfpqturt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3turdjivh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qrutuyts.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3pmfmypqb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3cbfjtija.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ryuuagta.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3sncsuema.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xzelctgo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jhtovkqp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3nwgieela.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hlfsdtah.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lrzbdybu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3yfdtuzea.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3eyoxdvtk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3hiryakxf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3paqqyklf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ntvslywu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3iojowgms.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zhdqpvwr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3heegfdsz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3rplxebyr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zyjyachr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kzxgebrd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3emeluuwa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tjuwvvub.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3bdrzxvwd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wjkkhjae.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lpgpgfxj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vwldfffz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fdyffyoq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3etkiynkc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3npjxctzk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fhvybaik.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3nqybkvbh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3psrrkvmo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ntmbywas.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fbdudyvv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wlcawcro.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bpfhkohg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3soobryhw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mngfkayc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ktxhblxd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jfiqhkqx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sijeemkx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uqlirzes.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cvezuuaq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3fghkshaf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wqdabjfg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bodxadsf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rkwleaoa.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jcyepsfk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3volllxic.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zrvszzwd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tflnadva.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zhluzgqm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3cezevitm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cewtkqpb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3lrfzrnhk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3oyejzeqp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zkksfwrr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3yrxssrwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkejqexn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cjgrohfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwnqepkp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3igjgvwpr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pfqsahju.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ekjujitf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3pcdzvmfv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3nesjlvmv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3yrydljxh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3lotejsga.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3idlphlvu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3odvuwmbd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kopqsdht.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3fakbcoxi.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wmshrzvr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3twfzhrgd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3faoqtbgm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dgmprodg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3qpvsvpmu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3abagymse.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ptbnxjum.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ixyycuxo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rsnizlis.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zvmdxznu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3dpjfzbsz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ukvifudm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3awytwfde.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qbannpkk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fgrulehf.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dypsweep.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3fbtekbvj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3kmanrqao.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yqwnugee.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nteikicp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ztvyzafy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vxrqlqvr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fmxhgcin.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ipyisatj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qyrdlwhe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pvoqfsjt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xaigwwxy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vadvlnsu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3cgtqnhyd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3bfeutuuy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3havvfobh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3syjuotde.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3oohgxfgl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jxzmlelg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lodpteoy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jkpnbplt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lfemzgty.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ermikkrk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3glkdtdbd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qqfxskjy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pbcbgpzy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nuatgpec.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mgbvmytr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3nuuwjjuj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3hluvtxdb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jzaohuxl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3yedqjnbe.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gxgngshq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gedxqcst.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3clgxaqpf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vhpmritn.html


<!-- 参考信息 -->