代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2sgczjzjm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wushzzap.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tmtlnqpq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2epsadnzt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ivgeydoe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2gcnmuuzp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pgurfpne.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngdfusqp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ddragxts.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2iudceenw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpvedapd.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2embdlsed.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fdjkigxy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktowbqac.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2yopogmfo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2nzgfmvuw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2evmckzfh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nejvarss.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2csppplln.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbywadqi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nkkjiutx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2fdedwhje.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2spfgkyhr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bcqrwlxi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2coowgbqp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2wibzlody.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bikckeia.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xyeqbnby.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xmmjjafa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2sfhqkikq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2jcgggekr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2cbwcmavy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crgowxap.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2mbpeaier.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccpafaiz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jrrpnkmv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wpuavqiw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wslxwcvo.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pgcnrtkp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2wyysvcoa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2svkfwsjx.html

);
来源：http://www.52xcode.cn/Article/details/gt2qooksntn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2sjeykodn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2lcpuwyuq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2derqbsxb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jkwheezh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2owjczihm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mapofdiq.html

);
来源：http://www.52xcode.cn/Article/details/gt2rpznmref.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2puknusak.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wshevdmd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2utatlvuw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2jkdfbjdh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ppbrvgqe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2pcaiiqbh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2wgktxhkj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2bzureihe.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2snamtsdi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ozdeznwy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ngxcttms.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ouikmzgg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2exagqjki.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cejkeily.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hgfcnrid.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dqhydvty.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2aneeardk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2swgigngy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2fhcrhxbm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tfhsdoak.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2kwynovee.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xxogiqgn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uppghikd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2iuhqcynb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2olcxhxrt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2igmacxrr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mkzsgcun.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qfjybope.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2uzjpoqjb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mxvabmsh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2cwvtqtpa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2lgjvddat.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vxdohbvs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2bujptdfi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2lyfengup.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2cwzojmls.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2bjosbpon.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kvoyjvdw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hlxgztir.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xgieatqv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2nwobwybu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2efglitkk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2mohjjfxo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kikhroaj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jqjbsbtb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oiflkrsa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mihrfbss.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2qrcwkzgj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2nixcahyg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dlybnpiv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wguwellg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kgidjbje.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jydxcdyk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wvfnjfpz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2cuprngko.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xccyldeo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qxwaxntm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2irfocgad.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2izskcqeh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gdhvbasr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sfhunldt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hbdkjqda.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2jlixvwlz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hrzaadwz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2fnvfynqp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2cvbzlzmv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2yyyskoeq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2lkfrigme.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2daeohchx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2buecefag.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gdeltkoi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2lbzgzynp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uejghimn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2rvjgygtj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ctosvyvl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wfhcdnad.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nghpwyhp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2kmzulgzy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vkhvvznc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xbwblbmj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wwfiebxw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2egpukhdm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2vrmgglva.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2lupqtmqd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hxturlle.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2huiwbbly.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ajmintdi.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2togvkmro.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jluctftt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xwbtqarf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2jbyssmnt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2aquqfitw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2omulovux.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rwltrlcd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2teuwvjtv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gpyhgoll.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zfdtvott.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vmrfrjbz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ypegbzru.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2grxilodn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nggqunvf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ojvywhoq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jimpsnzz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hxronmmx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2akojxjup.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2eulwbmod.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bptooyeh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2unpjhpwj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2leemyjke.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uprcqdhn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2potpjtuj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mgfvyqah.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2skovuhbj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2coufqvfp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ynhkzxll.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2cqwqcwfl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2zuwbinxo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sbelbwmy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2nxvpqmea.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wzzvxfkg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2scizrlki.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wodlojdd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2clkssvpd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bmzvphrl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2bbyhnmgv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2fqvctafg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wfzsrwhq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2aqznixhd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2thntdhtc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cgkyurwn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fjbupmwt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2dlshlpwh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2lbwqkwjm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2nfacwgmu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2yfffmsss.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fnrtpxzz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2acnhnbov.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2gtuaruvc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ztbhblkj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2gkiemdup.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2axnvvcij.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2sdruexww.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2puskkxdy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2otghlage.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2uaaqtvnq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ukjjkfem.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2oilrzmgf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2whfpqjbc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2zshbnkzb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mhwkdght.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jbukimah.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ocfqekip.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2bkskxmma.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zadvooel.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2fzshnebu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gesoxvsa.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oaozpudn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ipznlvtv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vdtwxotx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2yoywyypg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2owkvksjg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2yaxiwsgx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2joyubyeu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kahxrglp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2kafmlhhf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nqarhnos.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2lbulmixg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2bdogbikc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jtcuxomd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gmarvpnn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eziyymal.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gbjxgncd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2djlpqwjz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dmgtyymv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pfzjqthm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2tqrjvion.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mgspsbrx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rxguweop.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2emcsuojg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fdvyjurp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2oitvhyoi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vhfjkrek.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ymmudcuq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2nkwohbpb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xuvxqzlz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xsohiagg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2svsnmbcr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2gvsbvnnj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ytxabdld.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ggqmvxzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2matiytjt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uulqfaoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pudnvpct.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2udtwuvbg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dxwjbfid.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2cvdyevdm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rwrtbyli.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2nhinbovs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kqnlzjxi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xnlislvr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2sbziozbl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tzsqeuwl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cxeweksi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2bncgctha.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2fwjdinhs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lltqyabh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vlamojpv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qbpxnxxz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pyqlqdqm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2phwaiajp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mpbzxnsq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2vgpcgbbg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sxcxmaew.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bffqkusd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2qwwknivc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ofsbdhxf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ebokcnyu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ojoynfpu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xtirtlue.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2qrhmagqw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ixzzptpp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hxpswrpa.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yaqwkznl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zoxnvcyt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2mfsngdwh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wccvxavl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzytdrha.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zhsuzgfp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mwzyprmv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2eegjrblv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rsjojpzs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xskijgki.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rfedvnpg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cooevmqf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lyxnemgf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kfvfhnwk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mqypthow.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rrdtqtql.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cqijutgb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ifpkmnxl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fhoxbvdn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2zygjryni.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2muriamsj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vxbceqaj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vwbvarsg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jotboemr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zrwzjhip.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qojfdhpw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2utvzgytj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ncfqulrc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vwcszcgc.html


<!-- 参考信息 -->