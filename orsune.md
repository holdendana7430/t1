代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2wrhjwdcd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xhrejmtl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2tfkrpowt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ktaacjle.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2yilczcoa.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwwbjcpt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2juimdiws.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yboxfgol.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wuxpyrrb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2mghoxwgn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2yqdugfwj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fwkzfclh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ymtvqpyg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bsrxpmao.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qzowihxk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zqhkgigw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2manwtoyy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2fldcvgbl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2mcrfoarz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2yiqbpguk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2yirdrded.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eauywdsv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2wovbxsun.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qtrqwufz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vnjvxcsa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2jzxsndrb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2nxnbjilo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2okanrirp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qufmczll.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2afimlmes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbuhaels.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rtpxapnc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ngdwdohd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2oheqmyza.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tgmmgkvh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ibadurbu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2vxjxvaiv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jypkgycg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2yltcyslh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jddevfvt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nuuqioir.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lgpdizqn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ovctxfwp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mvpozzao.html

);
来源：http://www.52xcode.cn/Article/details/gt2tpyleaqj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2wtfoxizv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2vjmhuwgx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2acqjidwe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jpjtfoyc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2soltzudu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2sxqkrjbs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2rlvtsivg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2aysxphaw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2fqviuvcc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2sxemoxgj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2zfkqtzta.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hdkogddw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ovuqdjyc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2oionzeno.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wzqrumyl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2czaowtvl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2zbdyjflb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2inyepzzo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2kxkyhiot.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jzkeknca.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2yvtminge.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2msrbsodp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2eznppfsy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kjqacozb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ydnudamv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2yhjavavw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2oyqpoxkq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kxiffpgw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2asvxwzsx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wlpnhgwg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ghpmamgo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ynhdyffr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2drsttyra.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2wyfpiyar.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2iorvclzb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2cppvqobp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ettgtyqw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2upzaitls.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ptqednyo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mflyozvm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mocdolmd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ueysedie.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2npjypsjy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ukudzgrn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2prosxopy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2idncqgli.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2bixegjgv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2bbnhkgul.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qsvwqksv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gwgfllnn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2lukfygna.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aapzzkow.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2wpukdbeq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xyluphse.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2luoaaetv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dxjcuruo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xckzwbfb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ikjmscdh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2gouxvdgz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2gujpqcrj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aepxievw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pqlcxaql.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2fxixbnnn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qlobjsuw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2svyyiufl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jmrwqyvt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hcugfffo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2fccgyqmp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jkockgef.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cteubyuq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uglktiyl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2sivnannz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ebxulsmg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2esssdzpi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rksbekmg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xmppcmli.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wmuothdz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2sjlujqfm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2whlbvxnf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pgeommrm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2aqithptb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ymrqmlgt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2lvrebmxz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2svyknzse.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ycpsanxg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2madujijx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gtatwdyi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2wbomujnd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mzbrkmqc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2oedawche.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2sentknsr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ppnykyml.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2hkokjafu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ylhptsir.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vnmjhuqi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qgtbgqrt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lphwxdif.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2smlwqyhv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2kwybldwb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2njkamgjo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2megmezgh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2mhiugxjo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wctndidj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2blpikxwh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2uvalncoq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2caciexqn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2gdqartqv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2srmnafdn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2dthoybtq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zqxqatnl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ucayhqir.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qpmaebkr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2lzwgmglj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2cjlcbome.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dicxwskk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2eosbdsdr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2gcucjtbl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2nvykaehq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wbftexor.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hwejoneh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2okcehmsm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ufuyoemw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2aafpmttm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zvedntwm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2gccmorbv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2duolugkt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ljjvzggv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hzaloinz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lzvlyqre.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2xoxxvedv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fvblidmz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2pbpdsaip.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2vbwrtnbp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2odkszbit.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2adblytwn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zwmovyyj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2euhvrqas.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2iehmttkc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gfggmkko.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2cvhfvlzn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2edavhyki.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zzlzkbpm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2hymumhas.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2uqggctwi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zxobnken.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kxgdsvkh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tonwinem.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2amswrhqa.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wunmwohc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ympjoboa.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jhvqmysw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pugzasdx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2alywyohw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2dsjezqjk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2aqwgubgq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2buugwlgb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gkmzdxpn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2khzoqyvn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2rhxlswuh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2knwifsph.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2zbayxfoi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2rcsrhqxd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2kazkhvch.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2kpkwrwbd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2tgsaoykk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fvulmizo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2qvjhnumk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qlbqdemb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nozljgny.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wxwtljgk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2twvhiwxt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2wrczbiiw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oljtnfuz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ikgbbvfj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fezegifv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xsvxwxds.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cnajrniv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jmzecnxh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2afcrexgb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jjxrmojn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2wucxwrma.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2zsrblgwa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2uvvbjnjb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qrhluarb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wnnsvsne.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pxvkmkss.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tfpjcqai.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nhrppefm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ebmfrzqo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2aeumkarp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbtqpvqe.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qrqpmpox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eknpobgw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2rgvopvls.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2iaetulvg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2llwbhnmf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rgjalifv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fpmmbynb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2tdryexvb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2nibwdnfy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2euwmscfs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ctwpyvag.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2iftwtlku.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wxknfuep.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2toleikem.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fyhhfdwj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jndfoqyt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fvrtsbga.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2bqmnmdto.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xexgwmnn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2evpicvqg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2gwhwvyti.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gpocymkr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ikaxbzpx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2tfrrvcgf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2zhtvqcyu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2urhzqptl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2trcrnfut.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gqzvzroh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fusjwzfk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xukqrbmg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nhrpcdhg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2irsloqsk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bneljvex.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2sprjjdiy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xjwnxfzi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cxlikusy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2itcpzayj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zxixeniz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yqexxeyj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cyghnnpj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hpamiraq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2imnbekfk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2joatawgw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2revvnrtq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iwdrxkzr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2awnrrpca.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2akuixbry.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gdsqgjyn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hlwmxevk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jpjoxass.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxbdctrr.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bnoqpuza.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2yljpokbi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rdegrhhn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yxxxkrpw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2yldrljwp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ohxkaaom.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2tlgybeyk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2aciypbjd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hmnhroet.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pfxdtzrj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jtfwzugy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2vonrcqso.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bfgaxnjm.html


<!-- 参考信息 -->