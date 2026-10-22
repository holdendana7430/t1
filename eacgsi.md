代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2cfocnwmg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2hwgdltqz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xfglkdmk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2uelaoimr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lbxikxaw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2mkpjemck.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qcltdvdc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2htujezzz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2lhzcflug.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2teaoipoa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cyxgrxsb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hsrhxpcz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jaopumqn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2erebcjup.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rhvfxpdf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2damenxqf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2nzzqjzjj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2okuwgfpg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2nqhtnpcd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rxoorifv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2pvxekhiy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2anelbgow.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wbxyfkld.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2gszcwrsx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2sdqrnqbq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2klztjwzg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wyjjznag.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xadtzjjd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2tfbxgnvx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eofyzhee.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ymnklmuc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hcxzponi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2oaidrjme.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2yvgjjlsr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2izwolmbc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qijcyrfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iosmbakk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2sqkapvxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2libdupkg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ycwkjszy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xabfmvut.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pydixnkf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pezcthvs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2lsqeuwoa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ufqeahhb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bldzgmxc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2uxftlptg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2extrntun.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pmcrvvwn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2juetcust.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xeskiwwd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2eftxzwuv.html

);
来源：http://www.52xcode.cn/Article/details/gt2hnjeavpl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zbkxdnhd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2bdixepwg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2vzngdeii.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tlyqizve.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2mhwwhqrt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2uclaeniz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2taxemqqn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ssvpyzlc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2bbmwxnkq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ytggpxou.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ovnbiaiy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2grpytdas.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2pvlwnhmu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qpwkryck.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2uxmeukme.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2agmoxbch.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2nfxtwjlf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2eimujytf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zdzyupqa.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2cgsipuvy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2puwnsvka.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vjpxuvuv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qdtgrqav.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xufgyqgg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2dtqsotqi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2owzhpshh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jqespham.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vqupqllk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zchpmjal.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pqcmijtx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wfhucmes.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xacesuqp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pzcfqzrk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2olxdmlrs.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ddlpjqro.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2sniseogh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qwsondkw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uritbujx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2kogrtevg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mmmpcule.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2grefmlgf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2pukkcpey.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bdwbnnqj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2dkcjyldh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mvdqrfuy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tlospnli.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2cogggazl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mhgihysh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2rpqnparq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qwxrizfp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vqkjgfgf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sggtidfx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2trczqpst.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hzmaobah.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dukumkpp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dyiwubnc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2levegcfe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xeoogdbq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2pupapccq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ozpgmptq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uireegzl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mzcskuaz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wtdlezit.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bbsiyynf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2njgjbiqi.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vqrvfmqz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2uejyvnge.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qjhanxoa.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2iyvalpyz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ycqaojra.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qtwcjhyo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2nbnzfdbl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rixfahln.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ttnonjxh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qqpqhmqr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gwgbedbn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2accgdnsh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2knmlzrzz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vzbydcga.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2udcexnxw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2qpyrtjvn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2lkevyoet.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ihtrgxpb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jfpuwxhl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vloxlfoo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bccrdnrn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2lxbalpex.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2jzakptsh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vuatkkif.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ooogjnpi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jtdpuezq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ilpdfgsd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2gcfnmbvc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dmenwbzt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vyctqafm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2mwtoozgj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rnfxinjc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wvdyxybe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2icrzxhxl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bwilndio.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2oqgyrqvm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2koncbtlx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2lbwsxxra.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gzitrmug.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2uubyibcn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rysjlrmy.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2vsdhzdhl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bgnojkat.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2hmyrlmvo.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bsbckmbz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qusuiavk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2incddels.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wjbxifvn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2fdpvsdkw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2johgnjmw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kbynwptg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2snngpgfv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bzbqomzg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2sfjhoaoq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2taurfhvz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2fzwjkkwb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jlqykdll.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2uiphkthb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ojyphyvq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wjvmvuzw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2cbiowixy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rsuhsodp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2kbpjogqc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bzogkbbd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2iogbhcox.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ngbtwmjo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2gdykoghs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2pmkukpbt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wownshus.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2oyscndgp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zktrysha.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2kxsgbrvl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jiryapti.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2pvhjzwje.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2wfdojova.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jcsrrepo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ypazpqno.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jcbrhfhr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2serenfme.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ioedrdrw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2lvwvrudk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2wqxmwaeo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2gbszhfkq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2nbgaqecc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cbfczwic.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rhguctgf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pjdztvaa.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2npbiiivw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2girgofty.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ybumixmw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gsnejjuj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nkwiwobe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hrpnbcrb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2rroiieam.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lmklhlnl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jjrtrqem.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lxpkpvnl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2tfgwhumm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hwzybrec.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gqbzfady.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2onbnnwpx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wxegexkt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ytprnwqt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cfofxefn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rkxyqafr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fzjhfzkn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ukredkbb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cxgtvxyy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2deustvej.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2khbshtks.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2dxwltczv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ebbyriuc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2wtiyoatb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2kneljipv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2etnojvck.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2scwkrqal.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2weqhylsd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2crkyszwo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2blwjtumm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2grwgilmu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ombzewgk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lxzdnjyh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zbynieya.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ijisderw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2mmyaiscu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oekjdgss.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xkedkmzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdrmyqdp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ryxlufry.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2hzzhqmcg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2jqmwexka.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pnkkiexm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2bcbbuduq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kwsspcjb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cxwuphjf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2msaozvlf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qcsrqvby.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2coglgchs.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2pvsjyfja.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gprlpxaq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qekoukvj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrkyisac.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yaoqfjis.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xahhpkbn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nlstsgkk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ozgjtucy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aspbbsds.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mubjlpey.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wiwgxorj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jrrhrfff.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mbbykqmo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2okwdspsk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tlittdqi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dshrqqgl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gorcmkep.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2evcsrpjk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2xyzaxuih.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lwmvuktn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2naclyawv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2mwikyqaw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xiivuqrj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jefkjlkb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ffgzszxl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wfeyyjkg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kqwahcka.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2knznmrcm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vukumljz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vdlptcty.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mgzqtcqt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rpaqqjxv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2pueambib.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2aqytsfkl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2fmmxotiw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ewvxjogq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gqwvwndk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uvuipadg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2selyjkyw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rljhpcut.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rnmxrsiy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rlkkwlhr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ybrzjrtf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2earypukj.html


<!-- 参考信息 -->