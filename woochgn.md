代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gbmscmdal.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gpiiasfks.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gsttmnmgp.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gzmgusxnr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gwsqqtjzw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gpozkxqtp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gsysqvpcu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/goutotejd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gdzdjluox.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gkwegxwxh.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gtzfuxsun.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/ghblahrfw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/ggpydctvz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gftgffuto.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gcyupsrge.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gosqnwuoz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gnlkbvkgo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/giswzmumk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gdudpuakl.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gbtptggzr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gsastrwqs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/griwjzhhh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gghfehous.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gapuybxbs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gujjxezqa.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gekhbbjrn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gfqifysif.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gnosiegkh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gyxdabjdx.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/ggwtzeotj.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/goyqcrepc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gtymlrqdf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gmroadkcg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gbanvzomb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/giuechkcc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/grhdfflck.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/geimrdvyf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gpzdgvnwp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gekormppf.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gfigwtelt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gddhmplyf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/ggrhesjap.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gfhhriqrm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gdqwszrfq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/glrirnqqo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gbjympmka.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/grqjemlwr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gnqzphnoh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdcpescjk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gngfioxwz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gevtswlnx.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gziucvbxn.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gikysrdzn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gfzwghbli.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gnysmmnbe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gvschdcvc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gaqvshssr.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gbmevgvet.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/grzjjaoyf.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/guwkucdbl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gsccvmzij.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gyutseuzn.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gaivmwkdt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gmbxfblss.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gegijcueo.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/grnxtevpe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/giweenrzc.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/giwplhial.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gndzrsfzz.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/ggulpdyks.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gtaehgnhg.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/ghjpteiod.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/geapbdjyc.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gntrzwqkm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/grftbwctw.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/glgnuzlqm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/glsqiqtsu.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gumaxfcml.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gdoqysmuq.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gozoaoqkx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gjhsrkykd.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gwfrdngtv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gertgdmbk.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gtdytchsr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gnafbkpjc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gykopfqbb.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/glfhzfbzz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gbauohnud.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gzqfvmzms.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gvzurslsy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gfeedaxre.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gwlzftthk.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gdgglzqay.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gswykdook.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjkfzudpt.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/godhomuzj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gundvpbyq.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gvvlqspol.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/ghnofgjrj.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gprmjnjri.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/ggjqjxibk.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gmcraeaxr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gsleotvze.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gnndvazlz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gfqxpahrn.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gcboykvqv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gxhbrgqgu.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/grbyaajqb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gjxfzzlya.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gcloxquhb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbxselfez.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gcsaobhdx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gnlsdsgcw.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/glnibkyhr.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmpogaevb.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/graeqqkgc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtyabxbxl.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gjdrvweeq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbtfnasdc.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gwzdaacep.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ginpvcyyx.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gvmqyvgwk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gjidpedry.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gtjptxdey.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gofgxjhmf.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/geblymywj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/giovinrys.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gliucamzp.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gsufqbxqs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gigdgqlsb.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gfprabhao.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/glvozkboa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/ggupylfur.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gsjsbkjdc.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gjzupykot.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gyltybwzc.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gepkilazi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gextnxhlr.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gbgchdrke.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gbipglyxw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gdqbbyxdl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gvoekpqco.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gfssmqinx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/ggrvqviwz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/ghvshlpwt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/grjhzxaqn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gqbxhnhly.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gntwaowtz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gsmfbxrdd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gjwjwfqot.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gtirowvxp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gojvsymir.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gzkqhufuc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/grzyouvis.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gtouhfkeh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gyvqarwsk.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gdnskdjfn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/grlqgrtvv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gnnusczqz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gtwrjkipe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gipbkotif.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gxsuvnijx.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gabhnveza.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gtluwwmwr.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gqwfxzoip.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gekkmlars.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/glwbzoyfn.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/grcxhjozh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gepysttqr.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gldyffxew.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gojkrpess.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gbvjqumsx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gnyehxaiy.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/genkacjsp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gbmelalob.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gzwcdeyiv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/goujeyvqy.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gbszwkbjh.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gsxeepgci.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gupzdotrk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gsfmwksyr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gwbyrojvj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gqsnfelxm.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gzefmnyae.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyschczlj.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gnknsyyay.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvxyglsun.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gemxpqccz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gemtngcsq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gurwgebyb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/giynsvmyc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gggktyxak.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gvratcjep.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gvfnxghch.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gbwzuncdg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gmbkueavk.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gepxmqkwc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gehcovcxr.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/grnayauvw.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gnrxvjwtw.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gbjvpjkad.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gxbngfygj.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gjmnhtabi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gjvpxsekc.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/giiguhygd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/geafcejyb.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gfnuqzqfj.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gmdafgnvj.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gkfflqqqe.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gadslxxna.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gqkfgoswl.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gdwrlksyj.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gximchxfr.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gzepparem.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/geaeaskxn.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gumweqoui.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gitcyymfn.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gclewrhgp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gvgwufznq.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gbvuewhbh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gskgufazj.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gwrllzzuk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gepttjepk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/grsgfhdfh.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gfwekwaux.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gvwlvpbgr.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gdnxtdhvc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gkungzwtu.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gxbdtrmsk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gxosffyvr.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gyombkjfj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/guftkojou.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gqxxaljmz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grovnvekr.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gudsyuijw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbxsqmqmk.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gfqsimwjy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdzrlrjae.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gedlscnfv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkmryawxu.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/goxrssuhf.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkbmeyexu.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/giefcyqjr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/guansdhbl.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gohyoiids.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gxorlxryk.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gavxhzqsu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gfgzdijsq.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gumxtuppv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gbqzqwekl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxmgzsxvd.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gorafhfny.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gepbznedf.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gerkgpwdu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gqanpnrln.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gslqjrjdl.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/ggmuwdtes.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqczwzfbq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gwnhxwrhf.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gelaspeqs.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/glevkepow.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gmajspyne.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gjdvsjtvt.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/girhxzagq.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gljgrpazz.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gbtzruwbg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/ggwxfjjgh.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gphmgggac.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gjfyvgmwl.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/guatoqesm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gxfgujhds.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gxwdbtwwp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gjogaltqu.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gbsfdbkqr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gkrsugaox.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gbexeikjo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/grueugfid.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gdpvpcwri.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gnwyfsyqg.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gtvypywoq.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gouemkhla.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gwecpimiz.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gjtleyqoy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gctleoroc.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gactuuoih.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gcscnhjjp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gsojpaypx.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gjtctrean.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gxnvuehtd.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/glfrxihsj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gyyhbinlw.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gquqyvtxp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gypdewzvr.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/goqvzkcfr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/glahctklo.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/ghqdpkbux.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gsoopzvnr.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gntrocgih.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gktbedayc.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gmbwbauaj.sHtML


<!-- 参考信息 -->