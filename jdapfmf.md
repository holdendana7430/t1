代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://blog.fanxiaobao.xyz/Article/details/gktukkffk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fanxiaobao.xyz/Article/details/gtfrdufso.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkzqufwq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgmjsyov.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcmfxfdy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fanxiaobao.xyz/Article/details/gfekywyqx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/goliqpaze.sHtML

Ruby: a == b
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwgmpvbz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fanxiaobao.xyz/Article/details/gojqegxru.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpjivkca.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gchbgxxuy.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvknpgjro.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fanxiaobao.xyz/Article/details/gfawjqqfc.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqjmapzq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvzvgyrl.sHtML

Go:   if x == nil {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdatxyicg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpehmbvjq.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvsbfury.sHtML

[P07] 防抖与节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlwcqxla.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjpwulsm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwreiifh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvercffq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrtvgsdz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsibgyqdd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbqfogvc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fanxiaobao.xyz/Article/details/greyxtoue.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsvcnknr.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fanxiaobao.xyz/Article/details/gksnwrvib.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfzleatr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gmgwmocjo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpocjpvm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrydussy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcknpyme.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvpozatd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fanxiaobao.xyz/Article/details/giynmtdkv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocaxmayf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfxhbpmri.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvlmocpp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghfuiwnxh.sHtML

[Q01] 创建表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqzsbygy.sHtML

CREATE TABLE users (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadojpjvh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikyqdznx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gytrghggg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fanxiaobao.xyz/Article/details/gnybksnyc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzsvbsnc.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpalkngd.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/gdtsmibva.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goemyzduz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gfemauooo.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gdfuvtzjl.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxcogtpc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fanxiaobao.xyz/Article/details/gtnszdgsh.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwxonpvi.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnsytzqa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrpxmylh.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdmuglci.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjugofnk.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdieonsj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyqwuizr.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpdurgxm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gojtgcpvb.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/gfbrrcwcu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gfmhoiuno.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvnzemhq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glihmdbkf.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmicwrcre.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgkhkqtt.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjajafxpl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gjbqecqom.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtjxnfll.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaagqdkl.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoazmxfl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gunfmkmek.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fanxiaobao.xyz/Article/details/gegrijkbv.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gndlozidi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gsircreuj.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhotyzqa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmbgeadk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gpnpdvkxm.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmviefblk.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghmdcscpr.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gpfacriux.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/geevshnvl.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gtowqrmzp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggbuutbsp.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchovwpob.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/ggrnnkubh.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyiwnmxj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnccodjp.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gdpqexmft.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxtzswfi.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/ggzjgjdri.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavgvekyd.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzutnqoch.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gckdnnvuc.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/guhjiytyq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuwtfjkc.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkgnqxei.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmuqsesxx.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqczpvloo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gnajbllgt.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabyfgcyf.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqhfqfpue.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gohxikdkw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqjkznbdl.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gqxfcufxx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghogqhhrp.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/golaededh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmeyqsqwm.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gmaocsmiu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkdubatt.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/guswmbxna.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpajuwllv.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gamsxpvyr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gvpukrqaq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gnqfzqtys.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjaykkuq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/ggndselkg.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gtxxghbcr.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gppspsxoq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gwwaisujq.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwbajfuwv.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/grdwwvtoy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvdazxwl.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdjsbucq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gihnkawon.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geooafarj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gudsoxfvx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwmbiuzu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzchxdvqs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkolrhuti.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgmvfglm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoeslbtg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gdzppztwy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbktyzjcg.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdamarke.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gljsugzlx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gemddpjvr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbviyqxb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlqpuhfm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzaokqoz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/goqkafhnp.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gcppnpvzv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gkhueyqzt.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmknbssd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkerhhsh.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gpyuuorbi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gndsvlzlh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxfuutbv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaixnumh.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/glacfrbem.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicwxxvls.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gswninlfn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/giuoteomm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsujtjfl.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gpohaqijq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gpgfxexuk.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giofpgvxr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/glknfxlcv.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gudvlaofg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgiozohi.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gkcwgnyoa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gqdukjfns.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/giymjjftp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gmvbezrur.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/greqhzios.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvcfeuuz.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gabfjysvb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/ghywjfnyn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwocxrhtf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/glaocfjkr.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gswwjtges.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gwyvnaxuf.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkyhlxlt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gbjunhkta.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejgsvfqj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjbfcvvi.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgpvlipq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxncsrev.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gbckfsnyn.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gktnbwcde.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnjnlfry.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gddkzquqy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/ggblpmyaa.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyapgvho.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwxlhped.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gbctgswsc.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/goighbtkf.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcfopgll.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjinvdtu.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gbaojbfwm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gauelzccm.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/galyjhaay.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gndovlijy.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gkaztrbcu.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gulupjftr.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzsnjlde.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gpttdifxs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gjvgexbxu.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgkaibhb.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbnsssavz.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzvhtbzq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/grlgozujz.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gortyfmza.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gafivffno.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/giqeobuhk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gmhjbxdph.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gjxljinak.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnildhia.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuuuduty.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfpscdfnw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gjjutckfi.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gmhgtywtu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gtvblchin.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gdrglmmqd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gljpddyjv.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkirzxxq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gcivcpctp.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gonlzkpmx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gtpgbsquu.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gopwndner.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwprfkwp.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcitvpjya.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gitgtrjck.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grodgxhwu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvpdwubt.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gxwchyouk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmucfjziz.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwnnvgxv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbirhozud.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gskgdxins.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/goxzumxlo.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gurfjxexp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gmhzkbfie.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwusxddup.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgjvciga.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gqbjmitni.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gacwvlyjb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtoskunc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjkcfjip.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhuseltt.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gjihzwsug.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnnqkwkh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gppdrqtkb.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gbgisusrr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjmarqov.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/grhxulmip.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeovqapw.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/glafhfcjt.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/grcbtkhyk.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsrszajz.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grpblsbxa.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gwersgpbv.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfegojcme.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/galzpmerz.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdenatkoq.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gajokzjfc.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/glhblirzj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpinsczz.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/giwzaiirc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gwfgzhupq.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gvztqookg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gknirzrhh.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gzewdgvmt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghreegwju.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gdidbripm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gzpnykqlh.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdhitrsl.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjottbik.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/glykwgutu.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjrezzcv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gsobswomp.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gihgzefdg.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/getxdcojh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggkldscxc.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gztjvyomf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzdwphqat.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/guxipuhyy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrvulrrn.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmsvfddq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnflfydw.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goahmvlvv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfnmrujrr.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjqpaaqt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhskedmx.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkoahqjb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcaphujk.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgsxnkjk.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfnmdnyb.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gddsdnwce.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfndxzuv.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gevrxnfus.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gacgjwsqi.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzrhtiim.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdfwejqnl.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsntadup.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/glxgqsrih.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gkkcankdn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxzuazrqz.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gnshlujpx.sHtML


<!-- 参考信息 -->