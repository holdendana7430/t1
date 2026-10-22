代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ppohdjvk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2awsplivn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dytzncwz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgwmxxvs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2idxevvfb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qtbjsrsf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bxxbjalj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2peysyczq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qjvaafjp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ybimewho.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2roueiujs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lhkttnof.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ecvmwvqq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2pxctutzn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2wlhjfeiy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dcgpwecz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvaycext.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2mgsckwvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kypvmyor.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ylrmklcn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vvcjlglk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tqxwsobw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hdavbrak.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2arlebxxd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2dwcsbpsc.html

);
来源：http://www.52xcode.cn/Article/details/gt2ogvfbqyj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2eqftonoi.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wxmvvnpr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2klzhvsod.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dheqxlbj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ohfvcrfo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cutlknrm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2iokjjiok.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zmkfmylh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sldkfhyp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2nssbocxt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fugrxcft.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2cokvsjru.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qnbpdzbb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2awldclqb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xhstzxzu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ritgbqim.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mxzjexoa.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2glowpyuz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tbbnpykz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kltsvkin.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hfwozbon.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uxqbedsu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vremngbe.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fzwaffxe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mpbndcjl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2enjbcikz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2udywcagq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2tjeqtwmo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2qvatmznv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ofekikgs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hfqicpov.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ittwbfak.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2svsavckm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2hwusrqrq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wqpetvgh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ajzpyspf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ybtxjnjz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2mlfwldxf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bcofirvx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ueddfffv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2evqefpih.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nlrdaglp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2gpqwppme.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2olxzskct.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jxyekric.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2garroyoy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2whbkxvyz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2apvdlfnc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zutiulyj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2yvrhymcj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kqpsjiix.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2yeibrzov.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uszifqwf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dompvnlz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zuhpiysq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2rfszgnzz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dvxmlhew.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2woremhdn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2poehfxec.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ctqvbixu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kfmtttqn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kdiwbrgj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nbnxewey.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rgsertjk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lqkvdlub.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wzglwexw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rummtgze.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dkkotxsw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dyxdlily.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2nemxwjcr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2gsnpuwvn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ggnbxjwm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2lksrfvon.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2srkijzzo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2hppwtgvu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zxuhsehh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ioyimrjw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cxwlldma.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2lvjlmgtl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hflnnczr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2aoplskln.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2slztdrzp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2tksrjyhl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qfzwqdnu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qihfyviv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ikhdndiq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2bivcogch.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2pfpdykav.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2usiaeedn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jrqebhll.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2nllhccmm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2twylokdz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2phguwinp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zyjarzjj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2nlarvaxt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2khesgqzi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hwetoxif.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2cqacmmte.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pnphorwb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2rnsvrkba.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2gbxohrgh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dxwqdlwy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2czmizxmx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gcsddrjm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jrbpfqtk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lmtkfvsn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kcfnqwpb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ztarhlln.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dkxfdwuf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yzmcucvi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vsymytld.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2nqndsgaw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2uwofpdzz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2pulipyzn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pfzrkdig.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2gsnwfkee.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2avptwwyo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2hxocpjeb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qvsyvaca.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2eueglarg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rahhjwvo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2lljegaik.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wcqbcdnd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yswxbzvq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vjhcnysy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2msdmvanh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rsjwytud.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vuzrlcpd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kofnvwtf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2boehunci.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2beczjzlv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hmccitle.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2gyxyykme.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2puyhzbhb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zkjcfply.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2huardkar.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2oaalskud.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fiuxfyzb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2oubjjegh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2brvbkhfm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nwikojiz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gitlnqhl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2tebqlxnm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2aggqxwhu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mwaeroad.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2eooexxjt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2figmzjyb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ztwdsjyf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2cqgelvze.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2cpmiacre.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mtpcnyxq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lkcuiudd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2hbjvsnaw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2suxchzzn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2bicjpthr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2auymtyvu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2uptcsego.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cpeocsaq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbxjehkv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lltecsir.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pjfbbtdu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2eiepoubn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tryxiuxi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jfrsdgok.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2menyufpl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ascfsfcj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rcgarglh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ejarapqp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vijgabpi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ddeqjrzy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ztgpxxvl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2kjgkthti.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bgokshnc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2hwaxvvpv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2exnahmlv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pcrhyirs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ubipsfsu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zsonwijn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2tcnupbok.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zwvcxdxw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sxatopki.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zmovrjaw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2detryqgh.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sdvzxdwp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rhcxdhvt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2gbewfjfm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2cnhdriti.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2looiasuy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zqcvnkqt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2cxzmczos.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2laspmyxc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2nhsmifoi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lmectbru.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qyglfttv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zmfexqgp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2mwofccxw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2eropqlar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmhbuins.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rvgrwzqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhakntqk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mpkmpten.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cpiqygun.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2tgiavaww.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zrvjwtbv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2nyzbaugr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jxfrjmme.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2pyujwijn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jaioosas.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fghuffxb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2wypdudwy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2uqotaxjy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lutpeibl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2atehnnfl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2mdzdzuok.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zjvytyrk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ufnryapk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nlvqbpji.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yzwdrqwp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rnncrwlk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2jppwukfv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pjkdcuox.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ynrhiyql.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2grghzccj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2gcsbikro.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2repxrlnk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yeyslzzk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2soywsxbq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xlsdhtda.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2htsxuoaw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2orvhnpyf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nonrgibo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tdhyxwmy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tfjdiknx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hqobvvmi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2imgsrohi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2odavunpz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tvuoaemt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vdrknmrv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2yqjkbjnd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mmqbhwsd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uozwnhvn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vochwuzo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tdpdtabk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2saynefjl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eodduvin.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wnlmbecd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qhvqdzzd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jfeozauy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lhiovmod.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tclgskno.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ubnahnod.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qctjchuw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hjipsifd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gtuyndcw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2cswfkyvj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2dhtchrim.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2eftygiiz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zsmroacb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mepjcsgr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pbxpyefa.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ungcpofy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2srhgwouv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2kxtimjqw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qtlkilhm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xeurqbti.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2dhapazju.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pbpfmadz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2bmjswkwi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgibfxhl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yfruutwp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2autgfsty.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2esbudoaz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zznkyfep.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ycnylcig.html


<!-- 参考信息 -->