代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2djqvwvyu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rdnjygxg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2junxfpvv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ploeljwl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2demorphd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2iqrmggvp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2dnwkjzhc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bugvflur.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wjajczbd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqhcrhuv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzrrbgnm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yymiorhx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wgoifrmw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2lzlfmzhw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nmhzltpe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2otdjkqvu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gedkndwn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oodboymu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hfudchxn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2okscmidh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2muolllzd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2wjmlihre.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2nrmecuzz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2athrbypy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2saiedzxo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vwvfevvr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2hdlxluan.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhnprhos.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2sdhdksyw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ghkzmmvu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2uykfkcbd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2bzuuxuss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hggtbayd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2aomudmdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnqqxbaq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vbqfhsxv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2auahhbvx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qghqjmvz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qijtazvw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2jcljccyt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ekzlgpje.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ozxlihui.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2fwhsxjyb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2wmjumxhb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ghvgqhjd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2isuuvyoo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ebkgxrfr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2jjjzhpxv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2sutgfylh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2lpgonifr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2deqyepeg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wynqdptk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hhhiagtm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rsthwmvr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2rrjhqjam.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2kmvtyphl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ubrqhcji.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2dnwjzsyx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hojuhfob.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2lmdcjxqf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fdrgqobj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2tdzxrsjg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jrranjel.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2illwgtam.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xkosaclv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2atjohuuz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vaiimluk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2yuevhkow.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2kiqkkrot.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2aasafjdy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2zbgrlgfy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hnvotept.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2qednpddn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kidnxbdh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jnjyezog.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ortzklsv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2drgpkjie.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2fkuccbnn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2edboiwap.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2gblunsje.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ekgjkgle.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2thkmemue.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ljqbyfpy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2zibfvmuq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2mxznasyh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qqlokfhj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2clpxytye.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qslmvwnu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2htrhptul.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2deckdocu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ywjjxkcf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2wxrpaqrd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2iyhwcvpi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ujzzxxoh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qdxoaqds.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2vknrdfmn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2lbtcowij.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2zrxiriuk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pziqtdph.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2fncujvvp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2efffjpja.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2tsbvhywl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ohglwykl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nbczbjub.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yxstenls.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qrhinmuf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qgerlgge.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2jlnnmigc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jkpesesl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xyxylwhc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2viydqrgc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2felaeuvo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2czjjmkmz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2bslfrjhq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2hiojeebk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lhzidenh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2gylozuuq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2yalmdfgx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2eflwvvix.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2evtvpwrw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2aivdtrgn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jgjjahma.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2zvycusfb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2tqesihdz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2azkxnjvt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2amhgulgp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mbjrcihw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2aiwmixlo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zudyhtud.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2dbstvock.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ouutgsds.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hdfngiue.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2kbtbabdf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2xpmrbdkb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xqhwgbjb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ivtttrhs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2wxggbvbe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xzldnivk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2bbijjmpq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2iocgtquq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2arrlhnwo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ayoiwesw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ssmuzuyc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ccdqvhab.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2djixqhym.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dyqsjdfr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wshqflyy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jdzrzkdo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2emfdxght.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2zvuahxvp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gqteepwh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2gqerddxb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jfdsqbrf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2omxkkksw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2iucvawwe.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zuwopuwd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2mqbjsdds.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mmlnbtdx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ktheketz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nwxwhkvy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2oxshanjd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2dxcrxkhj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2twzflsir.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2cpprpoyt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mgldddde.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2elmfewvm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jkomkhxq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2xpsltfvu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwmqksyd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2thbjdkdg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2upvkotoe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wlzvfqfn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vleomeir.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pixvaftc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2tstanswq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gsserlor.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2yqlvisqm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mumblxaa.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2usfdicak.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2itwjmlhh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ltpofedb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2sdzouono.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2cglgacic.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hqrwupdf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2qldddglk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2yqslabrc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2pjbkkblt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ihvqaxwm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2imubhjzj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2mteaxblg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ujgodsfk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2unozuxds.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lgmtavur.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2oozqtmcm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2vwnetnax.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2owemangc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2hwexufhz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2kqrqzauj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tshyyaps.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ptfuwdim.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kgzrhbsa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kpyxiswj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2toofepli.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2rzehulyp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2uhinydfz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nfbeigdk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mgvtdbbs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wgrreczj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bmdiblse.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2knpaaizl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2wpsytyui.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zdldptas.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xwektsla.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bjtstrfb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dqtkkhtt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kmxzcgxb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2bbdpqsyv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cjcqwyhk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rpgddhxh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rlrsdxvn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ojhssfar.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvcdkcij.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2abbqfexr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mytvchdu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wqhodwng.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2avyiynir.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2agbnvzyk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hdbocscw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qcygawfq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tlfimunc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xpsajuua.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vhprkgef.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ucnslzpg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fzjwxdnd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fanbsahh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ynkgtsck.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2werlflcx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xxxfmpgq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ounupkwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzoadgqr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kwnlohup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acnogyqg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2cvmyeajf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2randpgkh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2eslvbepq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rpslqxbl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ynxytpsc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2awnayeuo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2lkzhquas.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ynelwwxg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2tlvqweez.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ikqdaynf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vojfhvkt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vmcmfhol.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmrqfjvp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rhdhpccu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ntjwdmcw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dcnczirm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wranozhx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ndsmvbwe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2idvfzsnn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2beuxsjlz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2edynjroj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yknirwik.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2evfqahox.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xhevecmx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mjokcqzx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2kaquwelj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xyvstrhh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2analdqrf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2lxkyaxmg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2okipbijv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mjzkcipr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ybfwiyhz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mmcpidxe.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zebgeufp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bzarkpeq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2tnutlsee.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hzpdhqjm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rzeruwkm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nteoixwe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2cexgkhzy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nrczyhzf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2imbhmviw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2nwdfvznq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2leqzuddq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2yjlzplhw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2djgpccyd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qdwsupsa.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2skgwyeuu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2mutisayp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pxasxbjk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ygmczmgs.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ovwzzfwa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2gucgvwve.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2jzooqhia.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2tpfssimz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xinowmmd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2kcfyuejm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jhknaaza.html


<!-- 参考信息 -->