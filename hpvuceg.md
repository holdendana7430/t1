代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/guumgrqnt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gpblfdcnn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/ggodilhyk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/grhgmbbtc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/ggksdjxyk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gzfezpvov.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gwhiaoava.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gsjismxsm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gtzmmyrhf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/ggccklsvt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gacykdcaw.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gwwujmyeu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gzsvzevwa.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gzjcezzzq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gnxgsknlv.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gtnnydptt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/goeravsti.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gxgxiapti.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gspqmnuji.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gtskqgvum.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gvdbeettq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gysjvgvjc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gtmgigore.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gmumimcsr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gtunpvzrx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gwhumwogz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gfaeglrer.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gwopghiki.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gjxmkytop.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gmmbjppun.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gzyalxwnv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gbamfzfsl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gtmilruju.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gcvxuelem.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gicstnhlo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/ggijumhce.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grjclqpyt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gctecqgln.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqupdjrpt.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gggkgbrlv.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gqdqfnykk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gwmjktoqd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gvwbadpka.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gdoofavqo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gvtsctavl.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gnjwyuhqp.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/ghsgdkwuj.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gauddjsbh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/glccoimdx.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gonbbbopi.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gaktmlaua.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gbnxkgbhd.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/glxozstwa.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gqqrhiinp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gstneqfzr.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gmomygoap.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gbcrzduul.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gjpmgnueb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gzjcxrzqt.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gmhdaoubm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/ggglgvsqw.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gzuydcxdl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gonfirkxi.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gbfzhtwnk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gidvsiyug.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gryeewzaj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gtlnpbanf.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gwrejaxyn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/geayofrup.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gmfoeunxt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gqnjkibjf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gesqtnnps.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gcfdqggqb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gykckuuwo.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/glctmfqur.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gvfkimsev.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/geldtflfc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gmymkayek.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gskadmkms.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gofnbtxny.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gqwvjgwob.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/ggswthiea.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gegukphke.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gmbzvzlyb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gexfiarbq.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gjajkpdwq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gejxpobxl.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gwubqdejr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gdpzjbfnp.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/ggvrrrjrf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gybazzhzg.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gicftcesq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gicgkqxsx.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gmtlkoopz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gyvabwajm.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gxwcfttge.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gdawvqawt.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gaeduwtmh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gelqbrfqi.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gytlvxncp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gkjeiyakc.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gzgrugeic.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gniagezfn.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/giithhofm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gpnltiedl.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/grgfzrfaj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gobfvclzj.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/grcskkywv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gukigkwuz.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/giemlwcfu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gwfmhzrsm.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gnmmjgjeb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gnhbuiojj.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gzusbjcnw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gfgowlvyr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gfbzrvgyd.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/glqntawso.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gpdcljqwh.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/girphjmnp.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/ghcufjema.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gfcadganu.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/grjimypgl.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gbzqwdfxw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gejculbec.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gsdrdrbfi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gdtqoumie.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gqkevjngm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gedszdsoe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gnelbtprs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gaybeqtxl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gbeehthck.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gxxkmlkzg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gkkwjqegi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gumgcnvmk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gdscphstt.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gaizbpujx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gmwiykuqt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gssmnxqqx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gsutkpaka.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gdykdhsvc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/ggvpvulbu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/garovalkw.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gtmterocj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gonififjn.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/ggezdvrsg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gdlatykka.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gapfitekj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gvdibhxnb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gkfvpwbbg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gwcwdeaxw.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gczqnmxic.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gmikeuuti.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/glbgicbta.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gkvdkwhgh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gdkrxohfo.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/guqsspdde.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/ggprtoddt.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gfdxmnrhn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/ghsnpgkzc.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gfaeyunfc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gqrxmcgge.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gsbxcgswa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gxymovtrv.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gisfriobr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gpdvzaqls.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gnntbench.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gqpvjxfpm.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/goqgkgnbb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gwkpaosdh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/grtlkeujv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gtvebhrdk.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/groeazula.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gporuhqmd.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/glgmoguqa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gkjaoajzu.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gxzhisyph.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gfqdgwgcz.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gtezbchyk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gkojesgyl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjbtqjawh.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gegnibdlz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gmmtinpij.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gcqjrkpqb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/giuomnqsh.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gyzdzayty.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gxmhcpcqm.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gdigocfkf.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gkwuycktq.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gmsfrfvvc.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gbahzczwu.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gmggbrzwc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gsagfilzc.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gbfmpzuuk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gvdobdtgl.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/glpeizbzz.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gaybfzswc.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gftyznqgs.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gteodlaxc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gbzoyahsx.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gdzjvdxqy.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gysewcype.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gtcrxkvjw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gtjpgbfkp.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gbtokokwl.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gglbfaeig.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gzzrxkoxg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gvulwicjz.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gfkcifyba.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gzthbfpxg.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/ghxxvaoca.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/goqvimmab.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/ggppnfoam.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gqyurioox.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gojufigdq.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/girfratlv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gfgqdvgig.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/ggzdfucbm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gvvozvzdd.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/ggtappgdu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gcbsxcott.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gmqztwpmx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwxqpwclr.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gzmumelhf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gqrnzaxaf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gjulodkyo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gzvfjffwf.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gxwlymlmt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gemijozho.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gwlmghelu.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbfdvxqqd.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gfdnzfric.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gogcepewm.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gthlvjrkf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gpcegdukg.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/ggmbgdeiw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gtkmgjfrk.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gezbmfriu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gqduzhhmg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gfcmfbciy.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gdcancieu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gfsseybgq.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/grpjuygfx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gqsvgckgi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzgxotfwd.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/getamebod.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvqltbxaw.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gtvusjslb.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gvpbeamyt.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gddxbpghn.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gghtverif.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gudylvqvu.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gkgxocutb.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/geeozqzee.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/griyysmod.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gpotyrizs.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gzgyzvita.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gzgnztmup.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gbqasvppg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gegdrbhcn.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/giuepibck.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gzqjxdyrj.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/ggelbptxf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gxfrnqopu.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/ghwssibcd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gkldrfuoj.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gltudkyme.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gpumzvsna.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/grhrtcaqo.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/grmjeucpz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gqenchhoi.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gxpmwwmyh.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gcpxkhnhc.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gneeoifzt.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gipxybxqe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/geiopbhna.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/ghnosatji.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gjvjlnkkj.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/ghmzateww.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/ghfpenqir.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gmpglwdxj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gtnjyxuma.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gpoppykpg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gkvxzefsf.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/ghshghvdv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gtwwljkta.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gstgtuifw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gdsywncdj.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/glqrxoeiq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqcvoiocm.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gekcqmjmf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gpcvhllnh.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gogbmqqqw.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gdinymkmo.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gewrbuajl.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/geuzfkvuo.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/grdpdhvwf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/grqdxemox.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gqyihfibl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gbvoqgppq.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gexocgczm.sHtML


<!-- 参考信息 -->