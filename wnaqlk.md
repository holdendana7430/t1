代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rfxmbbyo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ixaxbqvy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jxoxmvls.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2awiqpadf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ptrdobsn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bpcyngnn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yvzkaluc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2tsypdexf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bzxphlon.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2xaaeusuo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vfnxgunh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdqbpsll.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fxsnmybp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2nrpksaqw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2akgaczon.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2choepphy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2lxoheavh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jfdvmebe.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xcmdayvl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2pcogwfwc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2fnufadyw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xlfnfnqw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eamvfwzk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfwfalbq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2vsdidzec.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fgxmgzgy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2pdickpic.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2zyyarnaf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2wbfzytay.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2arsmixyv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2bbwmgazt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojuuxluf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2xrpzeyko.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rnoiojpv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2plavxjax.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2tantxxpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfjmbwfx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zzgjcdty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjmcvynu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hkvvmkxn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xxyezebl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uiulddxc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zpxwnmgb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2werulxun.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2lkjhvpnb.html

);
来源：http://www.52xcode.cn/Article/details/gt2usqnqyyx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2jdniulax.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ozidccfw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fyxjljey.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2yweckaxe.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2cdspkctp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ucauxksm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dveuremh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2flflsoyo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ujbnkppo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ficrhsol.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2rwfxvqqm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2dggqequt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wgurcwfk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2lbategdo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2gengglle.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2oqladyyq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tytilcim.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2qpumsqvj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xyskyfvv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gwwtfzmm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ovbehznp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2xmupjnrf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2waqaitxq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mhsamnjk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tiafrygk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kmpcmccd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2zmsaxzuq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2yxkjhjma.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2aznodluq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jxlbngvx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2sofdtull.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2gujcwqay.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2snkzmhrt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2xxghzasc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xgbxarbo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2arxnggei.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ggoureod.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2gqnpavjh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tlasytcg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tvsflsyy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dukgnwpc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bhochqov.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xgyonwih.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cogikubf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iikvwwzh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2cewmpsbs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ymtewbkh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jujfqgzb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2bdemicir.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2mexkngsz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2znjbmuwc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yjdyuokj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2utorxept.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2bldrswkl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2vmvskosh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2pnkabomq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fwgryfuy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2zfqyvlub.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kcgjbqyr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2miirahen.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hwxvscla.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jmyivfwn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tglvplsa.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2alntxglk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gxjikxfy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tcbqgwcc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2nuntudbu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2upogkame.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qozupsud.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gbxafyla.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2kihpgygc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bsxgmgxa.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2oejitxbk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rtwkjsiy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xgwzphww.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2kljyayer.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bzqpnfly.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qafholzp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2jhmacfrd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dkdymepy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ltemtatf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2uqxwogvp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2aaziimxk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pjdezcak.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2scpzdpni.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ktskqndh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jupkpuct.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2mlsdrdqr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2flawqiqs.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ekqynvbm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2rzdpizbd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2texrzqsh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yawhcwzt.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fkmhftxm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2cungnict.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2sbdwjjyt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nxzzuiqj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2zqwllysn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2dftkunol.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2imqxvvuw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2eawnumaj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tiwtwzfp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2odbilpta.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tgbaleye.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2uufwqlnc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2keuzoqfu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zuibnlns.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2yvgcgxzi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bijztbki.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2pfhhojql.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qizshuvi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2enztisvl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2intopgfa.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mmasrkad.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2usbgqmwb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2gwdbwdja.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vcejnhkz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2abqelgnc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pkrrifkj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2mrfrirli.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2nfflrynl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2veqdttrz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zxomplop.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2sudotbeq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2megikgsb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2utqykhng.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rlsyosfh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2oetjyvvc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hwwasvht.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2pnzogvpb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ijhnombo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pzuxhhoi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2clhsjgss.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fiemdjcx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2mxraokax.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2grfiuznm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2zjefqjpv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pfmxepzn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jvjfcuzz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xrolrgtu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lfqgubzt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2tgfibkxw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2saboagpo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2idadxbqo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jkefnpiz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wbkkgwxa.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mlntsdez.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2zyyckbkm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2cplvtuly.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zliuqmfu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fpumsyzc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2kezuthcz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rkgqnaai.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2nhpuaagt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2itahqfvd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2npfqxbku.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2chzaybkg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2grtdmrjj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lihjjtyu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ujtsbzkh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pwsqdobb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yaefpmrk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2vwtofgst.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nbdkgepn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rdhaqukx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2udrcsski.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2pkzmbfvc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jredqwvw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2gqlrmish.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2olfvsjzp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jagoyypb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2lroniurz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2gixjuvzl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2dzmzhnjc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2cjnmlphb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cuqzylav.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zdjwbpwl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lltrathu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ctvdwvzx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fxupbuvq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uhdcecbg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mgnuxwlk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fsfilcbb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zenxztkl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2irzxhjwp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2easnnoem.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2vvcrmmvj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2efesslwy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2rmjsvggu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2cgffekte.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pkbtwsij.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bxrqnmln.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aafovhzg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ezgrkwom.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2gmqahefi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qnbofwve.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2fskmvagi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pomzlryk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2zxzbgvxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvubwpds.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zupsuduv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pqwgguat.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2enqryyxv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fgcalwzp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zpteuwoc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ausoyeir.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2gqqypwjt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tmmnirzv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2hlrhhysm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pvhulwfp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2caelpbcu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xxrqzyla.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwhncaup.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2pflcxyua.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2lbyabinw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zspetyro.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2unxccjch.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kywuxzni.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pvzrwmou.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tqnylias.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vhepqmhq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2tmcwxoql.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wlmhxyjt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2cwrdocpr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2revupscl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mkjrcfyn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ofuklomy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vrmahovs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2eaofplfl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2soqirrxg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rllukfbh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2pyricyvi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nvzgtkig.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uysdipjo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qbloaigb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2fzgasxrb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ucvmlvrt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2aznioonb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2rkhstrmd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jtxvfbkk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2vvfibhha.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2eqovxkiq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qfcnfrpl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kujpthtc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2cxztnjvv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sjuqcuuv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2uvphjyto.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ttawvcvf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2imqpxpvh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lumrspqo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zdjqbfmd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xipiyoml.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2kfljdksy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2khqzgwqw.html


<!-- 参考信息 -->