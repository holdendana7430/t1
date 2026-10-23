代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3oertzylq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ikezopkv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qfmjsxxy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xvoohpbp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3pqjuybsc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3hipdmrch.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3rsfhsbjg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ocozqbgv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dwofmtzv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3edvdqump.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ikdhmiqc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3txnopmms.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mokzfrfy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3pkxkvaii.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3qnlayrsg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hsfpxhir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzykvugj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3buveebem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrxzmfkv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3foehlhno.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3zqtmrpxs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3asebawse.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uiximkgn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3odphdlwj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3tusjklkv.html

);
来源：http://www.52xcode.cn/Article/details/gt3zztrtkze.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3mogdwopo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3awfxloos.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3oeqmnrvy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fuhdximq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ivmpnfoh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3aovcgntr.html

);
来源：http://www.52xcode.cn/Article/details/gt3tcpcegrq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3dutgqkuv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ecfxyixs.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rjdshidv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fgmgrtht.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3yivzumwm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3etijocuk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3irhqqier.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3iofqormy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mquvlqfn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bwktroau.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qsgykzhv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vlzttjyz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3jtnfrcmc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yzwknbpj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3bsrffdqo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3opeesven.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ykdfboxw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3riisjihd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3qzlzqkfe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3bczzblmw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3mdgdqagj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3uwgfhnuf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xmuzekum.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3itduonym.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3evbbrdey.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jfzcttbh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3abfmgumj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aiyepkmc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3uznvqyrm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hylptpgl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3lvjwigke.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ayaifoiy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iuzqqpxb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3yajyqkcp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3qrmurrkb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3slavdimz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vubyziqh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fehbxncv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ytodctui.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ampxxpey.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3gjhuxxlf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3kvnvayyb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ugvgitcc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3myqozdtb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pnjdhlzh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tlamwknw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3orkdetvs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3viowywwu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bgkdalsg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3saamisdl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3hsbktdse.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zrifvjoi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3siyqdpwv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zohmyfkf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ywvattqs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cuqtgoug.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3aagiuqeg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fwqozfef.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3nuugupry.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3avlhwrfr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dbiddryr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3emsaesom.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zivrjfgu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3icrjnsrx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zreuzgei.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3covukzzn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vhozjixs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3gwntvggu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lnpijypd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3teptkmwf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dqloglxh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hrazitoq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3oeyhqsro.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jnpnvzjx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hjulrjpt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jskaybau.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oloxutrn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jnrtgjsz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zbvwxnvg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rxrbxzli.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xggkohfr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3oblszmfx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3moveytkk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3mzpdrrge.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3jnzgrtui.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xjjmbwqy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qntclzda.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zrrpwlhh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3kvmdkeaf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3dlsmoisp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3vsfnnrjp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3khsglzsp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3lczidpzf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ahibswsm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3evswmqeo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3onllkptf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jcladjrh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xvdbqwjr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3omlvzlfa.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hcggdavk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3egdyiaen.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lxftrclc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3kvdgivli.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cghtxcgy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3blekbqxf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3orgswwbl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3rdfzzidd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mdpgszua.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3iaxoicve.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vsopzfqj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zsxbozcl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kkugbfkr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3szlegwfz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3zffscrej.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hryzmimn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3cztnfbhr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bkiqjjku.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rjqhbbik.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3uwulqstc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kielnuxk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ectzbhyh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mrapmvhu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qcwyivtq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3njmnoujt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3lozbcece.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3biktsexj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3awwihcpt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3mtymujfz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sbulciqv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3nijvldly.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wgbftmgx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3yeldlkaa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qvteiztl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qulhpofj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ywgocjvx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3rhsmkzdg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3uzstjibh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3giqgghod.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3thdjgepk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bdqkilhz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hifqhdnm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3favcluia.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jdpwcpmc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ujlorcut.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ozoaxmam.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3uivjvmet.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bjtuuzts.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fqoqofku.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3imnlphod.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3cvqmzbqe.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3svoqywlq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3umgakgsx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3supsusyz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ylhyycgi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ofwkheny.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3pkeswlea.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3prwferqt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tawbbhtp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jrzuyvah.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3cshsnfpf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3syrzhbey.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3rgzvduia.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tiohrbkb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3fkealfqi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3isiqbapf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xthzwyds.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3asmdszav.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3bhowgdxf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fakvgqga.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rdujthcj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3istpeduq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vsxyundv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mpfuedot.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vsmadmjf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mbbwnpbm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3qmarrxpb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wcqntris.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3bjprnaff.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3buerlfcf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3iwxawkiv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hwpvxmbs.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3syjrtuak.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ximzidem.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3pgmxsrno.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bqlwaifq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hvyaozcv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3hgcjdsey.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3vuivuomv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3cabjyydi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fwkjfxod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwhbephq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3sujrhxxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hghlyirk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gevamgja.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gwbstuts.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3pshjadtg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3oihzsekf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3wzqlxwab.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3tfmfxttr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hhdooxlk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3zoxcrffw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3oeuenqmg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tnzrllbt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3tkkbheaz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zjmuqikn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xoiocqis.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3bpcnyrqg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ggeakchj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ymfgxtds.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3udwynvqw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wlhygwnx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3npssqpzu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3thhqvggw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3kfmwexil.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vtqfivgr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ceqqfysu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3olcbjdfg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3zyvwvjrv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vrgcbuto.html

esac
来源：http://www.52xcode.cn/Article/details/gt3slfshijs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3yeuiwvxz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3euzvzjrh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dmkyyzhv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ducdvbgj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3rjlvrdoo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ikemwpjp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3offklwft.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3djevhpjo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3htmuemej.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mgjzvxhq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3dmudtbjl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3mhbefttz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vhveklpv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3whpsvrxc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oyigvtvu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3foablcsf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3jmnumyso.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qhhwrsvi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ljafghpa.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jlacufyq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3munkkgxc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3odllvkbk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gznorbza.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gbydztiw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3porjlolu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3nkpfkigi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3dmhqkhfy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qqremctv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3bmstiipe.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3kvloetgm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3wggtfpvi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3mmssfsnc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qbsiujpi.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dknxeuzc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fnnxjixd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3sznlwpjg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hdkojeew.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fehcmzxn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3agtjwuez.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdjvtqzy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3gzjloiyo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzhnnije.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pafcfljx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tcfuchfc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3odxzklir.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kvosztjl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3cxaopshv.html


<!-- 参考信息 -->