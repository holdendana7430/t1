代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gwnuvmuz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2akwifwgj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2amgwyong.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqemoysz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2cstkmpqm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rblwslxo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2hachrniw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2zejfbwdj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2mfdcxatx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xxydjwxy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2gpzkserm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ugcuyfoe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vteyoweg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2xmpyoeea.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2tizpahjc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ofxoxjvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nltjmrbv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2luxfexne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccwziebw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2oexahoft.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2rniwddxk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cdmzeluc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xyiijkqo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2jwcpshmt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2anjhvdig.html

);
来源：http://www.52xcode.cn/Article/details/gt2ookubxxb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2wtlqqwpj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2uyepmbbx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tdejzjth.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2cdvekyzu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2qclpozxz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2eokiwdrr.html

);
来源：http://www.52xcode.cn/Article/details/gt2kltoxwse.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2cxtyuocu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ipgijkha.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zxbzjrgm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2aviuzufk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ymngrpje.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2biqhijbw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2iflbyled.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2yavefwwm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qypubwnp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fjmncsti.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wqwkqhbk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mczjcitt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2mvbmwfdx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mifscjot.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2enbdugaz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oiczvgpw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2uitrzimk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jslyxmfn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rwzdzesr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2iqtfyahy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lvcbacea.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bgltggnf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cqwcxhck.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nxmwcfmg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2avlcwatg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2gjznyvto.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dnqpcviz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qdrldtiv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2kfmuqdtf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gehbtkiv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2vtzbnmkq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zhydesid.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2nbonxiuj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hqmxiwdf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gijdibua.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2gnzrqmwm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zqblybgd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tpctzfkd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ldrnhsmh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2fweanjuh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2vcjtxqqj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2acdgdhwt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hhjpecuz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2fxuzwmut.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ewbnrgju.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hycggkvz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rlmpozst.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2idwodmgq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lnpogefc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2olnmvkhb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ltjlqcya.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rtfajsjp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2aqdqkcus.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rqimcvms.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fxoteehk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ibftrkko.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gyfogpll.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rrnlflwc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yfdxeugp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rwjmntsv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uwoicsuv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fioicsin.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2dfdbsnbt.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2toyhwllh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ennghtkv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2mikjsurv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fbynnduh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ytsexryu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qqgxxhrv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bxovyknc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xcjrrwus.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xbrzbssi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mcrkmwaj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2biucdeli.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vaoxrmwc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xuerdvmd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ehhrrlfq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2fbdhanyy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2yxdurtpt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cmtrpgvo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2whurdjja.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2anreilfd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dypycrer.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2teajlwrl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2cpcdcuqy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2plmpvypg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2cynaosml.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rfatluzu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2aqdfdxth.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uqetvppv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2catvcple.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dlrcdnyn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2vbjxtusg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2egygnodd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hqbjaoht.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ihcjfpjn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mmfptmdh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vxqisqlg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2yhzjgbpv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2winekeld.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2tuupghuy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ddbrzbyt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2makqcotv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ykviyixz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vqbbfatd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qnggitpo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2oocrlqik.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hvfprlrr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2nmrfcgwl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kjykvavc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2qhkzqnkk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2andfxmoi.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2vqsmrioy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2hyukqtfu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ncqdgygw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wnvfheaq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2nebncvrz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wuyphdbl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2lioukcnl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eqqdcxwa.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xfnlzbse.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nhxaelwd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2qiuhuoye.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xjblcmte.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zhzymvde.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ecvaojdv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nhpyjxhx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xnjekrqz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tkwkbxhq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hdbcztbc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2icvzrubp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2qkubccbs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2lqmypfoq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hphdlyet.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2iyxsgdad.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2injpjzxk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ziwjertc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2mhjygmgr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nefrmdvi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2fvtpjvmt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2moqthfin.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2mlydqqqs.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kofralnp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2sydeuljc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pfeeijmy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2eulgbkhh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2qzgbawyj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2gmsrpndx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2mdkvaolr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2unzuupeb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2gjndyitn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jhkhdoxn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tslsgnet.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ujwlbabg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nxdezont.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bbwcpwsm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dwepkyqt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mbwhdsqd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2baxbwvgx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wyotvcpu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2pssghflh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2whpiocmk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2tjvtkyau.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ingcstgf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2wizjojyp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cwraoqqj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2motvhwra.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2pqvptyuq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rmdlsflj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gkhvvsjd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wzcqclsk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lzdngphd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qtogumyv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rwompque.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bmrnjalw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2znepjfya.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oivsarlh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2snufiars.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dedmdcyw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wyfajfll.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2erxqafsf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2athelhst.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2cpabsabt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2sdpgcuzc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bhhiazig.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wuqvhdht.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2iahcwbas.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2lqkgigpq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2uwzgqpip.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2htsyyyze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qliszkhp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wshlmxrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odasqldr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mylmhvpe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dsusdykl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ehwhpppp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2afdtcqcz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2rdmybvdc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2pfzsyulm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2pxacnstn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2qwhdwwqy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2gapjbnsa.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mfosmwnj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ykngucka.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uykdwioy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vuuvofbt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lvwbapfp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2neeegasq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qiorihir.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vwjoseex.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xayaeqbb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2isjakprf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rzyxihti.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ifdtdkdw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yymolzlp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ofuosvzl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ujzypinp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2cpiiybkk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fusqpjzq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2cnqhxhhh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nqssuigt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ohzsrpzi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rlyabaoc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pnkyjrgu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2uygpijpl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2avvaymsm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lnktgufk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xxxenzbm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vdzwimuo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jmiunmjh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cagdxbte.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2csswcwwf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mmprvxey.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vdljqqck.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zyisdjba.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2yaaidsdb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2yucxnwuw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wdrasfeh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zbrbchxv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gmgvglpd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kpwjlegi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2czhmhixt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xgzecvik.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2awcinzol.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kxofbmxh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sywwdezt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jsouywkt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jmbpegqu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ddaxgzvj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hoeojmod.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rsrbfexh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rhrcakpz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2yzdzfnuf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ttnakwkm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2aqejgzev.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2yyoabkld.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2exapppnd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fopbukcp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rxwwfkmy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2murvfane.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2heagyzpc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggyjpzrg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ctnrykpu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2etygfptm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2gucflfaz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wwxvwvai.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2yiyufltq.html


<!-- 参考信息 -->