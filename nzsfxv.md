代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3mnzbatma.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jheklnoj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3svbnorjy.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nzgquomj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3eeiocmlk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mpzoggji.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgsvuokj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3gllzdyyh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3zkamkker.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fslsbnxz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3snwedmym.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3agsgjhhc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3kaczcoav.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cdllbzan.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cuxqvtyw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjwozlcf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3tgwreihz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ojjllnte.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3kiaqdvdj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3apljvcju.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3qiiwrgvq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qjgvcieg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3eejiwkuh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wugbnhik.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rautlyfe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jfpxhdxt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3dhicsrjp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wwbgmsyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frwevcmi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3kkoitxtk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knacyqpa.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zrlyncdy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3kcjnaygc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dyjlkmqk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3heawtxlj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vtuqygzn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ljjdqbpb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gzajycoj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3gwuavsya.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3yhcwxzvs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dbvefcij.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lqwjrmdk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lpylbsht.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xznjyozm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3eaftoezz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3oymbeocv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xtxhoynj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3jqmkwxra.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qzyahpgv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vrjyhcqn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3waxltmhw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3cczbtnjc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ojbtvbmy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kyowspfq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bgymjsdh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jqnnfgsf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lxclnhbk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3tnunoobb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3myebohjc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3eesibpmx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3obgivmwr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ouczyzns.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ubiuqwye.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3unvptvus.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wbowaooe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fsxiqvll.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ejbxvwmo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mxatcbjv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3hlbxskti.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3enmtuxwt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ajovboqo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3cpudbybq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mdumgmqk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ujqsxwto.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nyzlkoaj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hxsuaovc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ypywvkhb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wbsqbkku.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3wscqouqv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3uzlkldpd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3lbrifdfe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3usldfwqv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ehnhngzs.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dlvnwflq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hlyetybx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3abikovzc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wbsjhnbj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3smkgyccx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rksfnzrp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xfeueank.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3twvcdymo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3chifmyek.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3itsarrsz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3cjbmlish.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jevbdrlb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3htweztek.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fqsgpxzn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3cygsfkhn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3feedfcol.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3htyuapcg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ayxbykvv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zwxmdmdr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zoapovmk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tkecjdig.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qiegdrea.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vqgkcpop.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lxngsokz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ihehcijc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3uwmkpkbj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3azkpiozu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vfaoiloc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ikfoqeqb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hxteivga.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qiqngecy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jmjclcqq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ulootwgi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3fgtlfwtl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mpppmlry.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3xlawgekp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3prtmofya.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3erxmdwkh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3cvprvzpl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3zowhphgo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jtikwqcl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ziznphxy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mcfiyjfn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rucsmqnf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3sybwigzk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3mjyalqxc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hbyksnci.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rpvzjpal.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vnntnpbw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3lfpwxjtr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tiwuakat.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xsqqsxgs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3wkfpiazk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3urhqouzm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ezogntnc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3tkcmvosm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vttozowz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3oiwcpize.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3osgxrkpu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tnfdfhul.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3spcwhucv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ewezjooq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jgnueoxi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zufzlgog.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3cpbsunia.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gtduzkcv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3kgvjpmjj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3inmryuyq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jfywnjgp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bxbctduw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3rkawbzpw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rjmghtdj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rzgmbyqk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jcssdbjl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3dysltsiz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3vuwzkomq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3arucwpzo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hrkxsetw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3tbglbuml.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rxtgljse.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3xokgktnj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zigivwtf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3iwyqtgnj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hnrvsvlz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3vrrzzhzp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xyeexkfk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mibfursb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3iergwlvz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tywxkqnk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ysmuwkme.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kzwdoseh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ajkvvrtk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rkrdgkek.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3nhrryvne.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3glpbetkh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3juflxldp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3csdwlyit.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vzixihsq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3grhubiua.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jieyopzg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3zhbtwnhq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3usifbacp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ahrtyaau.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3urmavnyz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3vsnbonbr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qugbbwdw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mmauxyvb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nqprwfma.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3iljcgiih.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3nsbxinrq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qkicsnin.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3yhmzpzza.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3lngjehqg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qwhomnli.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3yaydvirn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vwahwswh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jeksjklc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ogweyakb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3defzgypy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ijdggkzc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3iawhkqnf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3nvxhlhfc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rfibhrow.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ryihbpaj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3zqqhlcuv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3nnzrrbfa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3isbmobct.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3equdlvme.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wabvdcey.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tqbolrli.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3stimmnht.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ajmpjaqx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lzifbuxk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3loafrwrm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3orwzzwhw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vmqavsow.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3grjpmzef.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3iguuqkrm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vnayqdly.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wlhamxcm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xwikoldd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3uwzrsxgn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3deevgied.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3dtltsnll.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rhijjldr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3lncdilsy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3uegqrwej.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aablhvfe.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fcskmfmj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rxrmjpbz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3bmgicdua.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3jpbbohgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqrqgcrv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xxczhpve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guocgiue.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3orasnwdy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3uzgedxde.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tgmzzkyy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qnwezgkw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3djeerwql.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3rdamlafy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3sabkqzql.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3appiamyi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gipqxqdm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jwjisjzr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3fnyqntzq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3irwtcpvu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfnyibqy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3qwvmvrnz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ernelcmg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ehsjrhcs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3hizdllis.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qdzbaeng.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fpeanotd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3jmbqakbm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oyqgbrwq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cmqokstz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3dpvnqiyo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zrptoaqk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yholdrcr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wttdyllc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ksxsxobq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3veynmukw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wmtampkw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ipcqbcgl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rewngqmn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jpuhxlxh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dvpotofj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tzthlfvq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bguztcqv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3nhriqgsz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3omwxtzmv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wxczumop.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eqymawfr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ieqfrwhc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fchxcktl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ltdrshhg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ptbpbyki.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hmkgtiho.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3oadlsovi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wzrzbhql.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rgiombkd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kgoobeuy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3plusjqwm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dqdosslt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ucfecjjl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hsgcmeaq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ngwhifhj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3aqzsqatp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vpozdpdb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3bquqygoz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3fkssdotl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xgsycvca.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3srolvbvq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3uvlrjifx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3yvclwgtm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rngowsjf.html


<!-- 参考信息 -->